# Ejercicio 1 - ETL

Este proyecto es parte de un ejercicio para demostrar conocimientos en un proceso de extracción, transformación y carga (ETL) utilizando Python. El objetivo principal es procesar datos de candidatos que participaron en procesos de selección, realizar transformaciones específicas y almacenar los resultados en una base de datos relacional.

## Objetivo del Proyecto 🎯

El propósito de este proyecto es:
1. Extraer los datos desde un archivo CSV.
2. Cargar los datos en una base de datos relacional (área de staging).
3. Transformar los datos aplicando una lógica de negocio específica.
4. Cargar los datos transformados en una nueva tabla de la base de datos.
5. Realizar un análisis básico de los datos almacenados.

## Flujo del Proceso ETL 🚦 
**1. Lectura del archivo CSV:**
- Se usa Python para leer los datos del archivo proporcionado.
  
**2. Carga en la base de datos (Staging Area):**
- Se migra la información cruda a una tabla en la base de datos relacional seleccionada.
  
**3. Lectura de la tabla de staging:**
- Se verifica que los datos se hayan cargado correctamente.
  
**4. Transformación de los datos:**
- Se crea una nueva columna hired, que indica si un candidato fue contratado o no.
- Regla de negocio: Un candidato es considerado “Hired” si su puntaje en el desafío de código (code_challenge_score) y en la entrevista técnica (technical_interview_score) son ambos mayores o iguales a 7.

**5. Carga de los datos transformados:**
- Los datos procesados se almacenan en una nueva tabla de la base de datos.

## Tecnologías Utilizadas 🛠 
- **Lenguaje de Programación:** Python
- **Entorno:** Jupyter Notebook
- **Base de Datos:** (A elección del desarrollador, en este caso se utilizó PostgreSQL)
- **Librerías:**
  - *pandas* para manipulación de datos.
  - *sqlalchemy* para la conexión con la base de datos.
  - *psycopg2* para la interacción con PostgreSQL.
  - *PyYAML* para la gestión de configuraciones.
 
## Instrucciones para ejecutar el proyecto

**1. Clonar el repositorio:**

```bash
git clone https://github.com/DanielaGomez98/Ejercicio-1_ETL.git
cd Ejercicio-1_ETL
```

**2. Instalar las dependencias:**
   
```bash
pip install -r requirements.txt
```

**3. Abrir el notebook deseado y comenzar a trabajar con el proyecto.**
