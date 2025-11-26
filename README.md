## Requisitos previos

Antes de ejecutar el proyecto asegúrate de tener instalado:

- **Python 3.9 o superior**  
- **pip** (gestor de paquetes de Python)
- Un editor o entorno de desarrollo como:
  - [Visual Studio Code](https://code.visualstudio.com/)
  - [Jupyter Notebook](https://jupyter.org/)
  - [PyCharm](https://www.jetbrains.com/pycharm/)

---

## Ejecución en local

A continuación, se detallan los pasos para ejecutar el proyecto en **Windows**, **macOS** o **Linux**.

###  1. Clonar el repositorio

```bash
git clone https://github.com/usuario/diabetes-health-indicators.git
cd diabetes-health-indicators
```
## Crear un entorno virtual

Ahora debes ejecutar las siguientes celdas desde la ruta del proyecto:

- **Creación del entorno para windows:**
  
```bash
python -m venv .venv
```
```bash
.venv\\Scripts\\activate
```

- **Creación del entorno para Linux/Mac:**

```bash
python3 -m venv .venv
```
```bash
source .venv/bin/activate
```
Si obtienes un error del tipo "no se encontró Python", asegúrate de que esté correctamente instalado y agregado al PATH del sistema.

## Instalar dependencias 

Con el entorno activado, ejecuta:

```bash
pip install -r requirements.txt
```

Esto instalará librerías como pandas, numpy, matplotlib, seaborn y scikit-learn, necesarias para el análisis.

## Estructura del Proyecto

El flujo de trabajo se divide en 7 notebooks organizados secuencialmente. Se inicia con la exploración de datos, seguido por el entrenamiento individual de 5 modelos distintos y finaliza con una comparativa global.

1. Análisis Exploratorio (EDA)
data_exploration.ipynb: Carga inicial, limpieza de datos, análisis de correlaciones, manejo de duplicados y visualización de la distribución de las variables.

2. Entrenamiento de Modelos (Individuales)
Se han desarrollado 5 notebooks de modelado, uno por cada algoritmo. En cada uno se sigue una metodología rigurosa y estandarizada que incluye:

Preprocesamiento: Escalado de datos (si el modelo lo requiere) y manejo de clases.

Optimización: Búsqueda de hiperparámetros con GridSearchCV y validación cruzada estratificada (StratifiedKFold).

**Los modelos implementados son:**

logistic_regression.ipynb: Modelo base lineal (Regresión Logística).

exploration_KNN.ipynb: Modelo basado en instancias (K-Nearest Neighbors).

balanced_decision_forest.ipynb: Ensamble personalizado de árboles con estrategia de balanceo (Balanced Decision Forest).

exploration_SMV.ipynb: Modelo basado en maquina de vectores de soporte

exploration_MLP_scikit-learn.ipynb: Modelo basado en redes neuronales.

3. Comparativa Final
model_comparison.ipynb: Consolidación de los resultados de los 5 modelos anteriores. 
