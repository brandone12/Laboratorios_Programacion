# Laboratorios de Programación para Analítica Web

Repositorio con los laboratorios y ejercicios prácticos del curso de Programación para Analítica Web, organizados por cohortes y semanas.

## 📋 Requisitos Previos

- Python 3.13 o superior
- Poetry (gestor de dependencias y entornos virtuales)

## 🚀 Configuración del Proyecto

### 1. Instalar Poetry

Poetry es un gestor de dependencias y empaquetado para Python que facilita la gestión de proyectos.

#### En Windows (PowerShell)

```powershell
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -
```

O usando pip:

```powershell
pip install poetry
```

#### En macOS / Linux

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

O usando pip:

```bash
pip install poetry
```

#### Verificar la instalación

Después de instalar, cierra y vuelve a abrir tu terminal, luego verifica la instalación:

```bash
poetry --version
```

Si el comando no es reconocido, es posible que necesites agregar Poetry a tu PATH. La ubicación típica es:
- **Windows**: `%APPDATA%\Python\Scripts`
- **macOS/Linux**: `$HOME/.local/bin`

### 2. Clonar el Repositorio

```bash
git clone <URL_DEL_REPOSITORIO>
cd Laboratorios
```

### 3. Instalar Dependencias

Una vez dentro del directorio del proyecto, instala todas las dependencias usando Poetry:

```bash
poetry install
```

Este comando:
- Creará un entorno virtual automáticamente
- Instalará todas las dependencias especificadas en `pyproject.toml` (pandas, numpy, ipykernel)

### 4. Activar el Entorno Virtual

```bash
poetry shell
```

Alternativamente, puedes ejecutar comandos sin activar el shell usando:

```bash
poetry run <comando>
```

### 5. Trabajar con los Notebooks

Para trabajar con los notebooks de Jupyter, puedes usar:

#### Opción 1: VS Code
- Abre el proyecto en VS Code
- Asegúrate de seleccionar el kernel de Python del entorno virtual de Poetry
- Abre cualquier notebook (.ipynb) y comienza a trabajar

#### Opción 2: Jupyter Lab
```bash
poetry run jupyter lab
```

#### Opción 3: Jupyter Notebook
```bash
poetry run jupyter notebook
```

## 📁 Estructura del Proyecto

```
Laboratorios/
├── pyproject.toml          # Configuración del proyecto y dependencias
├── README.md               # Este archivo
└── Cohorte I/
    ├── Semana 1/          # Fundamentos de Python
    │   ├── PY0101EN-1-1-Write_your_first_python_code.ipynb
    │   ├── PY0101EN-1-2-Strings.ipynb
    │   ├── PY0101EN-2-1-Tuples.ipynb
    │   ├── PY0101EN-2-2-Lists.ipynb
    │   ├── PY0101EN-2-3-Sets.ipynb
    │   └── PY0101EN-2-4-Dictionaries.ipynb
    ├── Semana 2/          # Control de flujo y archivos
    │   ├── 3-1.2ExcecptionHandling.ipynb
    │   ├── PY0101EN-3-1-Conditions.ipynb
    │   ├── PY0101EN-3-2-Loops.ipynb
    │   ├── PY0101EN-3-3-Functions.ipynb
    │   ├── PY0101EN-4-1-ReadFile.ipynb
    │   └── PY0101EN-4-2-WriteFile.ipynb
    └── Semana 3/          # Pandas y NumPy
        ├── DA0101EN-Review-Introduction.jupyterlite.ipynb
        ├── Module 4_Pandas_Practice.ipynb
        ├── Module 5_PY0101EN-5-1-Numpy1D.ipynb
        └── Module 5_PY0101EN-5-2-Numpy2D.ipynb
```

## 📦 Dependencias Principales

- **pandas** (>=3.0.1): Análisis y manipulación de datos
- **numpy** (>=2.4.2): Computación numérica
- **ipykernel** (>=7.2.0): Kernel de Python para Jupyter

## 🔧 Comandos Útiles de Poetry

```bash
# Ver las dependencias instaladas
poetry show

# Agregar una nueva dependencia
poetry add <paquete>

# Agregar una dependencia de desarrollo
poetry add --group dev <paquete>

# Actualizar dependencias
poetry update

# Salir del entorno virtual
exit
```

## 📝 Notas Adicionales

- Asegúrate de tener Python 3.13 o superior instalado en tu sistema
- Los notebooks están organizados por semanas y progresivamente cubren temas desde lo básico hasta análisis de datos
- Cada notebook es independiente y puede ejecutarse por separado

## 👤 Autor

Brandon Quezada - brandonquezada02@gmail.com

## 📄 Licencia

Este proyecto es parte del material educativo del curso de Programación para Analítica Web.