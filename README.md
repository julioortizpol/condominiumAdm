# condominiumAdm
Este repositorio es para un sistema de transparencia para la administración de condominios

# Requisitos:

## La aplicacion cuenta de los siguientes  factores:

Condominio: Abarcado todos los edificios.

Proyectos: En caso de requerir una reparacion o algun embelleizimiento al edificio se crea un proyecto, el mismo tendra un costo el cual se divide equitativamente por los mienbros del edificio. Los proyectos pueden ser por edificios o para el condominio. Los proyectos tienen finanzas.

Edificios: Los edificios manejan proyectos, tienen apartamentos, tienen finanzas en funcion a los apartamentos, tienen gastos asociados.

Apartamento: Los apartamentos pagan la cuenta de edificios, crean proyectos para edificio, tienen condomines.

Condomines: Personas que viven en los apartamentos, pueden ser propietarios o vivir arquilados.

* Las finanzas de edificio se atribuyen a apatamento, y el responsable directo es el propietario del mismo. 
 ** Todos los apartamentos deben tener un propietario.

Las finanzas de proyectos y mantenimiento se manejan por separado.

El sistema debe tener dos versiones una movil y una web.

## La version Movil:

El sistema debera mostrar informacion sobre las personas que estan relacionadas con el condominio: Empleados(aunque no sean directos del residencial), inquilinos, propietarios, etc.

En caso de los empleados debe de mostrar la siguiente informacion:
 * Nombre, apellido, foto, cargo, responsabilidades bien detalladas, horario en el que se encontrara en la plaza.
 
En caso de los condomines, esta informacion se debera poder filtar por edificios y tendra que incluir minimo la siguiente informacion:
* Informacion primordial como Nombre, Apellido, edad, telefono movil, telefono hogar.
* Informacion especifica como fecha de ingreso al residencial, ROL, Tipo de inquilino, edificio al que pertenece, # de apartamento.
  * Entiendase por ROL puesto dentro de directiva del edificio.
  * Entiendase por tipo de inquilino si vive alquilado, si es propietario o Dependiente.
     * Entiendase por dependiente que vive en el residencial con la persona que es responsable por el apartamento.


El sistema debera tener un apartado donde se muestren las finanzas por edificios(esto depende de como se administre el condominio). A este solo tendran acceso los mienbros del edificio, los administradores, el contable y el presidente del condominio:
  * RESUMEN PAGO Mantenimiento: Contendra lista de mienbros del edificio y mostrara si pagaron o no el matenimiento ademas de cuanto deben de mantenimiento si es el caso.
    * Para el usuario ver su historial en este apartado debera referirse a historial pago de mantenimiento o a su historial en el resumen de pagos.
  * Historial Pago de mantenimiento: En este apartado se mostrara el pago del mantenimiento mensual por condomine, con la fecha en la que realizaron el pago para el calculo de mora, ademas en cada mes se podra ver el detalle de los costos con su correspondientes facturas, cada condomine podra ver el desgloze de su monto con un historial por ciclo de pago de mantenimiento.
  * RESUMEN Finanzas por proyectos: En este apartado se muestra los apartamentos y el monto que deben o que le deben a un condomine por todos los proyectos, los proyectos aparte de los condomines tendra un apartado de FONDOS que saldria de los fondos acumulados por el pago del mantenimiento.
  * Historial Finanzas por proyectos: En este apartado se muestran todos los proyectos y el monto que deben o que le deben a un condomine por cada proyecto, asi como el cargo al FONDO si existe, y un acceso rapido al detalle del proyecto.
  * Cada usuario tendra un resumen personalizado con el movimiento de sus finanzas donde estara detallado el porque se presenta este monto, en esta tendra dos secciones la de mantenimiento y proyecto, pues las mismas no deben de sumarse NUNCA. Esta informacion debera estar segmentada por mes, y dar la opcion de mostrar por mes el total de dinero y los movimientos asociados a los montos.
  * EL FONDO: el fondo es un sobrante si existe del pago de mantenimiento, el mismo se comportara como un usuario, digase que debera tener un historial de movimientos bien detallados, ya que se podra usar FONDO para deuda de mantenimiento del edificio, proyecto del edificio y  proyecto del condominio. El fondo se acumula en mantenimiento y se resta en proyecto o en el mismo mantenimeinto.
  
  
En el sistema se podran crear proyectos todos podran acceder a los proyectos exepto por la parte de finanza, en la cual solo lo podra ver los edificios involucrados en el proyecto, el administrador, presidente, contable.
Ademas de los edificos el condominio tambien puede tener proyectos, todos los arreglos a las areas comunes se consideran proyectos.
  * Los proyectos tienen una fecha de inicio y una fecha de fin, una descripcion, un titulo, un bloque de finanzas, detalles de pago, facturas, etc.
  * Bloque de Finanzas de proyecto: Mostrar las finanzas de un proyecto, el total del mismo, el detalle de pago por condomine, los aportes materiales de los mismos si hubo alguno, pago pendiente de condomine, facturas del proyecto y afectados.
  * El proyecto debe de presentarse como una obra, esto sirve para medir la labor de la administracion.
  
## La version WEB:

Esta sera solo para administracion del sistema, sera como un CMS, para que los administradores del condominio puedan hacer los cambios a la base de datos de una manera mas sencilla en lo que a UI se refiere. Aunque el UI sera mas sencillo la version WEB debe incluir todo lo mencionado anteriormente pero con la opcion de editar.

Desde esta plataforma podra:
Crear inquilinos asociados a un apartamento.
Agregar o modificar informacion de los inquilinos.
Crear proyectos.
Editar informacion de los proyectos
Editar la informacion financiera. Subir las facturas sobre los gastos de mantenimiento o de los proyectos.
Asignar permisos a editar un proyecto para un condomine.
