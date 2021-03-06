## Requerimientos
* python >=3.7

## Ejecución
1. Instalar dependencias mediante `pip3 install -r requirements.txt`.
2. Ejecutar programa mediante `python3 main.py <ARGUMENTOS>`.

```bash
$ python3 main.py --help                                                                                             
usage: main.py [-h] --x-axis X_AXIS --y-axis Y_AXIS [--url URL] [--chart-type {line,bar,point}] [--chart-name CHART_NAME]
               [--chart-file-name CHART_FILE_NAME] [--base64]

optional arguments:
  -h, --help                         show this help message and exit
  --x-axis X_AXIS                    Chart X axis
  --y-axis Y_AXIS                    Chart Y axis
  --url URL                          Url of data
  --chart-type {line,bar,point}      Chart type
  --chart-name CHART_NAME            Chart name
  --chart-file-name CHART_FILE_NAME  Chart file name
  --base64                           Print image as base64
```

Ejemplo:
```
$ python3 main.py --url http://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_daily_reports/04-06-2020.csv --x-axis Province_State --y-axis Confirmed --chart-type line
```