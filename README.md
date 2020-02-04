```python
import turicreate
```

## SFrame from Serbia.csv
Colected data from every match of the Asobal season 19/20 (first round)
Every "Serbia" and "fake pivot cross"


```python
sf = turicreate.SFrame.read_csv('Serbia.csv')
```


<pre>Finished parsing file /media/ruben/7BC1C6120D3C85FF/Machine Learning Foundations A Case Study Approach/Experimentos/Tesis/Serbia.csv</pre>



<pre>Parsing completed. Parsed 100 lines in 0.043132 secs.</pre>


    ------------------------------------------------------
    Inferred types from first 100 line(s) of file as 
    column_type_hints=[str,int,int,str,str,str,str,str,str]
    If parsing fails due to incorrect types, you can correct
    the inferred type list above and pass it to read_csv in
    the column_type_hints argument
    ------------------------------------------------------



<pre>Read 329 lines. Lines per second: 10061.5</pre>



<pre>Finished parsing file /media/ruben/7BC1C6120D3C85FF/Machine Learning Foundations A Case Study Approach/Experimentos/Tesis/Serbia.csv</pre>



<pre>Parsing completed. Parsed 329 lines in 0.033191 secs.</pre>



```python
sf
```




<div style="max-height:1000px;max-width:1500px;overflow:auto;"><table frame="box" rules="cols">
    <tr>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Nombre</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Posicion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Duracion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Accion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Decision</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Defensa</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Oposicion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Protagonista</th>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2508040</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2720</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">BID</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2581520</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">5480</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">GUA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (2)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2685040</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">6080</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">GUA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (3)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">921560</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">7960</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (1)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">992720</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">7280</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (2)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1111480</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">6880</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (3)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">3507040</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">6200</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (4)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">3766880</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">9320</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (4)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">858960</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">7400</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">SIN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (5)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1302240</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">10200</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">SIN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
    </tr>
</table>
<table frame="box" rules="cols">
    <tr>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Resultado</th>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Gol</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Gol</td>
    </tr>
</table>
[329 rows x 9 columns]<br/>Note: Only the head of the SFrame is printed.<br/>You can use print_rows(num_rows=m, num_columns=n) to print more rows and columns.
</div>




```python
sf.groupby('Protagonista',operations={'count':turicreate.aggregate.COUNT()}).sort('count',ascending=False)
```




<div style="max-height:1000px;max-width:1500px;overflow:auto;"><table frame="box" rules="cols">
    <tr>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Protagonista</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">count</th>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">55</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">BEN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">40</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">40</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">CQN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">32</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">BAR</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">27</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">25</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">BID</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">22</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">LOG</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">20</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">GRA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">16</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">GUA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">12</td>
    </tr>
</table>
[16 rows x 2 columns]<br/>Note: Only the head of the SFrame is printed.<br/>You can use print_rows(num_rows=m, num_columns=n) to print more rows and columns.
</div>




```python
Serbia_ANA = sf[sf['Protagonista']=='ANA']
```


```python
Serbia_ANA
```




<div style="max-height:1000px;max-width:1500px;overflow:auto;"><table frame="box" rules="cols">
    <tr>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Nombre</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Posicion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Duracion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Accion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Decision</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Defensa</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Oposicion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Protagonista</th>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2508040</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2720</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">BID</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (9)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1557320</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">9280</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">GUA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (8)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">570160</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">7920</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">GUA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (14)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1995760</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">8800</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">LOG</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (28)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">952260</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">9580</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">SIN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (19)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1672340</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">8320</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">SIN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (20)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1732600</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">40140</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">SIN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (21)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1943380</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">8380</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">SIN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (35)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">196920</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">11000</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">BEN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (36)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">579640</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">10320</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">BEN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
</table>
<table frame="box" rules="cols">
    <tr>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Resultado</th>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Gol</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Gol</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Gol</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Gol</td>
    </tr>
</table>
[? rows x 9 columns]<br/>Note: Only the head of the SFrame is printed. This SFrame is lazily evaluated.<br/>You can use sf.materialize() to force materialization.
</div>




