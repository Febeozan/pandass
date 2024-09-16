__1. Mostrar ultimas 10 filas del dataframe__
~~~~
print("Últimas 10 filas del DataFrame:")
print(df.tail(10))
~~~~
resultado:
~~~~
PS C:\Users\Pc9\Documents\Programas> & C:/Users/Pc9/AppData/Local/Programs/Python/Python312/python.exe c:/Users/Pc9/Documents/Programas/nombres.py
                          nombre  cantidad  anio
9761599          Joselin Diamela         1  2015
9761600            Sohee Marilyn         1  2015
9761601         Giovanna Desiree         1  2015
9761602    Xavier Lorenzo Daniel         1  2015
9761603    Benjamin Amadeo Adiel         1  2015
9761604         Antonella Paloma         1  2015
9761605  Briana Princesa Abigail         1  2015
9761606            Neylan Dilara         1  2015
9761607              Laya Jazmín         1  2015
9761608      Fiorella Luz Mailén         1  2015
PS C:\Users\Pc9\Documents\Programas> 
~~~~

__2 - Mostrar informacion del dataframe__
~~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

print(df.info())
~~~~
resultado:
~~~~
PS C:\Users\Pc9\Documents\Programas> & C:/Users/Pc9/AppData/Local/Programs/Python/Python312/python.exe c:/Users/Pc9/Documents/Programas/nombres.py
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 9761609 entries, 0 to 9761608
Data columns (total 3 columns):
 #   Column    Dtype
---  ------    -----
 0   nombre    object
 1   cantidad  int64
 2   anio      int64
dtypes: int64(2), object(1)
memory usage: 223.4+ MB
None
PS C:\Users\Pc9\Documents\Programas>
~~~~
__3 - Obtener valores estadisticos del dataframe__
~~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

print(df.describe())
~~~~
resultado:
~~~~
PS C:\Users\Pc9\Documents\Programas> & C:/Users/Pc9/AppData/Local/Programs/Python/Python312/python.exe c:/Users/Pc9/Documents/Programas/nombres.py
           cantidad          anio
count  9.761609e+06  9.761609e+06
mean   6.177199e+00  1.980137e+03
std    4.336806e+01  2.429556e+01
min    1.000000e+00  1.922000e+03
25%    1.000000e+00  1.961000e+03
50%    2.000000e+00  1.985000e+03
75%    3.000000e+00  2.001000e+03
max    7.939000e+03  2.015000e+03
PS C:\Users\Pc9\Documents\Programas> 
~~~~
__4 - Obtener el tamaño del dataframe__

~~~~
import pandas as pd

df = pd.read_csv('historico-nombres.csv')

print(df.shape)
~~~~
resultado:
~~~~
PS C:\Users\Pc9\Documents\Programas> & C:/Users/Pc9/AppData/Local/Programs/Python/Python312/python.exe c:/Users/Pc9/Documents/Programas/nombres.py
(9761609, 3)
PS C:\Users\Pc9\Documents\Programas>
~~~~
__5 - Seleccionar una columna con [] (forma preferida de seleccionar una columna)__

