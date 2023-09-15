# Uber Data Engineering Project


## Objetivo
Este repositorio tiene como objetivo emular un proyecto "end to end" similar a las situaciones del mundo laboral. Se basa en un proyecto educativo donde se realizarán análisis de datos utilizando diversas herramientas y tecnologías, incluyendo GCP Storage, Python, Compute Instance, Mage Data Pipeline Tool, BigQuery y Looker Studio.

## Descripción
A lo largo del proyecto, comenzaremos con un archivo CSV, crearemos un diseño lógico, transformaremos el conjunto de datos, utilizaremos GCP y Mage para la creación de un pipeline ETL (Extract, Transform, Load), emplearemos BigQuery y, finalmente, crearemos un dashboard con Looker Studio. Este repositorio servirá como guía y ejemplo para comprender cómo se llevan a cabo proyectos similares en un entorno laboral real.

## Arquitectura 
![Arquitectura](https://github.com/LorenzoG9917/uber_data_engineer/assets/121797266/e5f1c003-b440-4fb8-bd34-0c2a1589507b)
## Tecnologías usadas
- Lenguaje de Programación: Python (Librería pandas)

- Google Cloud Platform (GCP)
- Google Storage: Almacenamiento en la nube de GCP.
- Compute Instance: Instancia de cómputo para ejecución de tareas en GCP.
- BigQuery: Base de datos empresarial de Google.
- Looker Studio: Herramienta de creación de dashboards
- Herramienta Moderna de pipeline de Datos: [Mage Data Pipeline Tool](https://www.mage.ai/)

## Conjunto de Datos Utilizado

Se utilizó el conjunto de datos "TLC Trip Record Data" del año 2016 que incluye registros de viajes en dos empresas de taxis. Estos registros capturan información como fechas y horarios de recogida y entrega, ubicaciones de recogida y entrega, distancias de viaje, tarifas detalladas, tipos de tarifas, tipos de pago y recuentos de pasajeros reportados por el conductor.
- Sitio web de los Datos: [TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

## Paso a paso
1. Diseño Lógico del Conjunto de Datos: Se creó un diseño lógico utilizando Lucidchart para diseñar un Modelo de Entidad-Relación (ERD).
2. Importación y Transformación de Datos: Los datos se importaron en un Jupyter notebook para transformarlos. Se crearon claves primarias (PK) y claves foráneas (FK) según lo definido en el ERD. Finalmente se creo una especie de tablón el cual contiene los joins entre la fact table y las dimensions tables del modelo.
3. Almacenamiento en GCP: Se utilizó Google Cloud Platform para almacenar los datos en un "bucket" único de almacenamiento en la nube.
4. Implementación de Mage: Se configuró una instancia virtual en Compute Engine y se instaló Mage en ella. Se establecieron las conexiones necesarias.
5. Creación de la Canalización ETL: Se utilizó Mage para crear una canalización ETL utilizando el bloque Dataloader para extraer el conjunto de datos y se aplicaron transformaciones realizadas previamente en el paso 2.
6. Exportación de Datos a BigQuery: Los datos se exportaron a BigQuery utilizando un bucle for y se configuraron las credenciales para conectarse a los servidores de Google.
7. Creación de dashboard en Looker Studio: Se utilizó Looker Studio para crear un dashboard que incluye filtros, resúmenes y gráficos interactivos.
8. Compartiendo el Panel de Control: El [dashboard](https://lookerstudio.google.com/reporting/f8f88d7e-c1f1-4ee4-8dfe-4620bf961b93/page/DlVaD) se compartió a través de Looker Studio.


## Agradecimientos

- Agradecimientos especiales a [Darshil Parmar](https://www.linkedin.com/in/darshil-parmar/) por la creación de este proyecto con fines educativos.
- Este proyecto se basa en un repositorio en inglés creado por [Mudasir Wazir](https://www.linkedin.com/in/mudasir-wazir/).

## Autor

Este repositorio ha sido personalizado y adaptado por [Lorenzo Guerrero](https://www.linkedin.com/feed/) con fines educativos.