```python
serbia_training_set, serbia_test_set = sf.random_split(.8)
```


```python
resultado_model = turicreate.logistic_classifier.create(serbia_training_set,target='Resultado', features=['Protagonista','Defensa','Accion'], validation_set=serbia_test_set)
```


<pre>Logistic regression:</pre>



<pre>--------------------------------------------------------</pre>



<pre>Number of examples          : 269</pre>



<pre>Number of classes           : 3</pre>



<pre>Number of feature columns   : 3</pre>



<pre>Number of unpacked features : 3</pre>



<pre>Number of coefficients      : 64</pre>



<pre>Starting Newton Method</pre>



<pre>--------------------------------------------------------</pre>



<pre>+-----------+----------+--------------+-------------------+---------------------+</pre>



<pre>| Iteration | Passes   | Elapsed Time | Training Accuracy | Validation Accuracy |</pre>



<pre>+-----------+----------+--------------+-------------------+---------------------+</pre>



<pre>| 1         | 2        | 1.001851     | 0.524164          | 0.350000            |</pre>



<pre>| 2         | 3        | 1.033570     | 0.505576          | 0.366667            |</pre>



<pre>| 3         | 4        | 1.034579     | 0.505576          | 0.366667            |</pre>



<pre>| 4         | 5        | 1.035520     | 0.505576          | 0.366667            |</pre>



<pre>| 5         | 6        | 1.036451     | 0.505576          | 0.366667            |</pre>



<pre>| 7         | 8        | 1.040719     | 0.505576          | 0.366667            |</pre>



<pre>+-----------+----------+--------------+-------------------+---------------------+</pre>



<pre>SUCCESS: Optimal solution found.</pre>



<pre></pre>



```python
resultado_model.summary()
```

    Class                          : LogisticClassifier
    
    Schema
    ------
    Number of coefficients         : 64
    Number of examples             : 269
    Number of classes              : 3
    Number of feature columns      : 3
    Number of unpacked features    : 3
    
    Hyperparameters
    ---------------
    L1 penalty                     : 0.0
    L2 penalty                     : 0.01
    
    Training Summary
    ----------------
    Solver                         : newton
    Solver iterations              : 7
    Solver status                  : SUCCESS: Optimal solution found.
    Training time (sec)            : 1.0412
    
    Settings
    --------
    Log-likelihood                 : 266.8357
    
    Highest Positive Coefficients
    -----------------------------
    Protagonista[TEU]              : 1.6737
    (intercept)                    : 1.1965
    Protagonista[BID]              : 1.1145
    Protagonista[HCA]              : 1.0078
    Defensa[TEU]                   : 0.9595
    
    Lowest Negative Coefficients
    ----------------------------
    Protagonista[CGN]              : -6.7269
    Defensa[GUA]                   : -2.7882
    Defensa[LOG]                   : -2.2789
    Defensa[BAR]                   : -1.8286
    Defensa[ALC]                   : -1.6842
    


### Very bad accuracy!!!


