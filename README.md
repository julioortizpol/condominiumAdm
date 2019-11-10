# condominiumAdm
Este repositorio es para un sistema de transparencia para la administración de condominios

# Requisitos:

Proyectos: En caso de requerir una reparacion o algun embelleizimiento al edificio se crea un proyecto, el mismo tendra un costo el cual se divide equitativamente por los mienbros del edificio.


El sistema debera mostrar informacion sobre las personas que viven en el condominio, esta informacion se debera poder filtar por edificios y tendra que incluir minimo la siguiente informacion:
* Informacion primordial como Nombre, Apellido, edad, telefono movil, telefono hogar. 
* Informacion especifica como fecha de ingreso al residencial, ROL, Tipo de inquilino, edificio al que pertenece, # de apartamento.
  * Entiendase por ROL puesto dentro de directiva del edificio.
  * Entiendase por tipo de inquilino si vive alquilado, si es propietario o Dependiente.
     * Entiendase por dependiente que vive en el residencial con la persona que es responsable por el apartamento.


El sistema debera tener un apartado donde se muestren las finanzas por edificios(esto depende de como se administre el condominio). A este solo tendran acceso los mienbros del edificio, los administradores, el contable y el presidente del condominio:
  * RESUMEN Finanzas: Contendra una lista con mienbros del edificio espesificando si deben dinero, si se le debe dinero, o si estan al dia y el total del edificio en FONDO siendo este negativo si el edificio tiene deudas.
    * Cada usuario tendra un resumen personalizado con el movimiento de sus finanzas donde estara detallado el porque se presenta este monto, en base a pago de mantenimiento y finanzas de proyectos.
  * RESUMEN PAGO Mantenimiento: Contendra lista de mienbros del edificio y mostrara si pagaron o no el matenimiento ademas de cuanto deben de mantenimiento si es el caso.
  * Historial Pago de mantenimiento: En este apartado se mostrara el pago del mantenimiento mensual por condomine, con la fecha en la que realizaron el pago para el calculo de mora, ademas en cada mes se podra ver el detalle de los costos con su correspondientes facturas, cada condomine podra ver el desgloze de su monto con un historial por ciclo de pago de mantenimiento.
  * RESUMEN Finanzas por proyectos: En este apartado se muestra los condomines y el monto que deben o que le deben a un condomine por todos los proyectos, los proyectos aparte de los condomines tendra un apartado de FONDOS que saldria de los fondos acumulados por el pago del mantenimiento, cada condomine podra ver el desgloze de su monto con un historial que le dara la referencia de cada proyecto con su cargo.
  * EL FONDO: el fondo esun sobrante si existe del pago de mantenimiento, el mismo debera tener un historial de movimientos bien detallados, ya que se podra usar FONDO para deuda de mantenimiento del edificio, proyecto del edificio y  proyecto del condominio.
  
  
  * Detalle Finanzas por proyecto: Mostrar las finanzas de un proyecto, el total del mismo, el detalle de pago por condomine, los aportes materiales de los mismos si hubo alguno, pago pendiente de condomine, facturas del proyecto y afectados.

Se debera mostrar un resumen con una lista de las personas del edificio y la cantidad de dinero que pagaron o deben del mantenimiento. Asi mismo debera de existir un apartado de total donde se presenta el Fondo del apartamento si existe o 



El sistema debe tener dos versiones una movil y una web.

La version WEB:

Esta sera solo para administracion del sistema, sera como un CMS, para que los administradores del condominio puedan hacer los cambios a la base de datos de una manera mas sencilla.
