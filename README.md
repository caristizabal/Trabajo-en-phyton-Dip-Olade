# Trabajo-en-phyton-Dip-Olade
Contiene el primer ejercicio de clase real con Phyton

I# **_Informe de aportes hidrológicos para el año 2004_**

+ la tendencia mundial es utilizar markdown,pq se convierte a html y es más facil

+ Con la tecla Esc verde (comando: markdown txt y se muestra en formato html ) y la Azul (código de phyton)

+ con la forma **word** se muestra en negrilla _word_ cursiva

* En azul + la l, le da numeración dentro la celda a las líneas
* ## es subsección

## Este es un ejemplo de clase sobre la manipulación de datos usando phyton

* help open: ayuda en el comando

# **Comandos**

+ con el comando %load XXX.txt abro cualquier tipo de archivo de texto en la línea de comando. Además, puedo crear archivos de texto en Jupyter

* Con el comando %%write file demo2.txt y debajo lo que se quiere guardar 
+ Para encontrar ayuda con las magic cells o comamndos se busca en google **''iphyton magic cells''**
+ El comando ''!head'' muestra las primeras 10 líneas del archivo
+ !wc l nombre del archivo
* pandas es una libreria de phyton para la manipulación de datos en cualquier formato. ''import pandas as pd''. Se hace un sola vez
* Para instalar una librería se hace ''!pip nomlibreria''
* ''$ pip search palabra_relacionada_con_el_paquete''
* x=pd.read_csv('AportesDiario_2004.csv', sep=';', decimal=',',thousands='.',skiprows=3), me guarda la matriz de la base de datos en x, y con el comamndo x['YY'] me busca todos los datos de YY

import pandas as pd
import statistics

x=pd.read_csv('AportesDiario_2004.csv',sep=';', decimal=',',thousands='.',skiprows=3)
x
rio=x['Nombre Rio']

n=set(x['Nombre Rio'])
n
