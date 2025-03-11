# procesos_python
Serie de procesos realizados con regularidad en el procesamiento de información

Obtener aquellos elementos del DF1 que se encuentran en el DF2
```
DF2[DF2['A'].isin(DF1['A'])]
```

Obtener aquellos elementos del DF1 que no se encuentran en el DF2
```
DF2[~DF2['A'].isin(DF1['A'])]
```
Cambiar el tipo de dato de una columna a texto y rellenar con ceros a la izquierda
```
df["columna_numeros"] = df["columna_numeros"].astype(str).str.zfill(6)
```

## Geopandas
Extraer los valores de aquellas entidades que coinciden espacialmentte




```

```


```

```
