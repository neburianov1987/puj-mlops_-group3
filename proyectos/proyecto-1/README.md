# Proyecto de MLOps - Nivel 0 a Nivel 1

## Descripción

Este proyecto tiene como objetivo evaluar la capacidad de crear un entorno de desarrollo para Machine Learning que permita la ingesta, validación y transformación de datos, asegurando la correcta versionización del código y del ambiente de desarrollo. 

El flujo de trabajo cubre los siguientes pasos clave:
- Selección de características
- Ingesta del conjunto de datos
- Generación de estadísticas
- Creación y validación de esquemas
- Preprocesamiento y transformación de datos
- Seguimiento de la procedencia de datos mediante metadatos de ML

## Requisitos

Para ejecutar el proyecto, asegúrate de contar con los siguientes requisitos:

- **Docker** y **docker-compose** para la gestión de contenedores.
- **Python 3.8+** y las siguientes librerías:
  ```bash
  pip install -r requirements.txt
  ```
- **Jupyter Notebook** para la ejecución de los scripts de procesamiento de datos.
- **Git** para la gestión del código y versionado.

## Instalación

1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/tu_usuario/tu_repositorio.git
   ```
2. Accede al directorio del proyecto:
   ```bash
   cd tu_repositorio
   ```
3. Construye y levanta los contenedores con Docker:
   ```bash
   docker-compose up --build
   ```
4. Accede a Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## Uso del Proyecto

1. **Cargar el Dataset**
   - El conjunto de datos utilizado se basa en una variante del *Tipo de Cubierta Forestal*.
   - Puedes descargar el dataset desde el enlace proporcionado en el notebook o desde la fuente original.

2. **Pipeline de Datos**
   - Selección de características relevantes.
   - Ingesta y validación de datos mediante *ExampleGen*.
   - Generación de estadísticas con *StatisticsGen*.
   - Creación y validación de esquemas con *SchemaGen* y *TFDV*.
   - Transformación de datos con *Transform* para aplicar ingeniería de características.

3. **Ejecución y Monitoreo**
   - Los metadatos se almacenan con ML Metadata para garantizar la trazabilidad de los artefactos generados.
   - Se puede visualizar la canalización en ejecución y los artefactos almacenados mediante herramientas de monitoreo.

## Estructura del Proyecto

```
📂 tu_repositorio/
 ├── data/               # Conjunto de datos
 ├── notebooks/          # Jupyter Notebooks con análisis y procesamiento
 ├── src/                # Código fuente del proyecto
 ├── docker-compose.yml  # Definición del entorno Docker
 ├── requirements.txt    # Dependencias del proyecto
 ├── README.md           # Documentación del proyecto
```

## Contribuciones

Las contribuciones son bienvenidas. Para colaborar:
1. Haz un *fork* del repositorio.
2. Crea una nueva rama para tu contribución:
   ```bash
   git checkout -b feature/nueva_funcionalidad
   ```
3. Realiza los cambios y haz *commit*:
   ```bash
   git commit -m "Agregada nueva funcionalidad"
   ```
4. Sube los cambios a tu *fork*:
   ```bash
   git push origin feature/nueva_funcionalidad
   ```
5. Abre un *Pull Request* en el repositorio original.

## Contacto

Si tienes dudas o sugerencias, no dudes en crear un *issue* o contactarme a través de GitHub.

---

### Autor

**Cristian Javier Diaz Alvarez**  
Pontificia Universidad Javeriana  
Fecha: 19 de febrero de 2025
