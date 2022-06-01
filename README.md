# IPyNB
Interactive Python log parser using a Jupyter notebook extension.

## Sample: Log Filtering, Sorting and Analysis. ##
Data output cutout.

<img src="https://github.com/jiunnhwa/IPyNB/blob/main/SCADA_RTU_SER/hisevent.PNG" width=70% >


### HISEVENT_PARSER: Use of Lamda. ###
```
def filter_func(x):
    return x['EQUIPMENTNAME'].str.contains('SMC__0001', na=False) 

df.groupby(['EQUIPMENTNAME']).filter(filter_func)
```
