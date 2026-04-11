# Proyecto IoT — Gestión de Datos en Manufactura

Plataforma IoT para monitoreo predictivo de maquinaria industrial mediante recolección y análisis de datos en tiempo real.

---

##  Descripción

Este proyecto consiste en el desarrollo de una plataforma IoT para una planta de manufactura, orientada a la recolección y análisis de datos provenientes de una red de sensores instalados en máquinas industriales.

El objetivo es monitorear variables como **temperatura** y **vibración**, para utilizarlos de forma predictiva y prevenir posibles fallas mediante modelos de inteligencia artificial iterativos.

El sistema integra:
- Ingesta de datos en tiempo real
- Procesamiento de datos
- Visualización mediante dashboards para ingenieros

---

##  Arquitectura

Se implementa una **Arquitectura Pipeline Híbrido Modular**, que separa:

| Componente | Tipo | Descripción |
|---|---|---|
| Ingesta de datos IoT | Estructura Rígida | Recolección estable y confiable desde sensores |
| Análisis e IA | Estructura Flexible | Modelos adaptativos y procesamiento analítico |

Esta arquitectura facilita la **escalabilidad**, mejora la **interoperabilidad** entre componentes y permite adaptar el sistema a futuras necesidades sin afectar las operaciones principales.

---

##  Requisitos

| Herramienta | Descripción |
|---|---|
| Git | Control de versiones |
| Docker | Contenedores |
| Python 3.10+ | Lenguaje principal |
| Apache Kafka | Ingesta de datos |
| Apache Spark | Procesamiento |
| Medallion | Procesamiento por capas |
| Power BI (o similar) | Visualización |

---

## Instalación

**1. Clonar el repositorio**
```bash
git clone https://github.com/mikjimenez/Proyecto-IoT-GestionDatos
```

**2. Acceder al directorio**
```bash
cd proyecto-iot
```

**3. Levantar servicios con Docker**
```bash
docker-compose up -d
```

**4. Ejecutar el pipeline de datos**
```bash
python main.py
```

**5. Acceder al dashboard**

Abrir en el navegador: [http://localhost:3000](http://localhost:3000)

---

## Estructura del Repositorio

```
Proyecto-IoT-GestionDatos/
│
├── data/                # Datos crudos y procesados
├── ingestion/           # Configuración de Kafka
├── processing/          # Scripts de Spark
├── models/              # Modelos de IA
├── api/                 # API Gateway
├── dashboard/           # Visualización
├── docker-compose.yml   # Configuración de contenedores
└── README.md
```