```python
resultado_model.evaluate(serbia_test_set)
```




    {'accuracy': 0.36666666666666664,
     'auc': 0.4879337226957196,
     'confusion_matrix': Columns:
     	target_label	str
     	predicted_label	str
     	count	int
     
     Rows: 9
     
     Data:
     +----------------------+----------------------+-------+
     |     target_label     |   predicted_label    | count |
     +----------------------+----------------------+-------+
     |  Pierde la posesión  |  Pierde la posesión  |   7   |
     |  Pierde la posesión  |         Gol          |   12  |
     |         Gol          |  Pierde la posesión  |   3   |
     |         Gol          |         Gol          |   12  |
     | Conserva la posesión |  Pierde la posesión  |   3   |
     |         Gol          | Conserva la posesión |   7   |
     | Conserva la posesión | Conserva la posesión |   3   |
     | Conserva la posesión |         Gol          |   6   |
     |  Pierde la posesión  | Conserva la posesión |   7   |
     +----------------------+----------------------+-------+
     [9 rows x 3 columns],
     'f1_score': 0.3424697907456528,
     'log_loss': 1.2378572911206172,
     'precision': 0.37164404223227754,
     'recall': 0.35489510489510484,
     'roc_curve': Columns:
     	threshold	float
     	fpr	float
     	tpr	float
     	p	int
     	n	int
     	class	int
     
     Rows: 300003
     
     Data:
     +-----------+-----+-----+----+----+-------+
     | threshold | fpr | tpr | p  | n  | class |
     +-----------+-----+-----+----+----+-------+
     |    0.0    | 1.0 | 1.0 | 12 | 48 |   0   |
     |   1e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     |   2e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     |   3e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     |   4e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     |   5e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     |   6e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     |   7e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     |   8e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     |   9e-05   | 1.0 | 1.0 | 12 | 48 |   0   |
     +-----------+-----+-----+----+----+-------+
     [300003 rows x 6 columns]
     Note: Only the head of the SFrame is printed.
     You can use print_rows(num_rows=m, num_columns=n) to print more rows and columns.}




```python
sf['predicted_resultado'] = resultado_model.predict(sf,output_type='probability_vector')
```


```python
sf
```




<div style="max-height:1000px;max-width:1500px;overflow:auto;"><table frame="box" rules="cols">
    <tr>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Nombre</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Posicion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Duracion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Accion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Decision</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Defensa</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Oposicion</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Protagonista</th>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2508040</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2720</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">BID</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ANA</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2581520</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">5480</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">GUA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (2)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">2685040</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">6080</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">GUA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (3)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">921560</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">7960</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (1)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">992720</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">7280</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (2)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1111480</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">6880</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (3)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">3507040</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">6200</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia (4)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">3766880</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">9320</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Serbia</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">HCA</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Óptima</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ATV</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (4)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">858960</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">7400</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Incorrecta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">SIN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso (5)</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">1302240</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">10200</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Apoyo pivote falso</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Correcta</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">SIN</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Deficiente</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">ADE</td>
    </tr>
</table>
<table frame="box" rules="cols">
    <tr>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">Resultado</th>
        <th style="padding-left: 1em; padding-right: 1em; text-align: center">predicted_resultado</th>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.16235293794971617,<br>0.5371435687535469, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.4103139616156577,<br>0.12227262070558918, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.4103139616156577,<br>0.12227262070558918, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.3770568361282094,<br>0.3317250268496909, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Gol</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.48243884502031553,<br>0.3197718810214899, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.48243884502031553,<br>0.3197718810214899, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Conserva la posesión</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.48243884502031553,<br>0.3197718810214899, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.48243884502031553,<br>0.3197718810214899, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Pierde la posesión</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.25787515262466376,<br>0.6299830641814343, ...</td>
    </tr>
    <tr>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">Gol</td>
        <td style="padding-left: 1em; padding-right: 1em; text-align: center; vertical-align: top">[0.25787515262466376,<br>0.6299830641814343, ...</td>
    </tr>
</table>
[329 rows x 10 columns]<br/>Note: Only the head of the SFrame is printed.<br/>You can use print_rows(num_rows=m, num_columns=n) to print more rows and columns.
</div>




```python
action_serbia = {'Protagonista':'LOG','Defensa':'BID','Accion':'Serbia'}
```


```python
action_fake_cross = {'Protagonista':'LOG','Defensa':'BID','Accion':'Apoyo pivote falso'}
```

### Probability of result (aphabetical order, i.e.: 'Conserva la posesion','Gol','Pierde la Posesion')


```python
resultado_model.predict(action_serbia,output_type='probability_vector')
```




    dtype: array
    Rows: 1
    [array('d', [0.1279896616354692, 0.43752895216271837, 0.4344813862018125])]




```python
resultado_model.predict(action_fake_cross,output_type='probability_vector')
```




    dtype: array
    Rows: 1
    [array('d', [0.08380485497982404, 0.3802546212079736, 0.5359405238122024])]




```python

```

