# procesos_python
Serie de procesos realizados con regularidad en el procesamiento de información
<br><br>

Concatenar columnas, agregando un separador y omitiendo nulos
```
df['concatenada'] = df[['col1', 'col2', 'col3']].astype(str).agg(lambda x: ', '.join(x.dropna()), axis=1)
```
<br><br>


Obtener aquellos elementos del DF1 que se encuentran en el DF2
```
DF2[DF2['A'].isin(DF1['A'])]
```
<br><br>

Obtener aquellos elementos del DF1 que no se encuentran en el DF2
```
DF2[~DF2['A'].isin(DF1['A'])]
```
<br><br>

Cambiar el tipo de dato de una columna a texto y rellenar con ceros a la izquierda
```
df["columna_numeros"] = df["columna_numeros"].astype(str).str.zfill(6)
```
<br><br>
Filtrar registros de acuerdo a uno o más valores dentro de una columna
```
df_sub = df[df["columna"].isin(["valor1", "valor2", "valor3"])]
```
<br><br>

Filtrar registros de acuerdo a valores en multiples columnas
```
df_sub = df[(df["columna1"].isin(["valorA", "valorB"])) & (df["columna2"].isin(["valorX", "valorY"]))]

```
<br><br>
## Geopandas
Extraer los valores de aquellas entidades que coinciden espacialmentte




```

```


```

```
