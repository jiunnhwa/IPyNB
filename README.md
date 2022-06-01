# IPyNB
Interactive Python log parser using a Jupyter notebook extension on VS Code without using Jupyter Notebook.

On demand interactive analysis can be quite useful for ad-hoc queries on data from machines, curreencies, etc.

## Machine Data: Log Filtering, Sorting and Analysis. ##
Data output cutout.

<img src="https://github.com/jiunnhwa/IPyNB/blob/main/SCADA_RTU_SER/hisevent.PNG" width=70% >


### HISEVENT_PARSER: Use of Lamda. ###
```
def filter_func(x):
    return x['EQUIPMENTNAME'].str.contains('SMC__0001', na=False) 

df.groupby(['EQUIPMENTNAME']).filter(filter_func)
```

## Forex Data: Volatility By Hour Analysis from Logs. ##
<img src="https://github.com/jiunnhwa/IPyNB/blob/main/CCY/ATR%20Vol%20By%20Hour.PNG" width=70% >

### Volatility: Plot. ###
```
df.plot(x='Hour',y='Val')
```
