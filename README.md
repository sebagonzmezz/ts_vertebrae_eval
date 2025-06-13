# Configuración

Para poder correr el código del ejemplo:

1. **Crear un entorno virtual** (elige una de las siguientes opciones):

   - **Conda**:
     ```bash
     conda create --name myenv python=3.10 -y
     conda activate myenv
     ```

   - **venv** (incluido en Python):
     ```bash
     python -m venv myenv
     source myenv/bin/activate        # Linux/macOS
     myenv\Scripts\activate           # Windows
     ```

   - **virtualenv**:
     ```bash
     pip install virtualenv
     virtualenv myenv
     source myenv/bin/activate        # Linux/macOS
     myenv\Scripts\activate           # Windows
     ```

2. **Clonar el repositorio**:
   ```bash
   git clone https://github.com/usuario/repositorio.git
   cd repositorio

3. **Instalar dependencias**:
   ```bash
   pip install -r requirements.txt

# Objetivo
Evaluar un modelo de segmentación de órganos en tomografías computarizadas.

# Descripción
En este proyecto se busca evaluar el desempeño del modelo TotalSegmentator en la segmentación de las vértebras T8, T10 y L4. La segmentación de estas vértebras puede resultar útil para delimitar la zona abdominal en un escáner de tomografía computarizada, con la vértebra L4 delimitando la parte inferior, y las vértebras T8 y T10 delimitando la parte superior, según el criterio adpotado.

# Dataset
El dataset a utilizar corresponde a un subconjunto del dataset original de TotalSegmentator, conformado por 1089 CTs y sus respectivas 1089 máscaras de segmentación de vertebras generadas manualmente por expertos.


# Métricas
Utilzar índice Dice para evaluar la segmentación generada por TotalSegmentator, comparándola con las máscaras generadas manualmente por expertos.
- Presentar métrica DICE
- Presentar ejemplo de resultados usando slicer3D
- Presentar 3 ejemplos buenos y 3 malos
