# Evaluación Data engineering - Data analyst


| La evaluación constara de 3 puntos fundamentales: |                                                                                | % importancia |
|---------------------------------------------------|--------------------------------------------------------------------------------|---------------|
| 1                                                 | Capacidad de comprender un problema de negocio                                 | 20%           |
| 2                                                 | Capacidad de dar a conocer una situación de negocio con datos                  | 30%           |
| 3                                                 | Capacidad de entregar una solución de negocio (simple, entendible y escalable) | 50%           |


Por ser un cargo con capacidades técnicas, se requiere que al menos obtenga mas del 80%

# Contexto de la situación de negocio

Uno de los negocios principales para la empresa, es la venta de laminas protectoras de pantalla para telefonos movil; para este fin, la empresa ha dispuesto 5 puntos de venta. sin embargo, por condiciones de una alianza comercial de la empresa con un retail estrategico, en los puntos de venta se deben cumplir unas condiciones de abastecimiento y de antguedad de inventario, que son las siguientes:

1	Todos los puntos deben estar abastecidos con al menos 5000 laminas

2	El inventario de laminas en punto no puede ser más antiguo de 90 días

En caso de no cumplirse con esas especificaciones, el punto quedará deshabilitado para continuar atendiendo ventas
Actualmente existe la problemática de que no existe una forma de reportar y llevar control de las existencias de inventario de laminas por punto


## La necesidad de la empresa se puede resumir de la siguiente manera:


| 1 | Tener un reporte para identificar inventario envejecido (mas de 90 días) por punto y tomar medidas inmediatas                                                                                                                                                 |
|---|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 2 | Tener un reporte para identificar proactivamente inventario (entre 75 y 90 días) para planear estrategias anticipadas de rotación                                                                                                                             |
| 3 | Estrategia de rotación de laminas por ruta (tenga en cuenta que si se recoge el inventario envejecido en un punto y se lleva a otro, eso soluciona el problema). Esta estrategia debe ser un paso a paso de operación(ver ejemplo), y justifique su respuesta |
| 4 | Ordenar los puntos de venta de mayor a menor numero de ventas                                                                                                                                                                                                 |
| 5 | Identificar cual punto de venta lleva una estrategia optima en el control de inventario y ventas                                                                                                                                                              |


Ejemplo (paso a paso de rotación laminas)

1	Salir de la bodega principal con 3200 laminas

2	Ir al punto de venta 4: dejar 3200 y recoger 4200 de mas de 90 días

3	Ir al punto de venta 3: recoger 700 de mas de 90 días

4	Ir al punt o de venta 2: recoger 1200 de mas de 90 días

5	Ir al punto de venta 1: dejar 2500 y recoger 2500 de mas de 90 días

6	ir al punto de venta 5: dejar 2200 y recoger 1200 de más de 90 días

7	Regresar a la bodega principal con 1900


# El ejercicio consiste en desarrollar una solución para las necesidades de negocio sujetas a:

*	Debe ser orientada a datos y no contener comentarios o deducciones no respaldadas en ellos

*	Debe ser de acceso facil a cualquier persona, clara e intuitiva en su contenido (se recomienda un servicio en una pagina html, o un tablero bi, cuya interpretación sea intuitiva)

*	Debe ser trazable y escalable (la información debe estar en una base de datos y todo reporte o visualización debe estar conectada a ella)

*	Debe soportar versionamiento de código, de tal forma que nuevos o futuros desarrolladores puedan trabajar en el mismo proyecto (git, github)

## Las fuentes de información disponibles para el desarrollo del ejercicio se encuentran adjuntas en este mismo repositorio en la carpeta "results" y se describen de la siguiente forma:

1	La información entregada en los excel con nomenclatura (P#_entrega_AAAA-MM-DD.xlsx) corresponde al registro de laminas abastecidas a 5 puntos de venta desde bodega

2	La información entregada en los excel con nomenclatura (P#_ventas_AAAAMMDD.xlsx) corresponde al registro de laminas vendidas en los 5 puntos de venta

3	Considere la siguiente ubicación geo-espacial de los puntos (en la optimización de la estrategia de ruta):

| punto | latitud | longitud |
|-------|---------|----------|
| P1    | 1       | 1        |
| P2    | -2      | 1        |
| P3    | -2      | -2       |
| P4    | -1      | -1       |
| P5    | 3       | 2        |

Le deseo exitos en su desempeño!


