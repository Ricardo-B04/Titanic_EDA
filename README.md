# Análisis Exploratorio de Datos — Titanic

Exploración y visualización del dataset del Titanic para descubrir cómo variables como la clase social, el género y la edad influyeron en la supervivencia de los pasajeros.

## Descripción

El dataset contiene registros de 891 pasajeros con variables categóricas, continuas y binarias, incluyendo datos faltantes no triviales. El análisis abarca:

- Carga y limpieza de datos
- Estadísticas descriptivas y manejo de valores nulos
- Análisis univariado (distribuciones de edad, tarifa, clase, género)
- Análisis bivariado (supervivencia por clase, género, tamaño familiar, puerto de embarque)
- Detección de outliers con IQR
- Prueba chi-cuadrado e hipótesis estadísticas
- Heatmap de correlaciones y visualizaciones avanzadas

## Estructura del proyecto

```
Titanic_EDA/
├── titanic_EDA.ipynb   # Notebook principal con el análisis completo
├── README.md           # Este archivo
└── requirements.txt    # Dependencias del proyecto
```

## Datos

El dataset se carga directamente desde el repositorio público de Kaggle/datasciencedojo:

```
https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
```

No es necesario descargar ningún archivo adicional.

## Instalación

1. Clonar o descargar el repositorio.
2. (Recomendado) Crear un entorno virtual:

```bash
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
.venv\Scripts\activate      # Windows
```

3. Instalar las dependencias:

```bash
pip install -r requirements.txt
```

4. Abrir el notebook:

```bash
jupyter notebook titanic_EDA.ipynb
```

## Dependencias

- Python 3.9+
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- jupyter

## Variables del dataset

| Variable | Descripción |
|----------|-------------|
| `Survived` | Supervivencia (0 = No, 1 = Sí) |
| `Pclass` | Clase del pasajero (1 = 1ª, 2 = 2ª, 3 = 3ª) |
| `Name` | Nombre del pasajero |
| `Sex` | Género |
| `Age` | Edad en años |
| `SibSp` | Nº de hermanos/cónyuge a bordo |
| `Parch` | Nº de padres/hijos a bordo |
| `Ticket` | Número de boleto |
| `Fare` | Tarifa del pasaje |
| `Cabin` | Número de cabina |
| `Embarked` | Puerto de embarque (C = Cherburgo, Q = Queenstown, S = Southampton) |
