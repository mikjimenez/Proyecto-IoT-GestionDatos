Descripción del Proyecto
Este proyecto consiste en el desarrollo de una plataforma IoT para una planta de manufactura, orientada a la recolección y análisis de datos provenientes de una red de sensores instalados en maquinas industriales. El objetivo del proyecto es monitorear variables como temperatura y vibración, para utilizar estos datos de forma predictiva y prevenir posibles fallas mediante modelos de inteligencia artificial iterativos. 
El sistema integra procesos de ingesta de datos en tiempo real, procesamiento de los mismos y visualización para los ingenieros mediante dashboards, permitiendo mejorar la toma de decisiones en el entorno de procesos industriales de la manufactura.
Arquitectura Seleccionada 
Se implementa una arquitectura Pipeline Hibrido Modular, la cual permite separar la ingesta de datos IoT (Estructura Rígida) de los procesos analíticos y de inteligencia artificial (Estructura Flexible).

Esta arquitectura facilita la escalabilidad, mejora la interoperabilidad entre componentes y permite adaptar el sistema a futuras necesidades sin afectar las operaciones principales de la empresa.

Requisitos y Configuración del Entorno
Para ejecutar el proyecto, se requieren las siguientes herramientas:
•	Git (control de versiones) 
•	Docker (contenedores) 
•	Python 3.10+ 
•	Apache Kafka (ingesta de datos) 
•	Apache Spark (procesamiento) 
•	Medallion (procesamiento)
•	Herramientas de visualización (Power BI o similar)

Instrucciones de Instalación
Clonar el repositorio: 
git clone https://github.com/mikjimenez/Proyecto-IoT-GestionDatos

Acceder al directorio: 
cd proyecto-iot

Levantar servicios con Docker: 
docker-compose up -d

Ejecutar el pipeline de datos: 
python main.py

Acceder al dashboard desde: 
http://localhost:3000

Estructura del Repositorio
Proyecto-IoT-GestionDatos /
│
├── data/                     			# Datos crudos y procesados
├── ingestion/             			# Configuración de Kafka
├── processing/          			# Scripts de Spark
├── models/                			# Modelos de IA
├── api/                			# API Gateway
├── dashboard/        			# Visualización
├── docker-compose.yml   		# Configuración de contenedores
└── README.md

