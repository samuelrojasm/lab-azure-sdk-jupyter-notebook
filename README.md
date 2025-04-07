# 🛠️ Azure SDK Jupyter-Notebooks con Python

[![Azure](https://badgen.net/badge/icon/azure?icon=azure&label)](https://azure.microsoft.com)
[![Azure SDK for Python](https://img.shields.io/badge/Azure%20SDK%20for-Python-0078D4?logo=python&logoColor=white)](#)
[![Jupyter](https://img.shields.io/badge/Jupyter-Lab/Notebook-F37626?logo=jupyter&logoColor=white)](#)
[![Status](https://img.shields.io/badge/Status-Work%20in%20progress-yellow)](#)

- Repositorio con notebooks de laboratorio para probar y demostrar el uso del SDK de Azure (Azure SDK for Python) en notebooks Jupyter. 
- Ideal para aprender, experimentar y validar funciones del SDK en diferentes servicios de Azure.

---

## 📌 Objetivos
- Explorar y probar funcionalidades del SDK de Azure para Python.
- Crear laboratorios reproducibles con ejemplos reales.
- Facilitar la comprensión del uso del SDK en entornos interactivos.
- Servir como referencia técnica o base para otros proyectos.

---

## 📂 Contenido
### Ejemplos Azure
[]()

---

## 🧰 Tecnologías utilizadas
- [Azure SDK for Python (azure-* packages)](https://learn.microsoft.com/en-us/azure/developer/python/)
- [Jupyter Notebook](https://jupyter.org/)
- [Python 3.x](https://www.python.org/)
- [Conda](https://www.anaconda.com/docs/getting-started/miniconda/main)
- [Azure CLI](https://learn.microsoft.com/en-us/cli/azure/)

---

## 🚀 Requisitos
### 1. Instalar Azure CLI
- Instalación en macOS:
    ```bash
    brew install azure-cli
    ```
### 2. Acceso a la suscripción de Azure
- Autenticación:
    - Método interactivo (usando el navegador)
        ```bash
        az login
        ```
    - Método con autenticación interactiva en CLI (sin navegador)
        ```bash
        az login --use-device-code
        ```
- Configurar la variable de entorno:
    ```bash
    export ARM_SUBSCRIPTION_ID="<SUBSCRIPTION_ID>"
    ```
### 3. Configuración de entorno de python
Para esta opción usamos el gestor de env de python **conda**
- Crear entorno de desarrollo:
    ```
    conda create --name azure-sdk
    ```
- Instalar librerias de Azure
    ```
    conda install -c conda-forge azure-identity azure-mgmt-compute -n azure-sdk
    ```
- Lista los paquetes instalados en el environment
    ```
    conda list -n azure-sdk
    conda list -n azure-sdk azure-identity
    conda list -n azure-sdk azure-mgmt-compute
    ```
- Instalar librerías adicionales de python
    - ipykernel:
        ```
        conda install -c conda-forge ipykernel -n azure-sdk
        ```
    - Pandas: 
        ```
        conda install -c conda-forge pandas -n azure-sdk
        ```
    - duckdb: BD en memoria uso con SQL
        ```
        conda install -c conda-forge python-duckdb -n azure-sdk
        ```
    - Apache Arrow: formato de columnas en memoria
        ```
        conda install -c conda-forge pyarrow -n azure-sdk
        ```
- Activar environment de azure-sdk
    ```bash
    conda activate azure-sdk
    ```
- Desactivar el environment
    ```bash
    conda deactivate
    ```

### 4. Ejecutar de manera local Jupyter Notebook
- Entorno para trabajar con los Notebooks de python
    ```bash
    jupyter-lab
    ```
---

## 📚 Referencias adicionales
- [Azure for Python Developers](https://learn.microsoft.com/en-us/azure/developer/python/)
- [Ejemplos de Azure SDK en GitHub](https://github.com/Azure/azure-sdk-for-python)
- []()

---

## 📌 Notas
- Es necesario tener una suscripción activa de Azure.
- Algunos notebooks requieren permisos específicos o recursos ya existentes.

---
