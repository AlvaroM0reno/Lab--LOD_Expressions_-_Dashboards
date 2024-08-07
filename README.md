# Laboratorio | Expresiones LOD y Dashboards
En este laboratorio, continuará trabajando con el mismo libro de trabajo de Tableau del último laboratorio (laboratorio 6.2). Como recordatorio rápido, estaba usando archivos abTesting.csvy case_study_ab_test.md. Si necesita revisar nuevamente el archivo del estudio de caso, puede encontrarlo en files_for_lab/case_study_ab_test.md.

Instrucciones
En el siguiente gráfico, queremos analizar los clientes de group 1(de los grupos de edad que creamos a partir de la columna clnt_age). El objetivo es encontrar y filtrar aquellos participantes cuyo saldo de cuenta sea menor que el promedio del grupo. Siga estos pasos:

Crea un campo calculado con expresión LOD como { FIXED [clnt_age (group)] : AVG([Bal]) }.
Cree otro campo calculado para almacenar la diferencia entre el saldo promedio del grupo y el saldo del individuo como { FIXED [Client Age]: AVG([Bal]) } - { FIXED [Client Id]: AVG([Bal]) }.
Agregar Client_IDsa las filas. Filtrar todos los clientes excepto group_1.
Agregar saldo promedio para cada cliente.
Ordene los datos en orden ascendente de equilibrio.
Agregue el campo calculado con la expresión LOD.
Añade el campo calculado con la diferencia.
Agregar filtro para los valores de diferencia para seleccionar sólo valores positivos (es decir, casos donde el saldo individual es menor que el saldo promedio del grupo).
Tiene gráficos del laboratorio anterior. Utilícelos para crear un panel interactivo para los usuarios.
