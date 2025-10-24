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

### 🔹 1. Clonar el repositorio

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

## Ejecutar el análisis exploratorio

- Opción 1 — Usando Jupyter Notebook

```bash
jupyter notebook
```
Luego abre el archivo notebooks\data_exploration.ipynb

- Opción 2 — Desde un editor (como VS Code)

Abre el proyecto, activa el entorno virtual y ejecuta las celdas del notebook o los scripts Python.
