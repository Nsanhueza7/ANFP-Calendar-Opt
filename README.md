# Modelo Optimización Programación Dinámica Calendario Deportivo ANFP

Modelo computacional de optimización del calendario deportivo ANFP.

## Modo de uso


### Visualizar Rendimiento

- Guardar stdout una carpeta, por ejemplo `python3 SSTPA/V3/model.py fi ff >> STPA/logs/log_{fi}-{ff}`.

- Se modifican parámetros de `gen_stats.py`. `LOGS` son los nombres de los logs dentro de la ruta `PATH`.

- Comando `python3 gen_stats.py`.

- Se crea una carpeta en `output/visualization` llamada `{NAME}-vis` con distintas visualizaciones.

- Comando para guardar varios logs a una carpeta `for i in {fi..ff}; do python3 SSTPA/model.py $i 30 > SSTPA/logs/folder/log_$i-30; done `, por ejemplo, `for i in {18..25}; do python3 SSTPA/model.py $i 30 > SSTPA/logs/26-6/log_$i-30; done `


### SSTPA V3

`python3 SSTPA/V3/model.py fi ff`

Donde `fi` y `ff` son la fecha inicial y fecha final a programar.

### SSTPA V4

Rama `modelo-V4`

`python3 SSTPA/V4/model.py`

## Modelo 1: SSTPA

### Cambios Recientes

- `refactor:` modulo de carga de datos.

- Incorporacion de parametro `BREAKS`.

- `feature:` Generación de gráficos para fit de funciones lineales, polinomiales y exponenciales de tiempo vs fechas.

## Modelo 2: FPP

Standby

## To Do

- `pat_gen` refactor.

- Cambiar variables binarias por enteras.

- Sample de patrones para reducción de dimensionalidad.


