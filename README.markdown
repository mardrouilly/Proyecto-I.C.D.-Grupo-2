---
jupyter:
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
  language_info:
    codemirror_mode:
      name: ipython
      version: 3
    file_extension: .py
    mimetype: text/x-python
    name: python
    nbconvert_exporter: python
    pygments_lexer: ipython3
    version: 3.11.4
  nbformat: 4
  nbformat_minor: 5
---

::: {#7e2741b1 .cell .markdown}
# PROYECTO CIENCIA DE DATOS: ¿COMO SE RELACIONAN LAS TASAS DE SUICIDIOS CON ALGUNOS DE LOS PRINCIPALES INDICES ESTADISTICOS QUE DESCRIBEN LA SITUACION SOCIO-ECONOMICA DE UN PAIS-CONTINENTE-REGION?
:::

::: {.cell .markdown}
### CONTEXTO Y MOTIVACION

Elegimos este proyecto porque nos interesa estudiar el problema del
suicidio, que es una de las principales causas de muerte en el mundo y
más dolorosas, por lo silenciosa que puede ser. Además, tiene múltiples
factores de riesgo, entre ellos el nivel socioeconómico. Según la OMS,
el suicidio se puede prevenir con intervenciones oportunas, basadas en
evidencia y a menudo de bajo costo. Para ello, es necesario contar con
datos e información confiables y actualizados sobre el fenómeno. Por
eso, decidimos usar las herramientas que nos provee la ciencia de datos
para estudiar la relación entre la tasa de suicidios por zona y el
ingreso por familia en la zona, usando datos del INE y otras fuentes.
Nuestro análisis está dirigido a profesionales de la salud, educación,
política o medios de comunicación, que puedan usar nuestros resultados
para diseñar e implementar estrategias de prevención, intervención y
sensibilización sobre el suicidio.
:::

::: {#7128af86 .cell .markdown}
### PREGUNTAS

-   ¿Existe una correlación significativa entre la tasa de suicidios y
    el promedio de ingresos a nivel nacional en diferentes países?, si
    es que existe ¿Cómo ha evolucionado a lo largo de la última década?
-   ¿Cómo han evolucionado las tasas de suicidios en diferentes países a
    lo largo de la última década? (Países con mayor aumento y países con
    menor aumento)
-   ¿Existe una relación entre la tasa de suicidios de un país por cada
    100.000 habitantes y el nivel educativo de estos?
-   ¿Cómo afecta la religión a la tasa de suicidios en diferentes
    países?
-   ¿Cómo influye el acceso a la tecnología en la tasa de suicidios en
    diferentes grupos demográficos?
-   ¿Se relaciona la tasa de suicidios con la esperanza de vida de los
    países?
:::

::: {.cell .markdown}
### DATOS USADOS

-   [Ingreso
    Promedio](https://www.datosmundial.com/ingreso-promedio.php)
-   [Average Wage per
    country](https://en.wikipedia.org/wiki/List_of_countries_by_average_wage)
-   [Religiones](https://countryeconomy.com/demography/religions)
-   [Suicide
    Rate](https://en.wikipedia.org/wiki/List_of_countries_by_suicide_rate)
-   [Population
    2010](https://en.wikipedia.org/wiki/List_of_countries_by_population_in_2010)
-   [Religious Composition
    2010-2050](https://www.pewresearch.org/religion/wp-content/uploads/sites/7/2015/04/Religious_Composition_by_Country_2010-2050.xlsx)
-   [Internet Users by
    Country](https://en.wikipedia.org/wiki/List_of_countries_by_number_of_Internet_users)
-   [Population by country
    (General)](https://www.worldometers.info/world-population/population-by-country/)
-   [Internet
    Usage](https://www.statista.com/statistics/184691/internet-usage-in-the-us-by-state/)
-   [life expectancy](https://www.worldbank.org/)
-   <https://data.who.int/indicators/i/16BBF41>
-   [Censo poblacion
    Chile](https://www.ine.gob.cl/estadisticas/sociales/censos-de-poblacion-y-vivienda/censo-de-poblacion-y-vivienda)
-   [Internet Usage by state
    US](https://www.statista.com/statistics/184691/internet-usage-in-the-us-by-state/)

Ademas, adjuntamos una carpeta de onedrive con todos los datos
utilizados en una carpeta, ya que no es posible subir todo a una carpeta
dentro de github:
[LINK](https://uccl0-my.sharepoint.com/:f:/g/personal/mardrouilly_uc_cl/EjSPKCYgGqlGvP07m517XcwB7RhDs7H64J2DiT1WZcN4jg?e=4DYqno)
:::

::: {.cell .markdown}
### RESUMEN DE LOS RESULTADOS

El análisis de los datos revela diversas relaciones y tendencias en las
tasas de suicidio a nivel global, considerando factores como ingreso
promedio, región geográfica, cambios a lo largo del tiempo, nivel
educativo, religión y acceso a internet. Se destaca la dinámica de las
relaciones socioeconómicas, como el cambio de una asociación inversa a
una positiva entre ingreso promedio y tasas de suicidio en la última
década.

Se observa que las tasas de suicidio varían según la región, con cambios
significativos en Europa y América en comparación con otras regiones. A
nivel mundial, la última década ha experimentado una disminución general
en las tasas de suicidio, aunque existen variaciones regionales.

La relación entre el nivel educativo y las tasas de suicidio presenta
desafíos para el análisis, indicando que la correlación se ve limitada a
través de variables como la edad o el género. No se puede afirmar con
certeza que exista una relación directa entre el nivel educativo y las
tasas de suicidio en Chile, subrayando la naturaleza multifactorial de
estos fenómenos.

Se aborda la correlación entre la religión y las tasas de suicidio,
donde se destaca que hay religiones con tasas más altas o más bajas,
pero la relación es compleja y no se puede simplificar a una única
variable. Se resalta que la prevención del suicidio demanda un enfoque
integral que considere factores diversos, como la salud mental, el
respaldo social y el acceso a la atención médica.

En cuanto a la correlación entre el acceso a internet y las tasas de
suicidio, se encuentra una relación mínima y prácticamente nula,
sugiriendo que no hay una correlación directa a nivel global entre la
penetración de internet y las tasas de suicidio.

En el caso de la esperanza de vida, se concluye que, aunque existe
alguna relación estadística, no es un predictor robusto por sí solo para
explicar las variaciones en las tasas de suicidio entre países. Otros
factores no capturados por la esperanza de vida influyen de manera
significativa en estas tasas.
:::

::: {.cell .markdown}
### ¿QUE PODRÍA SALIR MAL?

En el proyecto de ciencia de datos que llevaremos a cabo, nos
enfrentamos a posibles desafíos que podrían impactar la validez de
nuestras conclusiones. La disparidad en la calidad y disponibilidad de
datos entre países plantea un riesgo de sesgo y limitaciones en las
comparaciones que haremos. La complejidad de las relaciones causales
sociodemográficas y la posible omisión de variables cruciales podrían
conducir a interpretaciones erróneas en nuestro análisis. También
debemos ser conscientes de la importancia de considerar factores
culturales y contextuales para evitar distorsiones en nuestras
conclusiones. Además, la interpretación simplista de tendencias y la
falta de atención a variables de confusión podrían comprometer la
precisión de nuestros resultados y, en última instancia, la efectividad
de las políticas resultantes que propondremos. En resumen, en este
proyecto de ciencia de datos, es crucial identificar y abordar estos
desafíos para asegurar la robustez y aplicabilidad de nuestros hallazgos
:::

::: {.cell .markdown}
-   Ignorar que la Correlacion no implica causalidad
-   Haber elegido visualizaciones y graficos incorrectos, que no aportan
    informacion importante
-   No considerar el bias(sesgo) de los datos. \"Tus resultados son tan
    buenos como tus datos\". Desafortunadamente, a menudo no tenemos
    exactitud sobre como o donde se recopilan los datos. Es por tal que,
    debemos considerar si hay un bias presente o no.
:::

::: {#f2eaeb80 .cell .code execution_count="1"}
``` python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import geopandas as gpd
import requests as rq
from bs4 import BeautifulSoup as bs
import re
```
:::

::: {.cell .markdown}
IMPORTAMOS LAS LIBRERIAS QUE USAREMOS
:::

::: {#d14c0b0d .cell .markdown}
\## 1. ¿Existe una correlación significativa entre la tasa de suicidios
y el promedio deingresos a nivel nacional en diferentes países?, si es
que existe ¿Cómo haevolucionado a lo largo de la última década?
:::

::: {.cell .code execution_count="2"}
``` python
#https://www.datosmundial.com/ingreso-promedio.php
ingresos_mundo= pd.read_csv('Datos/income.csv', sep=',')
ingresos_mundo.rename(columns={'LOCATION':'CodigoPais'}, inplace=True)
ingresos_mundo2019 = ingresos_mundo[ingresos_mundo["TIME"]==2019]
df_suicidio_oms= pd.read_excel('Datos/data.xlsx',skiprows=2)
pd.set_option('display.max_columns', None)
df_suicidio_oms.dropna(thresh=0.2, inplace=True)
df_suicidio_oms_clean=df_suicidio_oms[['ParentLocation','SpatialDimValueCode','Location','Period','Dim1','FactValueNumeric']].copy()
df_suicidio_oms_clean.rename(columns={'SpatialDimValueCode':'CodigoPais'}, inplace=True) 
suicidios2009 = df_suicidio_oms_clean[df_suicidio_oms_clean['Period'] == 2009]
suicidios2009 = suicidios2009[suicidios2009['Dim1'] == "Both sexes"]
#haremos un merge de los datos de suicidios con los datos de ingresos
suicidios2019 = df_suicidio_oms_clean[df_suicidio_oms_clean['Period'] == 2019]
suicidios2019 = suicidios2019[suicidios2019['Dim1'] == "Both sexes"]
suicidios_ingresos2019 = suicidios2019.merge(ingresos_mundo2019, on="CodigoPais")
suicidios_ingresos2019.rename(columns={'Value':'IngresoPromedio'}, inplace=True)
```
:::

::: {.cell .code execution_count="3"}
``` python
#agregaremos una columna que diga correlacion entre los datos de suicidios y los ingresos
suicidios_ingresos2019['Correlacion'] = suicidios_ingresos2019['FactValueNumeric'] / suicidios_ingresos2019['IngresoPromedio']
#quitaremos las variables que no necesitamos
suicidios_ingresos2019.drop(['TIME','Flag Codes','INDICATOR', 'SUBJECT', 'ParentLocation','FREQUENCY','MEASURE','Dim1', 'Period', 'Location'], axis=1, inplace=True)
suicidios_ingresos2019.rename(columns={'FactValueNumeric':'Suicidios_por_100'}, inplace=True)
#ordenamos por ingreso promedio
suicidios_ingresos2019.sort_values(by=['IngresoPromedio'], inplace=True, ascending=False)
```
:::

::: {.cell .code execution_count="4"}
``` python
url_wage = "https://en.wikipedia.org/wiki/List_of_countries_by_average_wage"
page_wage = rq.get(url_wage).text
soup_wage = bs(page_wage, 'html.parser')
tables_wage = soup_wage.find_all('table', {'class': 'wikitable'})

table_wage = tables_wage[0]
columns_wage = ["Country", "2000", "2010", "2020", "2022"]
df_wage = pd.DataFrame(columns=columns_wage)


for row in table_wage.find_all("tr")[1:]: 
    col = row.find_all(["th", "td"])
    if col:
        country = str(col[0].text.strip().replace('*', ''))
        avg_wage_2000 = col[1].text.strip()
        avg_wage_2010 = int(col[2].text.strip().replace(',', ''))
        avg_wage_2020 = col[3].text.strip()
        avg_wage_2022 = col[4].text.strip()  
        new_row = pd.Series(data={"Country": country, "2000": avg_wage_2000,
                                  "2010": avg_wage_2010, "2020": avg_wage_2020, "2022": avg_wage_2022})
        df_wage = pd.concat([df_wage, new_row.to_frame().T])

df_wage.columns = df_wage.columns.str.replace('*', '')
df_wage.reset_index(drop=True, inplace=True)
#nos quedamos solo con los datos de 2010
df_wage = df_wage[['Country', '2010']].copy()
df_wage.rename(columns={'2010':'IngresoPromedio'}, inplace=True)
df_wage = df_wage.sort_values(by="Country", ascending=True)
df_wage.reset_index(drop=True, inplace=True)
df_wage["Country"] = df_wage["Country"].astype(str)
```
:::

::: {.cell .code execution_count="5"}
``` python
url_suicide = "https://en.wikipedia.org/wiki/List_of_countries_by_suicide_rate"
page_suicide = rq.get(url_suicide).text
soup_suicide = bs(page_suicide, 'html.parser')
tables_suicide = soup_suicide.find_all('table', {'class': 'wikitable'})
table_suicide = tables_suicide[1]
columns_suicide = ["Country", "2010"]
df_suicide = pd.DataFrame(columns=columns_suicide)
for row in table_suicide.find_all("tr")[2:]:  
    col = row.find_all(["th", "td"])
    if col:
        country = str(col[0].text.strip().replace(' *', '')) 
        suicide_rate_2010 = float(col[10].text.strip())
        new_row = pd.Series(data={"Country": country, "2010": suicide_rate_2010})
        df_suicide = pd.concat([df_suicide, new_row.to_frame().T])

df_suicide.reset_index(drop=True, inplace=True)
df_suicide.rename(columns={'2010':'Suicidios_x_100k'}, inplace=True)
```
:::

::: {.cell .code execution_count="6"}
``` python
df_wage["Country"] = df_wage["Country"].apply(lambda x: re.sub(r'\W+', '', str(x).lower()))
df_suicide["Country"] = df_suicide["Country"].apply(lambda x: re.sub(r'\W+', '', str(x).lower()))
df_merged = pd.merge(df_wage, df_suicide, on="Country", how="inner")
df_merged_sorted = df_merged.sort_values(by="Country", ascending=True)
df_merged_sorted.reset_index(drop=True, inplace=True)
df_merged_sorted['Correlacion'] = df_merged_sorted['Suicidios_x_100k'] / df_merged_sorted['IngresoPromedio']
df_merged_sorted['IngresoPromedio'] = pd.to_numeric(df_merged_sorted['IngresoPromedio'], errors='coerce').fillna(0)
df_merged_sorted['Suicidios_x_100k'] = pd.to_numeric(df_merged_sorted['Suicidios_x_100k'], errors='coerce').fillna(0)
```
:::

::: {.cell .code execution_count="7"}
``` python
fig, axs = plt.subplots(2, 2, figsize=(12, 10))

sns.lineplot(data=df_merged_sorted, x="IngresoPromedio", y="Suicidios_x_100k", ax=axs[0, 0], color='blue')
axs[0, 0].set_title("Correlacion 2010")
axs[0, 0].set_xlabel("Ingreso promedio")
axs[0, 0].set_ylabel("Suicidios por 100.000 habitantes")

sns.lineplot(data=suicidios_ingresos2019, x="IngresoPromedio", y="Suicidios_por_100", ax=axs[0, 1], color='green')
axs[0, 1].set_title("Correlacion 2019")
axs[0, 1].set_xlabel("Ingreso promedio")
axs[0, 1].set_ylabel("Suicidios por 100.000 habitantes")

sns.regplot(data=df_merged_sorted, x="IngresoPromedio", y="Suicidios_x_100k", ax=axs[1, 0], scatter_kws={"color": "red"}, line_kws={"color": "orange"})
axs[1, 0].set_title("Correlacion 2010")
axs[1, 0].set_xlabel("Ingreso promedio")
axs[1, 0].set_ylabel("Suicidios por 100.000 habitantes")

sns.regplot(data=suicidios_ingresos2019, x="IngresoPromedio", y="Suicidios_por_100", ax=axs[1, 1], scatter_kws={"color": "purple"}, line_kws={"color": "pink"})
axs[1, 1].set_title("Correlacion 2019")
axs[1, 1].set_xlabel("Ingreso promedio")
axs[1, 1].set_ylabel("Suicidios por 100.000 habitantes")


plt.tight_layout()
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/ae7bfff521c8793447918515d2080cfdbd10e742.png)
:::
:::

::: {.cell .markdown}
Comparando las correlaciones en 2010 y 2019, notamos una transición de
una asociación inversa a una asociación positiva entre ingreso promedio
y suicidios por 100,000 habitantes. Este cambio destaca la naturaleza
dinámica de las relaciones socioeconómicas y subraya la importancia de
considerar múltiples factores en la interpretación de los resultados.
Acá, es importante reconocer que la correlación no implica causalidad y
que la interpretación de estos resultados debe ser cuidadosa. Además, la
aplicación de modelos de regresión lineal proporciona una herramienta
valiosa para cuantificar y visualizar estas relaciones complejas.
Creemos que un análisis más profundo que considere otros posibles
factores influyentes son necesarios para obtener una comprensión más
completa de la dinámica entre ingreso promedio y tasas de suicidio.
:::

::: {#9e8a9b52 .cell .markdown}
## 2. ¿Cómo han evolucionado las tasas de suicidios en diferentes países a lo largo de la última década? (Países con mayor aumento y países con menor aumento) (Josías) {#2-cómo-han-evolucionado-las-tasas-de-suicidios-en-diferentes-países-a-lo-largo-de-la-última-década-países-con-mayor-aumento-y-países-con-menor-aumento-josías}
:::

::: {.cell .code execution_count="8"}
``` python
nuevo_suicidios2009 = suicidios2009.rename(columns = {"FactValueNumeric" : "FVN09"}) 
nuevo_suicidios2009 = nuevo_suicidios2009.drop("Period", axis = 1)
nuevo_suicidios2019 = suicidios2019.rename(columns = {"FactValueNumeric" : "FVN19"})
nuevo_suicidios2019 = nuevo_suicidios2019.drop("Period", axis = 1)
```
:::

::: {.cell .code execution_count="9"}
``` python
df_merged = pd.merge(nuevo_suicidios2009, nuevo_suicidios2019, on = "CodigoPais" )
columnas_para_eliminar = ['ParentLocation_y', 'Location_y', 'Dim1_y']
df_merged = df_merged.drop(columnas_para_eliminar, axis=1)
df_merged = df_merged.rename(columns = {"ParentLocation_x" : "ParentLocation", "Location_x" : "Location", "Dim1_x" : "Dim1"})
aumento_suicidios = df_merged["FVN19"] - df_merged["FVN09"]
df_merged["Aumento_Tasa"] = aumento_suicidios
df_merged
```

::: {.output .execute_result execution_count="9"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ParentLocation</th>
      <th>CodigoPais</th>
      <th>Location</th>
      <th>Dim1</th>
      <th>FVN09</th>
      <th>FVN19</th>
      <th>Aumento_Tasa</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Africa</td>
      <td>AGO</td>
      <td>Angola</td>
      <td>Both sexes</td>
      <td>6.69</td>
      <td>6.08</td>
      <td>-0.61</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Africa</td>
      <td>BDI</td>
      <td>Burundi</td>
      <td>Both sexes</td>
      <td>7.73</td>
      <td>6.24</td>
      <td>-1.49</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Africa</td>
      <td>BEN</td>
      <td>Benin</td>
      <td>Both sexes</td>
      <td>8.46</td>
      <td>7.81</td>
      <td>-0.65</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Africa</td>
      <td>BFA</td>
      <td>Burkina Faso</td>
      <td>Both sexes</td>
      <td>7.97</td>
      <td>7.48</td>
      <td>-0.49</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Africa</td>
      <td>BWA</td>
      <td>Botswana</td>
      <td>Both sexes</td>
      <td>25.12</td>
      <td>16.05</td>
      <td>-9.07</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>178</th>
      <td>Western Pacific</td>
      <td>SLB</td>
      <td>Solomon Islands</td>
      <td>Both sexes</td>
      <td>15.79</td>
      <td>14.67</td>
      <td>-1.12</td>
    </tr>
    <tr>
      <th>179</th>
      <td>Western Pacific</td>
      <td>TON</td>
      <td>Tonga</td>
      <td>Both sexes</td>
      <td>4.28</td>
      <td>3.82</td>
      <td>-0.46</td>
    </tr>
    <tr>
      <th>180</th>
      <td>Western Pacific</td>
      <td>VNM</td>
      <td>Viet Nam</td>
      <td>Both sexes</td>
      <td>6.94</td>
      <td>7.51</td>
      <td>0.57</td>
    </tr>
    <tr>
      <th>181</th>
      <td>Western Pacific</td>
      <td>VUT</td>
      <td>Vanuatu</td>
      <td>Both sexes</td>
      <td>19.75</td>
      <td>18.03</td>
      <td>-1.72</td>
    </tr>
    <tr>
      <th>182</th>
      <td>Western Pacific</td>
      <td>WSM</td>
      <td>Samoa</td>
      <td>Both sexes</td>
      <td>11.00</td>
      <td>12.55</td>
      <td>1.55</td>
    </tr>
  </tbody>
</table>
<p>183 rows × 7 columns</p>
</div>
```
:::
:::

::: {.cell .code execution_count="10"}
``` python
print(len(df_merged[df_merged["Aumento_Tasa"] < 0]))
```

::: {.output .stream .stdout}
    130
:::
:::

::: {.cell .code execution_count="11"}
``` python
print(len(df_merged[df_merged["Aumento_Tasa"] >= 0]))
```

::: {.output .stream .stdout}
    53
:::
:::

::: {.cell .markdown}
Según nuestros datos, tenemos que la tasa de suicidios en una decada
(2009 - 2019) aumentó en 53 países (28,96%), mientras que en 130
disminuyó (71,04%)
:::

::: {.cell .code execution_count="12"}
``` python
df_sorted = df_merged.sort_values(by='Aumento_Tasa')
cinco_menores = df_sorted['Aumento_Tasa'].head(5)
df_merged[df_merged['Aumento_Tasa'].isin(cinco_menores)]
```

::: {.output .execute_result execution_count="12"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ParentLocation</th>
      <th>CodigoPais</th>
      <th>Location</th>
      <th>Dim1</th>
      <th>FVN09</th>
      <th>FVN19</th>
      <th>Aumento_Tasa</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>38</th>
      <td>Africa</td>
      <td>SWZ</td>
      <td>Eswatini</td>
      <td>Both sexes</td>
      <td>54.24</td>
      <td>29.40</td>
      <td>-24.84</td>
    </tr>
    <tr>
      <th>108</th>
      <td>Europe</td>
      <td>BLR</td>
      <td>Belarus</td>
      <td>Both sexes</td>
      <td>36.54</td>
      <td>21.20</td>
      <td>-15.34</td>
    </tr>
    <tr>
      <th>127</th>
      <td>Europe</td>
      <td>KAZ</td>
      <td>Kazakhstan</td>
      <td>Both sexes</td>
      <td>30.26</td>
      <td>17.57</td>
      <td>-12.69</td>
    </tr>
    <tr>
      <th>129</th>
      <td>Europe</td>
      <td>LTU</td>
      <td>Lithuania</td>
      <td>Both sexes</td>
      <td>39.16</td>
      <td>26.14</td>
      <td>-13.02</td>
    </tr>
    <tr>
      <th>141</th>
      <td>Europe</td>
      <td>RUS</td>
      <td>Russian Federation</td>
      <td>Both sexes</td>
      <td>38.43</td>
      <td>25.11</td>
      <td>-13.32</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
Los 5 países con mayor disminución de tasa de suicidios son Suazilandia,
Bielorrusias, Kazajistán, Lituania y Rusia. A excepción de Suazilandia,
los países en cuestión pertenecen a Europa del Este.
:::

::: {.cell .code execution_count="13"}
``` python
df_sorted = df_merged.sort_values(by='Aumento_Tasa')
cinco_mayores = df_sorted['Aumento_Tasa'].tail(5)
df_merged[df_merged['Aumento_Tasa'].isin(cinco_mayores)]
```

::: {.output .execute_result execution_count="13"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ParentLocation</th>
      <th>CodigoPais</th>
      <th>Location</th>
      <th>Dim1</th>
      <th>FVN09</th>
      <th>FVN19</th>
      <th>Aumento_Tasa</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>23</th>
      <td>Africa</td>
      <td>LSO</td>
      <td>Lesotho</td>
      <td>Both sexes</td>
      <td>63.27</td>
      <td>72.44</td>
      <td>9.17</td>
    </tr>
    <tr>
      <th>63</th>
      <td>Americas</td>
      <td>GUY</td>
      <td>Guyana</td>
      <td>Both sexes</td>
      <td>32.85</td>
      <td>40.28</td>
      <td>7.43</td>
    </tr>
    <tr>
      <th>76</th>
      <td>Americas</td>
      <td>URY</td>
      <td>Uruguay</td>
      <td>Both sexes</td>
      <td>14.95</td>
      <td>21.24</td>
      <td>6.29</td>
    </tr>
    <tr>
      <th>77</th>
      <td>Americas</td>
      <td>USA</td>
      <td>United States of America</td>
      <td>Both sexes</td>
      <td>12.76</td>
      <td>16.14</td>
      <td>3.38</td>
    </tr>
    <tr>
      <th>166</th>
      <td>Western Pacific</td>
      <td>FSM</td>
      <td>Micronesia (Federated States of)</td>
      <td>Both sexes</td>
      <td>24.49</td>
      <td>28.21</td>
      <td>3.72</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
En el caso de los 5 países con mayor aumento de la tasa de suicidios
tenemos a Lesoto, Guyana, Uruguay, Estados Unidos y Micronesia. Tenemos
en este caso 3 de los 5 países que pertenecen a América.

Veremos si existe una tendencia según la localidad del país.
:::

::: {.cell .code execution_count="14"}
``` python
fig, axs = plt.subplots(1, 2, figsize=(16, 6))

df_agrupado = df_merged.groupby('ParentLocation')['FVN09'].mean().reset_index()
sns.barplot(data=df_agrupado, x='ParentLocation', y='FVN09', ax=axs[0], palette='Oranges')
axs[0].set_xlabel('Región')
axs[0].set_ylabel('Promedio de Tasa de Suicidios 2009')
axs[0].set_title('Promedio de Tasa de Suicidios por Continente 2009')
media_2009 = np.mean(df_agrupado['FVN09'])
axs[0].axhline(y=media_2009, color='green', linestyle='--', label=f'Media: {media_2009:.2f}')
axs[0].legend()

df_agrupado19 = df_merged.groupby('ParentLocation')['FVN19'].mean().reset_index()
sns.barplot(data=df_agrupado19, x='ParentLocation', y='FVN19', ax=axs[1], palette='Blues')
axs[1].set_xlabel('Región')
axs[1].set_ylabel('Promedio de Tasa de Suicidios 2019')
axs[1].set_title('Promedio de Tasa de Suicidios por Continente 2019')
media_2019 = np.mean(df_agrupado19['FVN19'])
axs[1].axhline(y=media_2019, color='red', linestyle='--', label=f'Media: {media_2019:.2f}')
axs[1].legend()

plt.tight_layout()
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/ac69edc3919bf532da467d47d3af0ae3e436a86a.png)
:::
:::

::: {.cell .markdown}
Si bien hubo cambios en el promedio de la tasa de suicidios, se puede
observar que existe cierta tendencia en la relación de suicidios según
su región.

Un cambio significativo es el de Europa, que disminuyó la diferencia que
tenía con los países del Pacífico Oeste, al igual que América con
respecto a los países del sureste de Asia,

Podemos ver que a nivel global en la última decada hubo más disminución
que aumento en la tasa de suicidios por país, y que hay tendencias según
la localidad de estos países, por lo que pueden haber factores que
afecten las tasas de suicidios, como cultura, avances en tratamiento de
la salud mental, desarrollo económico, etc.
:::

::: {#790172f6 .cell .markdown}
# 3. ¿Existe una relación entre la tasa de suicidios de Chile por cada 100.000 habitantes y el nivel educativo de estos? {#3-existe-una-relación-entre-la-tasa-de-suicidios-de-chile-por-cada-100000-habitantes-y-el-nivel-educativo-de-estos}
:::

::: {#7ae98adb .cell .code execution_count="15"}
``` python
datasuicidios_chile_2 = pd.read_csv("Datos/16BBF41_ALL_LATEST.csv")
suicidios_chile_2 = datasuicidios_chile_2[datasuicidios_chile_2["GEO_NAME_SHORT"] == "Chile"]
suicidios_chile_2 = suicidios_chile_2[["DIM_TIME","DIM_SEX","DIM_AGE","VALUE_NUMERIC"]]
suicidios_chile_2.rename(columns={"DIM_TIME":"AÑO","DIM_SEX":"SEXO","DIM_AGE":"EDADES","VALUE_NUMERIC":"MUERTES"}, inplace=True)
edades_deseadas = ["15 to 24 years", "25 to 34 years", "35 to 44 years", "45 to 54 years", "55 to 64 years", "65 to 74 years", "75 to 84 years", "85 plus years"]
df_suicidios = suicidios_chile_2[(suicidios_chile_2["AÑO"] == 2019) & (suicidios_chile_2["SEXO"] == "Total")]
df_suicidios = df_suicidios[df_suicidios["EDADES"].isin(edades_deseadas)]
df_suicidios["MUERTES"] = round(df_suicidios["MUERTES"],1)
df_suicidios = df_suicidios[["EDADES","MUERTES"]]
df_suicidios
```

::: {.output .execute_result execution_count="15"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>EDADES</th>
      <th>MUERTES</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>12047</th>
      <td>25 to 34 years</td>
      <td>10.1</td>
    </tr>
    <tr>
      <th>12048</th>
      <td>45 to 54 years</td>
      <td>13.7</td>
    </tr>
    <tr>
      <th>12049</th>
      <td>55 to 64 years</td>
      <td>12.3</td>
    </tr>
    <tr>
      <th>12100</th>
      <td>35 to 44 years</td>
      <td>11.8</td>
    </tr>
    <tr>
      <th>12101</th>
      <td>75 to 84 years</td>
      <td>13.8</td>
    </tr>
    <tr>
      <th>12110</th>
      <td>15 to 24 years</td>
      <td>7.4</td>
    </tr>
    <tr>
      <th>12111</th>
      <td>85 plus years</td>
      <td>14.5</td>
    </tr>
    <tr>
      <th>12256</th>
      <td>65 to 74 years</td>
      <td>10.7</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .code execution_count="16"}
``` python
df = pd.read_csv("Datos/Microdato_Censo2017-Personas.csv", sep=";")
columnas = ["P08", # Sexo
            "P09", # Edad
            "P13", # Asiste actualmente a la educación formal
            "P14", # Curso o año más alto aprobado
            "P15", # Nivel del curso más alto aprobado
            "P15A" # Completó el nivel especificado
            ]
df = df[columnas]
df.rename(columns={"P08":"Sexo","P09":"Edad","P13":"Estudia",
                   "P14":"Año","P15":"Nivel","P15A":"Completado"}, inplace=True)
df.replace({99:np.nan, 98:np.nan}, inplace=True)
df_clean = df.dropna()
```
:::

::: {.cell .code execution_count="17"}
``` python
df_clean["Edad"] = df_clean["Edad"].astype(int)
df_clean["Estudia"] = df_clean["Estudia"].astype(int)
df_clean["Año"] = df_clean["Año"].astype(int)
df_clean["Nivel"] = df_clean["Nivel"].astype(int)
df_clean["Completado"] = df_clean["Completado"].astype(int)
df_clean["Sexo"].replace({1:"Hombre",2:"Mujer"},inplace=True)
df_clean["Estudia"].replace({1:"Si",2:"No",3:"Nunca"},inplace=True)
df_clean["Nivel_Nombre"] = df_clean["Nivel"].replace({1:"Sala cuna o jardín infantil",
                            2:"Prekínder",
                            3:"Kínder",
                            4:"Especial o diferencial",
                            5:"Educación básica",
                            6:"Primaria o preparatorio (sistema antiguo)",
                            7:"Científico-humanista",
                            8:"Técnica profesional",
                            9:"Humanidades (sistema antiguo)",
                            10:"Técnica comercial, industrial/normalista (sistema antiguo)",
                            11:"Técnico superior (1-3 años)",
                            12:"Profesional (4 o más años)",
                            13:"Magíster",
                            14:"Doctorado"}, inplace=True)
df_clean["Completado"].replace({1:"Si",2:"No"},inplace=True)

categorias = ["15 to 24 years","25 to 34 years","35 to 44 years","45 to 54 years","55 to 64 years","65 to 74 years","75 to 84 years","85 plus years"]
df_clean["EDADES"] = pd.cut(df["Edad"], bins=[15,25,35,45,55,65,75,85,float("inf")], labels=categorias, include_lowest=True, right=False)
```

::: {.output .stream .stderr}
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:1: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame.
    Try using .loc[row_indexer,col_indexer] = value instead

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Edad"] = df_clean["Edad"].astype(int)
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:2: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame.
    Try using .loc[row_indexer,col_indexer] = value instead

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Estudia"] = df_clean["Estudia"].astype(int)
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:3: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame.
    Try using .loc[row_indexer,col_indexer] = value instead

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Año"] = df_clean["Año"].astype(int)
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:4: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame.
    Try using .loc[row_indexer,col_indexer] = value instead

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Nivel"] = df_clean["Nivel"].astype(int)
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:5: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame.
    Try using .loc[row_indexer,col_indexer] = value instead

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Completado"] = df_clean["Completado"].astype(int)
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:6: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Sexo"].replace({1:"Hombre",2:"Mujer"},inplace=True)
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:7: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Estudia"].replace({1:"Si",2:"No",3:"Nunca"},inplace=True)
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:8: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Nivel_Nombre"] = df_clean["Nivel"].replace({1:"Sala cuna o jardín infantil",
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:8: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame.
    Try using .loc[row_indexer,col_indexer] = value instead

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Nivel_Nombre"] = df_clean["Nivel"].replace({1:"Sala cuna o jardín infantil",
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:22: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["Completado"].replace({1:"Si",2:"No"},inplace=True)
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/2322813895.py:25: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame.
    Try using .loc[row_indexer,col_indexer] = value instead

    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      df_clean["EDADES"] = pd.cut(df["Edad"], bins=[15,25,35,45,55,65,75,85,float("inf")], labels=categorias, include_lowest=True, right=False)
:::
:::

::: {.cell .code execution_count="18"}
``` python
df_todo = pd.merge(df_clean, df_suicidios, how="left", on="EDADES")
df_todo = df_todo[["Sexo","Edad","Estudia","Año","Nivel","Completado","EDADES","MUERTES"]]
df_todo = df_todo.dropna()
grupo_mapping = {
    'Científico-humanista': 'media',
    'Educación básica': 'basica',
    'Profesional (4 o más años)': 'superior',
    'Técnica profesional': 'media',
    'Técnico superior (1-3 años)': 'superior',
    'Primaria o preparatorio (sistema antiguo)': 'basica',
    'Humanidades (sistema antiguo)': 'media',
    'Magíster': 'superior',
    'Técnica comercial, industrial/normalista (sistema antiguo)': 'media',
    'Doctorado': 'superior',
    'Especial o diferencial': 'basica',
    'Kínder': 'basica',
    'Sala cuna o jardín infantil': 'basica',
    'Prekínder': 'basica'
}
df_todo['Grupo'] = df_todo['Nivel'].map(grupo_mapping)
orden_categorias = ['basica', 'media', 'superior']
df_todo['Grupo'] = pd.Categorical(df_todo['Grupo'], categories=orden_categorias, ordered=True)
```
:::

::: {.cell .code execution_count="19"}
``` python
tabla = pd.crosstab(df_todo["Grupo"],df_todo["MUERTES"])
```
:::

::: {.cell .code execution_count="20"}
``` python
ax = tabla.plot(kind='bar', figsize=(10, 6))
ax.set_title('Suicidios cada 100.000 habitantes según su nivel educacional')
ax.set_xlabel('Nivel')
ax.set_ylabel('Cantidad de suicidios')
ax.legend(["7 --> [15,24] años", "10 --> [25,34] años", "11 --> [35,44] años", "12 --> [45,54] años", "12 --> [55,64] años", "14 --> [65,74] años", "14 --> [75,84] años", "15 --> [85,100] años"], title='Cantidad suicidios')
ax.set_xticklabels(tabla.index, rotation=45, ha='right')
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/9621e16916c99fc19ba8bdb09db55a75c7b4f7d8.png)
:::
:::

::: {.cell .markdown}
En este caso, se evidencia que la correlación entre el nivel educativo y
las tasas de suicidio presenta desafíos para su análisis, dado que la
única vía para vincular estos datos se limita a la edad (como lo hemos
abordado en este caso) o al género, siendo estas opciones un indicador
poco significativo para afirmar que el nivel educativo incide de manera
relevante en las tasas de suicidio. En consecuencia, no podemos afirmar
con certeza que exista una relación directa entre el nivel educativo y
las tasas de suicidio en Chile.

Las tasas de suicidio son fenómenos multifactoriales y no pueden ser
atribuidas de manera exclusiva a una única variable, como el nivel
educativo. No obstante, es crucial resaltar que la educación puede
desempeñar un papel significativo en la salud mental y el bienestar
general de las personas. Se requieren investigaciones adicionales para
comprender mejor esta correlación. Es esencial tener presente que la
prevención del suicidio demanda un enfoque integral que aborde diversos
factores, entre ellos la salud mental, el respaldo social y el acceso a
la atención médica.
:::

::: {#f0eeeba7 .cell .markdown}
# 4. ¿Cómo afecta la religión a la tasa de suicidios en diferentes países? {#4-cómo-afecta-la-religión-a-la-tasa-de-suicidios-en-diferentes-países}
:::

::: {.cell .markdown}
#### Obtencion de datos
:::

::: {.cell .code execution_count="21"}
``` python
url_porcentaje_creyentes = "https://countryeconomy.com/demography/religions"
page = rq.get(url_porcentaje_creyentes).text
soup = bs(page)
tables = soup.find_all('table')

df_porcentaje_creyentes = pd.DataFrame(columns=["Countries","Religious"])

#Solo hay 1 tabla en la pagina, por lo que solo se toma la primera
for row in tables[0].tbody.find_all("tr"):
    col = row.find_all("td")
    if (col != []):
        country = col[0].text.strip()
        religion = col[1].text.strip()
        new_row = pd.DataFrame({"Countries":[country],"Religious":[religion]})
        df_porcentaje_creyentes = pd.concat([df_porcentaje_creyentes, new_row], ignore_index=True)
    
#Limpiar la columna countries
df_porcentaje_creyentes["Countries"] = df_porcentaje_creyentes["Countries"].str.split("[").str[0]
df_porcentaje_creyentes["Countries"] = df_porcentaje_creyentes["Countries"].str.strip()
#Dejar la columna religious con valor numerico
df_porcentaje_creyentes["Religious"] = df_porcentaje_creyentes["Religious"].str.replace("%","")
df_porcentaje_creyentes["Religious"] = df_porcentaje_creyentes["Religious"].astype(float)
df_porcentaje_creyentes.rename(columns={"Countries":"Location"}, inplace=True)
df_porcentaje_creyentes.rename(columns={"Religious":"Religious %"}, inplace=True)
```
:::

::: {.cell .code execution_count="22"}
``` python
url_population = "https://en.wikipedia.org/wiki/List_of_countries_by_population_in_2010"
page = rq.get(url_population).text
soup = bs(page)
tables = soup.find_all('table')

df_population = pd.DataFrame(columns=["Location","Population"])

#Usaremos la 2da tabla de la pagina
for row in tables[1].tbody.find_all("tr"):
    col = row.find_all("td")
    if (col != []):
        country = col[1].text.strip()
        population = col[2].text.strip()
        new_row = pd.DataFrame({"Location":[country],"Population":[population]})
        df_population = pd.concat([df_population, new_row], ignore_index=True)
```
:::

::: {.cell .markdown}
#### Dataframe y limpieza de datos
:::

::: {#4b617018 .cell .code execution_count="23"}
``` python
df_porcentaje_religion = pd.read_excel('Datos/Religious_Composition_by_Country_2010-2050.xlsx',)
df_porcentaje_religion = df_porcentaje_religion[df_porcentaje_religion["Year"]==2010]
suicidios_2010 = df_suicidio_oms_clean[df_suicidio_oms_clean['Period'] == 2010]
suicidios_2010 = suicidios_2010[suicidios_2010['Dim1'] == "Both sexes"]
# Hacer merge de ambos dataframe segun Country(en df_suicidios) y Location(en df_porcentaje_religion)
suicidios_religion_2010 = suicidios_2010.merge(df_porcentaje_religion, left_on="Location", right_on="Country", how="left")
#Eliminar columnas innecesarias (row_number,level,Nation_fk,Year,Region,Country)
suicidios_religion_2010.drop(columns=['row_number','level','Nation_fk','Year','Region','Country','Unaffiliated',"All Religions","Dim1","Period","CodigoPais"], inplace=True)
suicidios_religion_2010.dropna(inplace=True)
#Hacemos merge con el dataframe de poblacion
suicidios_religion_2010 = suicidios_religion_2010.merge(df_population, on="Location", how="left")
#hacemos merge con el dataframe de porcentaje de creyentes
suicidios_religion_2010 = suicidios_religion_2010.merge(df_porcentaje_creyentes, on="Location", how="left")
#Arreglamos columnas
suicidios_religion_2010.rename(columns={"FactValueNumeric":"Suicides per 100K"}, inplace=True)
suicidios_religion_2010['Population'] = pd.to_numeric(suicidios_religion_2010['Population'].replace(',', '', regex=True), errors='coerce')
#Mostrar dataframe con random de 10 filas
suicidios_religion_2010.sample(15)
```

::: {.output .stream .stderr}
    /Users/mardrouilly/anaconda3/lib/python3.11/site-packages/openpyxl/worksheet/_read_only.py:79: UserWarning: Unknown extension is not supported and will be removed
      for idx, row in parser.parse():
:::

::: {.output .execute_result execution_count="23"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ParentLocation</th>
      <th>Location</th>
      <th>Suicides per 100K</th>
      <th>Christians</th>
      <th>Muslims</th>
      <th>Hindus</th>
      <th>Buddhists</th>
      <th>Folk Religions</th>
      <th>Other Religions</th>
      <th>Jews</th>
      <th>Population</th>
      <th>Religious %</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>119</th>
      <td>Europe</td>
      <td>Netherlands</td>
      <td>9.81</td>
      <td>8,410,000</td>
      <td>1,000,000</td>
      <td>80,000</td>
      <td>40,000</td>
      <td>30,000</td>
      <td>30,000</td>
      <td>30,000</td>
      <td>16574989.0</td>
      <td>66.00</td>
    </tr>
    <tr>
      <th>83</th>
      <td>Eastern Mediterranean</td>
      <td>Qatar</td>
      <td>8.23</td>
      <td>240,000</td>
      <td>1,190,000</td>
      <td>240,000</td>
      <td>50,000</td>
      <td>&lt;10,000</td>
      <td>10,000</td>
      <td>&lt;10,000</td>
      <td>1699435.0</td>
      <td>98.23</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Africa</td>
      <td>Burkina Faso</td>
      <td>8.03</td>
      <td>3,710,000</td>
      <td>10,150,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>2,530,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>15730977.0</td>
      <td>99.50</td>
    </tr>
    <tr>
      <th>113</th>
      <td>Europe</td>
      <td>Kyrgyzstan</td>
      <td>11.38</td>
      <td>610,000</td>
      <td>4,690,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>5418300.0</td>
      <td>95.00</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Africa</td>
      <td>Equatorial Guinea</td>
      <td>10.03</td>
      <td>620,000</td>
      <td>30,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>1313000.0</td>
      <td>96.56</td>
    </tr>
    <tr>
      <th>0</th>
      <td>Africa</td>
      <td>Angola</td>
      <td>6.97</td>
      <td>17,270,000</td>
      <td>40,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>790,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>18992708.0</td>
      <td>98.21</td>
    </tr>
    <tr>
      <th>55</th>
      <td>Americas</td>
      <td>Grenada</td>
      <td>0.94</td>
      <td>100,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>109553.0</td>
      <td>95.19</td>
    </tr>
    <tr>
      <th>150</th>
      <td>Western Pacific</td>
      <td>Philippines</td>
      <td>2.36</td>
      <td>86,370,000</td>
      <td>5,150,000</td>
      <td>&lt;10,000</td>
      <td>80,000</td>
      <td>1,430,000</td>
      <td>130,000</td>
      <td>&lt;10,000</td>
      <td>92337852.0</td>
      <td>99.07</td>
    </tr>
    <tr>
      <th>46</th>
      <td>Americas</td>
      <td>Brazil</td>
      <td>4.99</td>
      <td>173,300,000</td>
      <td>40,000</td>
      <td>&lt;10,000</td>
      <td>250,000</td>
      <td>5,540,000</td>
      <td>300,000</td>
      <td>110,000</td>
      <td>193252604.0</td>
      <td>91.50</td>
    </tr>
    <tr>
      <th>143</th>
      <td>Western Pacific</td>
      <td>Fiji</td>
      <td>9.64</td>
      <td>550,000</td>
      <td>50,000</td>
      <td>240,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>850700.0</td>
      <td>98.95</td>
    </tr>
    <tr>
      <th>101</th>
      <td>Europe</td>
      <td>Estonia</td>
      <td>18.79</td>
      <td>540,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>1340127.0</td>
      <td>30.97</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Africa</td>
      <td>Central African Republic</td>
      <td>15.75</td>
      <td>3,940,000</td>
      <td>370,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>40,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>4505945.0</td>
      <td>98.76</td>
    </tr>
    <tr>
      <th>115</th>
      <td>Europe</td>
      <td>Luxembourg</td>
      <td>12.01</td>
      <td>360,000</td>
      <td>10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>502066.0</td>
      <td>95.04</td>
    </tr>
    <tr>
      <th>107</th>
      <td>Europe</td>
      <td>Hungary</td>
      <td>25.52</td>
      <td>8,090,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>&lt;10,000</td>
      <td>10,000</td>
      <td>10014324.0</td>
      <td>72.84</td>
    </tr>
    <tr>
      <th>38</th>
      <td>Africa</td>
      <td>Uganda</td>
      <td>6.33</td>
      <td>28,980,000</td>
      <td>3,840,000</td>
      <td>100,000</td>
      <td>&lt;10,000</td>
      <td>290,000</td>
      <td>40,000</td>
      <td>&lt;10,000</td>
      <td>31784600.0</td>
      <td>99.57</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
#### Analisis de datos
:::

::: {.cell .markdown}
##### Paises mas religiosos vs menos religiosos
:::

::: {.cell .code execution_count="24"}
``` python
#Seleccionamos top 10 de paises mas religiosos
top_10_religiosos = suicidios_religion_2010.sort_values(by="Religious %", ascending=False).head(15)
#Seleccionamos top 10 de paises menos religiosos
top_10_no_religiosos = suicidios_religion_2010.sort_values(by="Religious %", ascending=True).head(15)
#Sacamos el promedio de suicidios por cada 100mil habitantes de ambos grupos
promedio_religiosos = top_10_religiosos["Suicides per 100K"].mean()
promedio_no_religiosos = top_10_no_religiosos["Suicides per 100K"].mean()

#Los comparamos en un grafico de barras
plt.figure(figsize=(20,5))
plt.subplot(1,2,1)
plt.title("Top 15 de paises mas religiosos")
sns.barplot(data=top_10_religiosos, x="Location", y="Suicides per 100K")
plt.xticks(rotation=90)
plt.axhline(promedio_religiosos, color="red")
plt.subplot(1,2,2)
plt.title("Top 15 de paises menos religiosos")
sns.barplot(data=top_10_no_religiosos, x="Location", y="Suicides per 100K")
plt.xticks(rotation=90)
plt.axhline(promedio_no_religiosos, color="red")
plt.legend(labels=["Promedio de suicidios"])
#Agregamos una descripcion que aclare que son datos de 2010
plt.figtext(0.5, 0.01, "2010", ha="center", fontsize=12, bbox={"facecolor":"orange", "alpha":0.5, "pad":5})
plt.show()

```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/f428a46512491505740fb72d1b6385b78e149228.png)
:::
:::

::: {.cell .markdown}
> #### Los paises menos religiosos tienen mayor promedio en su tasa de suicidios respecto a los mas religiosos
:::

::: {.cell .markdown}
#### Hay alguna religion que tienda a tener mas suicidios que otras?
:::

::: {.cell .code execution_count="25"}
``` python
#Ordenamos el dataframe por religion. Es decir en cada row, veremos cual es la religion predominante (Mayor numero respecto a la poblacion total)
#Para ello, agregaremos una columna('predominant') con la religion predominante por pais, siendo las opciones: Christians,Muslims,Hindus,Buddhists,Folk Religions,Other Religions, Jews 
religion_columns = ['Christians', 'Muslims', 'Hindus', 'Buddhists', 'Folk Religions', 'Other Religions', 'Jews']
religions_df = suicidios_religion_2010.copy()
for col in religion_columns:
    # Convertimos a numeros
    religions_df[col] = religions_df[col].replace('<', '', regex=True).replace(',', '', regex=True)
    religions_df[col] = pd.to_numeric(religions_df[col], errors='coerce')
religions_df['Predominant Religion'] = religions_df[religion_columns].idxmax(axis=1)
#Eliminamos todas las columnas que no sean necesarias: Christians,Musilms...etc
for religion in religion_columns:
    religions_df.drop(columns=[religion], inplace=True)

#Creamos un dataframe agrupado por 'Predominant Religion' y calculamos el promedio de suicidios 'Suicides per 100K'
grouped_df = religions_df.groupby('Predominant Religion').agg({'Population': 'sum', 'Suicides per 100K': 'mean'})

grouped_df = grouped_df.reset_index()
#Ajustamos el numero sucidies per 100k para que sea mas legible
grouped_df['Suicides per 100K'] = grouped_df['Suicides per 100K'].round(2)
```
:::

::: {.cell .code execution_count="26"}
``` python
#Creamos la columna 'Suicides per population' que es se calcula: (population * suicides per 100k) / 100000
grouped_df['Suicides per population'] = (grouped_df['Population'] * grouped_df['Suicides per 100K']) / 100000
grouped_df['Suicides per population'] = grouped_df['Suicides per population'].round(2)
grouped_df
```

::: {.output .execute_result execution_count="26"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Predominant Religion</th>
      <th>Population</th>
      <th>Suicides per 100K</th>
      <th>Suicides per population</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Buddhists</td>
      <td>2.354434e+08</td>
      <td>13.85</td>
      <td>32608.91</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Christians</td>
      <td>1.855450e+09</td>
      <td>12.02</td>
      <td>223025.07</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Folk Religions</td>
      <td>1.339725e+09</td>
      <td>10.24</td>
      <td>137187.82</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Hindus</td>
      <td>1.211433e+09</td>
      <td>10.36</td>
      <td>125504.43</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Jews</td>
      <td>7.623600e+06</td>
      <td>6.66</td>
      <td>507.73</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Muslims</td>
      <td>1.108498e+09</td>
      <td>6.38</td>
      <td>70722.16</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .code execution_count="27"}
``` python
g = sns.catplot(
    data=grouped_df, kind="bar",
    x="Predominant Religion", y="Suicides per 100K", hue="Suicides per population",
    palette="dark", alpha=.6, height=6
)
g.despine(left=True)
g.set_axis_labels("", "Suicides per 100k")
g.legend.set_title("Suicides per population")
plt.title("Suicides per 100k by Religion")
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/686f9d0882e419466c05fbb8f1bcddb75b91da5a.png)
:::
:::

::: {.cell .markdown}
> Podemos ver que los Budistas tienen una tasa de suicidios mas alta que
> el resto de las religiones cada 100.000 habitantes, seguido de los
> cristianos Si tomamos en cuenta la cantidad de personas que pertenecen
> a cada religion, podemos ver que los cristianos tienen una tasa de
> suicidios mas alta que el resto de las religiones, esto se debe a que
> hay muchas mas personas que pertenecen a esta religion en el mundo.
> Pero podemos ver un contraejemplo (de 2010) con los [1500
> millones](https://www.institutohalal.com/la-poblacion-musulmana-en-el-mundo/#:~:text=Una%20poblaci%C3%B3n%20en%20aumento%3A%20De,a%202200%20millones%20en%202030)
> de musulmanes con una tasa de suicdios de 6.5 cada 100.000 habitantes,
> que es menor a la de los [1.100
> millones](https://elpais.com/internacional/2013/03/13/actualidad/1363206070_914018.html#:~:text=En%201910%2C%20los%20cat%C3%B3licos%20eran,cat%C3%B3lica%20global%20del%20Pew%20Center.)
> Cristianos en el mundo, con una tasa de 12 cada 100.000 habitantes. Es
> decir en 2010, los musulmanes tenian una tasa de suicidios 50% menor a
> la de los cristianos. **Por lo que podemos afirmar que hay religiones
> que tienden a tener menos suicidios que otras.**
:::

::: {.cell .markdown}
#### Mapas
:::

::: {.cell .code execution_count="28"}
``` python
#Mapa con geopandas
world = gpd.read_file(gpd.datasets.get_path('naturalearth_lowres'))
merged = world.set_index('name').join(religions_df.set_index('Location'))
fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(10, 12))
merged.plot(column='Religious %', ax=ax1, legend=True)
ax1.set_title('Religious %(2010)')
merged.plot(column='Suicides per 100K', ax=ax2, legend=True)
ax2.set_title('Suicides per 100K(2010)')
plt.show()

```

::: {.output .stream .stderr}
    /var/folders/yr/1dwzyqt511jb113_wtkjnp640000gn/T/ipykernel_5111/3473983891.py:2: FutureWarning: The geopandas.dataset module is deprecated and will be removed in GeoPandas 1.0. You can get the original 'naturalearth_lowres' data from https://www.naturalearthdata.com/downloads/110m-cultural-vectors/.
      world = gpd.read_file(gpd.datasets.get_path('naturalearth_lowres'))
:::

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/3e3afbe667c25f7e49728f5c338ac6d6933ea5e3.png)
:::
:::

::: {.cell .markdown}
#### Correlaciones
:::

::: {.cell .code execution_count="29"}
``` python
# Graficos de correlacion df: religions_df
plt.figure(figsize=(15,5))
plt.subplot(1,2,1)
plt.title("Suicides per 100K vs Religious %")
sns.scatterplot(data=religions_df, x="Religious %", y="Suicides per 100K")
#Agregamos linea de regresion
sns.regplot(data=religions_df, x="Religious %", y="Suicides per 100K", scatter=False, color="red", label="Regresion lineal")
plt.figtext(0.5, 0.01, "Datos de 2010", ha="center", fontsize=12, bbox={"facecolor":"orange", "alpha":0.5, "pad":5})
plt.subplot(1,2,2)
plt.title("Suicides per 100K vs Predominant Religion")
sns.boxplot(data=religions_df, x="Predominant Religion", y="Suicides per 100K")
plt.xticks(rotation=90)
#Mapa de calor de correlacion entre suicidies per 100k y religious %

plt.show()

```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/9c9396852448d28d1a097fc55302a823871914ca.png)
:::
:::

::: {.cell .markdown}
#### Los paises con mas suicidios son los mas religiosos?
:::

::: {.cell .code execution_count="30"}
``` python
#Buscar el pais con mayor cantidad de suicidios de cada region (columna:ParentLocation)
suicidios_region_mas = religions_df.groupby("ParentLocation").agg({"Suicides per 100K":"max"})
suicidios_region_mas = suicidios_region_mas.reset_index()
suicidios_region_mas = suicidios_region_mas.merge(religions_df, on=["ParentLocation","Suicides per 100K"])
suicidios_region_mas = suicidios_region_mas[["ParentLocation","Location","Suicides per 100K","Religious %","Predominant Religion"]]
suicidios_region_mas.rename(columns={"ParentLocation":"Region","Location":"Country","Suicides per 100K":"Suicides per 100K (max)"}, inplace=True)
suicidios_region_mas.sort_values(by="Suicides per 100K (max)", ascending=False, inplace=True)
suicidios_region_mas
```

::: {.output .execute_result execution_count="30"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Region</th>
      <th>Country</th>
      <th>Suicides per 100K (max)</th>
      <th>Religious %</th>
      <th>Predominant Religion</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Africa</td>
      <td>Lesotho</td>
      <td>65.43</td>
      <td>99.72</td>
      <td>Christians</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Europe</td>
      <td>Lithuania</td>
      <td>37.24</td>
      <td>84.79</td>
      <td>Christians</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Americas</td>
      <td>Guyana</td>
      <td>33.31</td>
      <td>95.00</td>
      <td>Christians</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Western Pacific</td>
      <td>Kiribati</td>
      <td>30.70</td>
      <td>99.00</td>
      <td>Christians</td>
    </tr>
    <tr>
      <th>4</th>
      <td>South-East Asia</td>
      <td>Sri Lanka</td>
      <td>21.91</td>
      <td>99.95</td>
      <td>Buddhists</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Eastern Mediterranean</td>
      <td>Morocco</td>
      <td>9.15</td>
      <td>100.00</td>
      <td>Muslims</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .code execution_count="31"}
``` python
suicidios_region_menos = religions_df.groupby("ParentLocation").agg({"Suicides per 100K":"min"})
suicidios_region_menos = suicidios_region_menos.reset_index()
suicidios_region_menos = suicidios_region_menos.merge(religions_df, on=["ParentLocation","Suicides per 100K"])
suicidios_region_menos = suicidios_region_menos[["ParentLocation","Location","Suicides per 100K","Religious %","Predominant Religion"]]
suicidios_region_menos.rename(columns={"ParentLocation":"Region","Location":"Country","Suicides per 100K":"Suicides per 100K (min)"}, inplace=True)
suicidios_region_menos.sort_values(by="Suicides per 100K (min)", ascending=True, inplace=True)
suicidios_region_menos
```

::: {.output .execute_result execution_count="31"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Region</th>
      <th>Country</th>
      <th>Suicides per 100K (min)</th>
      <th>Religious %</th>
      <th>Predominant Religion</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>Americas</td>
      <td>Antigua and Barbuda</td>
      <td>0.16</td>
      <td>94.10</td>
      <td>Christians</td>
    </tr>
    <tr>
      <th>0</th>
      <td>Africa</td>
      <td>Sao Tome and Principe</td>
      <td>1.45</td>
      <td>98.76</td>
      <td>Christians</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Eastern Mediterranean</td>
      <td>Jordan</td>
      <td>1.52</td>
      <td>100.00</td>
      <td>Muslims</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Western Pacific</td>
      <td>Philippines</td>
      <td>2.36</td>
      <td>99.07</td>
      <td>Christians</td>
    </tr>
    <tr>
      <th>4</th>
      <td>South-East Asia</td>
      <td>Indonesia</td>
      <td>2.64</td>
      <td>99.25</td>
      <td>Muslims</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Europe</td>
      <td>Greece</td>
      <td>3.48</td>
      <td>97.39</td>
      <td>Christians</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .code execution_count="32"}
``` python
#Graficar suicidios_region_menos y suicidios_region_mas
plt.figure(figsize=(15,5))
plt.subplot(1,2,1)
plt.title("Suicides per 100K (max) por region")
sns.barplot(data=suicidios_region_mas, x="Region", y="Suicides per 100K (max)", hue="Country")
plt.xticks(rotation=90)
plt.subplot(1,2,2)
plt.title("Suicides per 100K (min) por region")
sns.barplot(data=suicidios_region_menos, x="Region", y="Suicides per 100K (min)", hue="Country")
plt.xticks(rotation=90)
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/e8f9606b81dbd554446bca327da4f379a33378dd.png)
:::
:::

::: {.cell .markdown}
> Esto indica que los paises con mas suicidios y menos no tienen una
> relacion directa con la cantidad de personas que pertenecen a cada
> religion. Sin embargo, al reves tiene una correlacion negativa, ya que
> los paises que mas suicidios tienen son los menos religiosos(Como se
> mostro al principio).
:::

::: {.cell .markdown}
##### Extremos de la distribucion de datos
:::

::: {.cell .code execution_count="33"}
``` python
#buscar el pais con mas sucidios por cada religion
suicidios_religion_mas = religions_df.groupby("Predominant Religion").agg({"Suicides per 100K":"max"})
suicidios_religion_mas = suicidios_religion_mas.reset_index()
suicidios_religion_mas = suicidios_religion_mas.merge(religions_df, on=["Predominant Religion","Suicides per 100K"])
suicidios_religion_mas = suicidios_religion_mas[["Predominant Religion","Location","Suicides per 100K","Religious %"]]
suicidios_religion_mas.rename(columns={"Location":"Country","Suicides per 100K":"Suicides per 100K"}, inplace=True)
suicidios_religion_mas.sort_values(by="Suicides per 100K", ascending=False, inplace=True)
#buscar el pais con menos sucidios por cada religion
suicidios_religion_menos = religions_df.groupby("Predominant Religion").agg({"Suicides per 100K":"min"})
suicidios_religion_menos = suicidios_religion_menos.reset_index()
suicidios_religion_menos = suicidios_religion_menos.merge(religions_df, on=["Predominant Religion","Suicides per 100K"])
suicidios_religion_menos = suicidios_religion_menos[["Predominant Religion","Location","Suicides per 100K","Religious %"]]
suicidios_religion_menos.rename(columns={"Location":"Country","Suicides per 100K":"Suicides per 100K"}, inplace=True)
suicidios_religion_menos.sort_values(by="Suicides per 100K", ascending=True, inplace=True)
#Agregar rows de suicidios_religion_mas y suicidios_religion_menos a correlacion_religion
combined_df = pd.concat([suicidios_religion_mas, suicidios_religion_menos], ignore_index=True)
combined_df = combined_df.sort_values(by="Suicides per 100K", ascending=False)
combined_df
```

::: {.output .execute_result execution_count="33"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Predominant Religion</th>
      <th>Country</th>
      <th>Suicides per 100K</th>
      <th>Religious %</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Christians</td>
      <td>Lesotho</td>
      <td>65.43</td>
      <td>99.72</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Muslims</td>
      <td>Kazakhstan</td>
      <td>29.94</td>
      <td>88.48</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Buddhists</td>
      <td>Japan</td>
      <td>24.11</td>
      <td>90.50</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Hindus</td>
      <td>India</td>
      <td>14.64</td>
      <td>99.69</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Folk Religions</td>
      <td>China</td>
      <td>10.24</td>
      <td>67.50</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Folk Religions</td>
      <td>China</td>
      <td>10.24</td>
      <td>67.50</td>
    </tr>
    <tr>
      <th>10</th>
      <td>Hindus</td>
      <td>Mauritius</td>
      <td>7.76</td>
      <td>99.29</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Jews</td>
      <td>Israel</td>
      <td>6.66</td>
      <td>95.50</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Jews</td>
      <td>Israel</td>
      <td>6.66</td>
      <td>95.50</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Buddhists</td>
      <td>Bhutan</td>
      <td>4.23</td>
      <td>99.97</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Muslims</td>
      <td>Jordan</td>
      <td>1.52</td>
      <td>100.00</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Christians</td>
      <td>Antigua and Barbuda</td>
      <td>0.16</td>
      <td>94.10</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .code execution_count="34"}
``` python
#Graficar correlacion de combined_df (Suicides per 100K y Religious %)
plt.figure(figsize=(15,5))
plt.subplot(1,2,1)
plt.title("Suicides per 100K vs Religious %")
sns.scatterplot(data=combined_df, x="Religious %", y="Suicides per 100K")
#Agregamos nombres de los paises
for i in range(len(combined_df)):
    plt.text(x=combined_df["Religious %"][i], y=combined_df["Suicides per 100K"][i], s=combined_df["Country"][i])
#Agregamos linea de regresion
sns.regplot(data=combined_df, x="Religious %", y="Suicides per 100K", scatter=False, color="red", label="Regresion lineal")
plt.figtext(0.5, 0.01, "Datos de 2010", ha="center", fontsize=12, bbox={"facecolor":"orange", "alpha":0.5, "pad":5})
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/a29665f48e1019e2dd9a2f11b9b70ef1d9d32f95.png)
:::
:::

::: {.cell .markdown}
> Con esto podemos ver que en los extremos de la distribucion de datos,
> No parece haber una relacion clara entre la cantidad de suicidios y la
> cantidad de personas que pertenecen a cada religion. Es decir en el
> pais con mas y menos suicidios de cada religion, no parecen ser los
> paises mas o menos religiosos. Al contrario de como vimos al
> principio, donde los 15 paises menos religiosos, eran los que tenian
> mas suciidios y no viceversa. Cuando nos vamos a los extremos de los
> datos, no se ve una correlacion clara, pero si nos vamos a la muestra
> completa, si se ve una tendencia clara de que los paises menos
> religiosos tienen mas suicidios que los mas religiosos.
:::

::: {.cell .markdown}
# 5. ¿Cómo influye el acceso al internet en la tasa de suicidios en diferentes grupos demográficos? {#5-cómo-influye-el-acceso-al-internet-en-la-tasa-de-suicidios-en-diferentes-grupos-demográficos}
:::

::: {.cell .code execution_count="35"}
``` python
response = rq.get('https://en.wikipedia.org/wiki/List_of_countries_by_number_of_Internet_users')
soup = bs(response.content)
table = soup.find_all('table')[5]

df = pd.DataFrame(columns = ['País','Region','Usuarios de internet','% Usuarios por pais'])

# iterar sobre cada fila ('tr') para completar la información
for row in table.find_all('tr')[1::]:
    cols = row.find_all("td")
    cols = [col.text.strip() for col in cols]
    puesto = cols[0]
    pais = cols[1]
    usuarios = cols[3]
    porcentajes = cols[4]
    new_row = pd.DataFrame({'País': puesto, 'Region': pais, 'Usuarios de internet': usuarios,'% Usuarios por pais':porcentajes}, index=['country'])
    df = pd.concat([df, new_row], ignore_index=True)

usur_por_pais=df

#ahora para ayudar a una mejor comparacion buscaremos agrregar una columna que nos de el porcentaje de suicidios por pais para esto extraeremos datos de internet para hallar el numero de ciudadanos por pais en el año 2021 año en el que no estamos moviendo
response = rq.get('https://www.worldometers.info/world-population/population-by-country/')
soup = bs(response.content)
table = soup.find_all('table')[0]

df = pd.DataFrame(columns = ['País','Nro Habitantes'])

# iterar sobre cada fila ('tr') para completar la información
for row in table.find_all('tr')[1::]:
    cols = row.find_all("td")
    cols = [col.text.strip() for col in cols]
    Países = cols[1]
    Población = cols[2]
    new_row = pd.DataFrame({'País': Países, 'Nro Habitantes':Población }, index=['country'])
    df = pd.concat([df, new_row], ignore_index=True)

#volvemos "Nro Habitantes" tipo entero
#df['Nro Habitantes'] = df['Nro Habitantes'].str.replace('.', '').astype(int)
df['Nro Habitantes'] = pd.to_numeric(df['Nro Habitantes'].str.replace(',', ''), errors='coerce')

#pasamos los datos de usur_por_pais a tipo numerico 
usur_por_pais['Usuarios de internet'] = usur_por_pais['Usuarios de internet'].replace(',', '', regex=True).astype(int)
usur_por_pais['% Usuarios por pais'] = usur_por_pais['% Usuarios por pais'].str.rstrip('%').astype(float)
usur_por_pais= usur_por_pais.merge(df,on="País")
usur_por_pais = usur_por_pais.sort_values(by='Nro Habitantes', ascending=False)
usur_por_pais
```

::: {.output .execute_result execution_count="35"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>País</th>
      <th>Region</th>
      <th>Usuarios de internet</th>
      <th>% Usuarios por pais</th>
      <th>Nro Habitantes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>India</td>
      <td>Southern Asia</td>
      <td>881250000</td>
      <td>62.6</td>
      <td>1428627663</td>
    </tr>
    <tr>
      <th>0</th>
      <td>China</td>
      <td>Eastern Asia</td>
      <td>1089140000</td>
      <td>76.4</td>
      <td>1425671352</td>
    </tr>
    <tr>
      <th>2</th>
      <td>United States</td>
      <td>Northern America</td>
      <td>311300000</td>
      <td>92.4</td>
      <td>339996563</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Indonesia</td>
      <td>South-eastern Asia</td>
      <td>215626156</td>
      <td>78.8</td>
      <td>277534122</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Pakistan</td>
      <td>Southern Asia</td>
      <td>130000000</td>
      <td>60.8</td>
      <td>240485658</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>194</th>
      <td>Nauru</td>
      <td>Micronesia</td>
      <td>6475</td>
      <td>51.8</td>
      <td>12780</td>
    </tr>
    <tr>
      <th>195</th>
      <td>Tuvalu</td>
      <td>Polynesia</td>
      <td>5520</td>
      <td>49.3</td>
      <td>11396</td>
    </tr>
    <tr>
      <th>197</th>
      <td>Montserrat</td>
      <td>Caribbean</td>
      <td>2833</td>
      <td>64.1</td>
      <td>4386</td>
    </tr>
    <tr>
      <th>196</th>
      <td>Falkland Islands</td>
      <td>South America</td>
      <td>2881</td>
      <td>76.5</td>
      <td>3791</td>
    </tr>
    <tr>
      <th>198</th>
      <td>Niue</td>
      <td>Polynesia</td>
      <td>1034</td>
      <td>53.4</td>
      <td>1935</td>
    </tr>
  </tbody>
</table>
<p>199 rows × 5 columns</p>
</div>
```
:::
:::

::: {.cell .code execution_count="36"}
``` python
suicidios_pais=df_suicidio_oms_clean[df_suicidio_oms_clean['Dim1']=='Both sexes'].reset_index(drop=True).drop(columns=['CodigoPais','ParentLocation','Dim1','Period'],axis=1)
suicidios_pais=suicidios_pais.groupby('Location').mean().reset_index()
suicidios_pais=suicidios_pais.rename(columns={'Location':'País','FactValueNumeric':'Suicidios'}) 
suicidios_pais=suicidios_pais.merge(usur_por_pais,on='País')

#ahora creamos una nueva columna para el porcentaje de suicidios por pais
suicidios_pais['% Suicidios por Nro. Habs.'] =(suicidios_pais['Suicidios'] / suicidios_pais['Nro Habitantes']) * 100 
#suicidios_pais.drop(['Suicidios', 'Nro Habitantes'], axis=1, inplace=True)
suicidios_pais#[suicidios_pais['País']=='China']

suicidios_pais = suicidios_pais.sort_values(by='Suicidios', ascending=False).reset_index(drop=True)
suicidios_pais
```

::: {.output .execute_result execution_count="36"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>País</th>
      <th>Suicidios</th>
      <th>Region</th>
      <th>Usuarios de internet</th>
      <th>% Usuarios por pais</th>
      <th>Nro Habitantes</th>
      <th>% Suicidios por Nro. Habs.</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Lesotho</td>
      <td>59.5735</td>
      <td>Southern Africa</td>
      <td>665312</td>
      <td>29.2</td>
      <td>2330318</td>
      <td>0.002556</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Eswatini</td>
      <td>41.0140</td>
      <td>Southern Africa</td>
      <td>414278</td>
      <td>34.7</td>
      <td>1210822</td>
      <td>0.003387</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Lithuania</td>
      <td>37.9765</td>
      <td>Northern Europe</td>
      <td>2243448</td>
      <td>80.5</td>
      <td>2718352</td>
      <td>0.001397</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Guyana</td>
      <td>34.5695</td>
      <td>South America</td>
      <td>290375</td>
      <td>36.1</td>
      <td>813834</td>
      <td>0.004248</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Belarus</td>
      <td>34.0420</td>
      <td>Eastern Europe</td>
      <td>7048231</td>
      <td>73.6</td>
      <td>9498238</td>
      <td>0.000358</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>155</th>
      <td>Jamaica</td>
      <td>1.9970</td>
      <td>Caribbean</td>
      <td>1409888</td>
      <td>49.9</td>
      <td>2825544</td>
      <td>0.000071</td>
    </tr>
    <tr>
      <th>156</th>
      <td>Jordan</td>
      <td>1.7900</td>
      <td>Western Asia</td>
      <td>6480202</td>
      <td>58.1</td>
      <td>11337052</td>
      <td>0.000016</td>
    </tr>
    <tr>
      <th>157</th>
      <td>Grenada</td>
      <td>1.7610</td>
      <td>Caribbean</td>
      <td>63692</td>
      <td>51.1</td>
      <td>126183</td>
      <td>0.001396</td>
    </tr>
    <tr>
      <th>158</th>
      <td>Barbados</td>
      <td>1.1360</td>
      <td>Caribbean</td>
      <td>233604</td>
      <td>83.1</td>
      <td>281995</td>
      <td>0.000403</td>
    </tr>
    <tr>
      <th>159</th>
      <td>Antigua and Barbuda</td>
      <td>0.6490</td>
      <td>Caribbean</td>
      <td>77529</td>
      <td>83.2</td>
      <td>94298</td>
      <td>0.000688</td>
    </tr>
  </tbody>
</table>
<p>160 rows × 7 columns</p>
</div>
```
:::
:::

::: {.cell .code execution_count="37"}
``` python
#Graficamos los Datos
plt.figure(figsize=(10, 5))
sns.scatterplot(y='% Usuarios por pais', x='Suicidios', data=suicidios_pais)
sns.regplot(y='% Usuarios por pais', x='Suicidios', data=suicidios_pais)
plt.title('% Usuarios por pais vs suicidos por 100k')
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/6ba989f32b6e7604eed0f636ae89528773cacd54.png)
:::
:::

::: {.cell .code execution_count="38"}
``` python
#Calculamos la correlacion genral entre Usuarios de internet y Suicidios
datos_de_interes = suicidios_pais[['% Usuarios por pais','Suicidios']]
correlacion = datos_de_interes.corr().iloc[0:1]
print(f'Correlacion por pearson de Usuarios de internet y Suicidios {correlacion}')
```

::: {.output .stream .stdout}
    Correlacion por pearson de Usuarios de internet y Suicidios                      % Usuarios por pais  Suicidios
    % Usuarios por pais                  1.0   0.093839
:::
:::

::: {.cell .markdown}
Al calcular la correlacion de Person para cada valor nos daremos cuenta
que existe una correlacion practicamente nula en ambos casos por ende
diremos que no hay una correlacion directa A NIVEL GLOBAL entre los
Usuarios por pais y los suicidios por numero de habitantes.
:::

::: {.cell .markdown}
Ahora si nos fijamos especifiamente en una reguion en espeifica como
EEUU en el año 2021 a partir de estos datos podremos ver:
:::

::: {.cell .code execution_count="39"}
``` python
#datos de acceso a internet
internet_acess = pd.read_excel('Datos/data/statistic_id184691_internet-access-in-the-united-states-november-2021-by-state.xlsx',skiprows= 4, sheet_name='Data' )
internet_acess = internet_acess.rename(columns={'Unnamed: 1':'STATE','Unnamed: 2':'% INTERNET ACCESS'})[['STATE','% INTERNET ACCESS']]

#datos de suicidios por estado
suicides_per_state = pd.read_csv('Datos/data/data-table.csv')
suicides_per_state = suicides_per_state[suicides_per_state['YEAR']==2019].reset_index(drop= True)[['STATE','RATE','DEATHS']]

#convertimos los el codigo de estado al estado correspondiente
estados = {
    'AL': 'Alabama', 'AK': 'Alaska', 'AZ': 'Arizona', 'AR': 'Arkansas', 'CA': 'California',
    'CO': 'Colorado', 'CT': 'Connecticut', 'DE': 'Delaware', 'FL': 'Florida', 'GA': 'Georgia',
    'HI': 'Hawaii', 'ID': 'Idaho', 'IL': 'Illinois', 'IN': 'Indiana', 'IA': 'Iowa', 'KS': 'Kansas',
    'KY': 'Kentucky', 'LA': 'Louisiana', 'ME': 'Maine', 'MD': 'Maryland', 'MA': 'Massachusetts',
    'MI': 'Michigan', 'MN': 'Minnesota', 'MS': 'Mississippi', 'MO': 'Missouri', 'MT': 'Montana',
    'NE': 'Nebraska', 'NV': 'Nevada', 'NH': 'New Hampshire', 'NJ': 'New Jersey', 'NM': 'New Mexico',
    'NY': 'New York', 'NC': 'North Carolina', 'ND': 'North Dakota', 'OH': 'Ohio', 'OK': 'Oklahoma',
    'OR': 'Oregon', 'PA': 'Pennsylvania', 'RI': 'Rhode Island', 'SC': 'South Carolina', 'SD': 'South Dakota',
    'TN': 'Tennessee', 'TX': 'Texas', 'UT': 'Utah', 'VT': 'Vermont', 'VA': 'Virginia', 'WA': 'Washington',
    'WV': 'West Virginia', 'WI': 'Wisconsin', 'WY': 'Wyoming'
}

suicides_per_state['STATE'] = suicides_per_state['STATE'].map(estados)

#Datos unifiados
Data = suicides_per_state.merge(internet_acess,on='STATE')
#Data.dtypes

#Pasamos los datos a tipo numerico
Data['DEATHS']=Data['DEATHS'].astype(float)
Data.dtypes
```

::: {.output .execute_result execution_count="39"}
    STATE                 object
    RATE                 float64
    DEATHS               float64
    % INTERNET ACCESS    float64
    dtype: object
:::
:::

::: {.cell .code execution_count="40"}
``` python
plt.figure(figsize=(12, 6))
sns.barplot(x='STATE', y='RATE', data=Data)
media_rate = np.mean(Data['RATE'])
plt.axhline(y=media_rate, color='red', linestyle='--', label=f'Media: {media_rate:.2f}')
plt.legend()
plt.title('STATE vs RATE OF SUICIDES')
plt.xticks(rotation=90)
plt.xlabel('STATE')
plt.ylabel('RATE')
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/5a41fae675f79bbdc50706ef745e2b7f79d1b0d1.png)
:::
:::

::: {.cell .code execution_count="41"}
``` python
# Gráfico STATE vs % INTERNET ACCESS
plt.figure(figsize=(12, 6))
sns.barplot(x='STATE', y='% INTERNET ACCESS', data=Data)
plt.title('STATE vs % INTERNET ACCESS')
plt.xticks(rotation=90)
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/4020a830f0cb8b7d12764430adf5aff50c1117ea.png)
:::
:::

::: {.cell .markdown}
##### Correlaciones {#correlaciones}

Ahora busquemos una correlacion entre los suicidios por habitantes y el
% acceso a internet en los datos de EEUU.
:::

::: {.cell .code execution_count="42"}
``` python
plt.figure(figsize=(8, 6))
sns.scatterplot(x='% INTERNET ACCESS', y='RATE', data=Data)
sns.regplot(x='% INTERNET ACCESS', y='RATE', data=Data)
plt.title('% INTERNET ACCESS vs SUICIDIOS POR HABS.')
plt.xlabel('% INTERNET ACCESS')
plt.ylabel('SUICIDIOS POR HABS.')
plt.show() 

correlacion = Data['% INTERNET ACCESS'].corr(Data['RATE'])
print(f"Correlación entre '% INTERNET ACCESS' y 'RATE' es: {correlacion}")

correlacion = Data['% INTERNET ACCESS'].corr(Data['DEATHS'])
print(f"La correlación entre '% INTERNET ACCESS' y 'DEATHS' es: {correlacion}")
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/81c69fbb1d06f32530da42834a8c66b1e1017634.png)
:::

::: {.output .stream .stdout}
    Correlación entre '% INTERNET ACCESS' y 'RATE' es: 0.0586523601686701
    La correlación entre '% INTERNET ACCESS' y 'DEATHS' es: -0.2762428321044948
:::
:::

::: {.cell .markdown}
Como se pyede ver en EEUU la correlacion entre los Suicidios por Tot.
habitantes y por Suicidios tienen muy poca correlacion en ambos casos,
por lo que no se puede notar una influencia clara entre el % aceso a
internet y los suicidios por habs.
:::

::: {.cell .markdown}
# 6. ¿Se relaciona la tasa de suicidios con la esperanza de vida de los países? {#6-se-relaciona-la-tasa-de-suicidios-con-la-esperanza-de-vida-de-los-países}
:::

::: {.cell .code execution_count="43"}
``` python
life_expectancy = pd.read_csv('Datos/data/life_exp.csv')
#Dejar solo la columna de 2019
life_expectancy = life_expectancy[["Country Name","2019"]]
#Renombrar columnas
life_expectancy.rename(columns={"Country Name":"Location","2019":"Life expectancy"}, inplace=True)
merged_df = pd.merge(suicidios2019, life_expectancy, on="Location")
merged_df = merged_df[["Location","Life expectancy","FactValueNumeric"]]
merged_df.rename(columns={"FactValueNumeric":"Suicides per 100K"}, inplace=True)
merged_df["Life expectancy"] = pd.to_numeric(merged_df["Life expectancy"], errors='coerce')
merged_df["Suicides per 100K"] = pd.to_numeric(merged_df["Suicides per 100K"], errors='coerce')
merged_df.dropna(inplace=True)
merged_df
```

::: {.output .execute_result execution_count="43"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Location</th>
      <th>Life expectancy</th>
      <th>Suicides per 100K</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Angola</td>
      <td>62.448</td>
      <td>6.08</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Burundi</td>
      <td>62.351</td>
      <td>6.24</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Benin</td>
      <td>60.454</td>
      <td>7.81</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Burkina Faso</td>
      <td>60.039</td>
      <td>7.48</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Botswana</td>
      <td>65.464</td>
      <td>16.05</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>154</th>
      <td>Solomon Islands</td>
      <td>70.382</td>
      <td>14.67</td>
    </tr>
    <tr>
      <th>155</th>
      <td>Tonga</td>
      <td>70.871</td>
      <td>3.82</td>
    </tr>
    <tr>
      <th>156</th>
      <td>Viet Nam</td>
      <td>74.093</td>
      <td>7.51</td>
    </tr>
    <tr>
      <th>157</th>
      <td>Vanuatu</td>
      <td>69.877</td>
      <td>18.03</td>
    </tr>
    <tr>
      <th>158</th>
      <td>Samoa</td>
      <td>72.157</td>
      <td>12.55</td>
    </tr>
  </tbody>
</table>
<p>159 rows × 3 columns</p>
</div>
```
:::
:::

::: {.cell .code execution_count="44"}
``` python
plt.figure(figsize=(15,5))
plt.subplot(1,2,1)
plt.title("Suicides per 100K vs Life expectancy")
sns.scatterplot(data=merged_df, x="Life expectancy", y="Suicides per 100K")
sns.regplot(data=merged_df, x="Life expectancy", y="Suicides per 100K", scatter=False, color="red", label="Regresion lineal")
plt.figtext(0.5, 0.01, "Datos de 2019", ha="center", fontsize=12, bbox={"facecolor":"orange", "alpha":0.5, "pad":5})
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/24a1cf9473ab776148315eed8dc20d08cdbf2158.png)
:::
:::

::: {.cell .code execution_count="45"}
``` python
correlation_df = merged_df[['Life expectancy', 'Suicides per 100K']]
correlation_matrix = correlation_df.corr()
plt.figure(figsize=(10,5))
sns.heatmap(correlation_matrix, annot=True)
plt.title("Correlacion entre life expectancy y suicides per 100k")
plt.show()
```

::: {.output .display_data}
![](vertopal_36467573d3e44472898f38feaa28002a/4c269484419da7414e222d0ac1a2f527cc10f6ba.png)
:::
:::

::: {.cell .markdown}
Podemos decir que aunque existe una relación mínima entre la esperanza
de vida y las tasas de suicidio en los países, el tamaño del efecto es
apenas significativo. Además, se destaca que la esperanza de vida, en sí
misma, no explica sustancialmente la variación en las tasas de suicidio
entre naciones. Este hallazgo sugiere que, si bien hay una conexión
numérica, la esperanza de vida no sirve como un predictor robusto por sí
solo para explicar las disparidades observadas en las tasas de suicidio
entre distintos países. Es probable que otros factores, no capturados
por la variable de esperanza de vida, contribuyan de manera
significativa a la variabilidad en las tasas de suicidio.
:::
