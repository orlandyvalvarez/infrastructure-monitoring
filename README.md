Proyecto 04 – Infrastructure Monitoring

Laboratorio práctico de monitoreo de infraestructura utilizando Prometheus, Node Exporter y Grafana.

El objetivo de este proyecto es implementar una solución de monitoreo capaz de recopilar métricas de un servidor Linux, almacenarlas mediante Prometheus y visualizarlas a través de dashboards en Grafana.

Objetivo

Implementar un sistema básico de monitoreo de infraestructura que permita:

* Recopilar métricas del sistema Linux.
* Monitorear recursos del servidor.
* Configurar Prometheus como sistema de recopilación de métricas.
* Utilizar Node Exporter para exponer métricas del sistema.
* Integrar Prometheus como fuente de datos en Grafana.
* Visualizar las métricas mediante dashboards.

Arquitectura del laboratorio

                ┌─────────────────────┐
                │    Servidor Linux   │
                │                     │
                │    Node Exporter    │
                │         │           │
                └─────────┼───────────┘
                          │
                          │ Métricas
                          ▼
                ┌─────────────────────┐
                │     Prometheus      │
                │                     │
                │  Recolección de     │
                │      métricas       │
                └─────────┬───────────┘
                          │
                          │ Data Source
                          ▼
                ┌─────────────────────┐
                │       Grafana       │
                │                     │
                │     Dashboards      │
                └─────────────────────┘

Tecnologías utilizadas

* Linux
* Prometheus
* Node Exporter
* Grafana
* VMware Workstation
* TCP/IP
* HTTP
* Monitoring & Observability

Entorno del laboratorio

El laboratorio fue realizado en un entorno virtualizado utilizando VMware Workstation.

El servidor Linux funciona como sistema monitoreado y ejecuta Node Exporter y Prometheus. Grafana se utiliza para consultar las métricas recopiladas y representarlas mediante dashboards.

1. Verificación del sistema

Antes de comenzar la implementación se realizó una verificación del sistema Linux y de la conectividad de red.

2. Instalación y verificación de Node Exporter

Node Exporter permite exponer métricas relacionadas con el sistema operativo y los recursos del servidor para que Prometheus pueda recopilarlas.

3. Configuración de Prometheus

Se configuró Prometheus para recopilar las métricas proporcionadas por Node Exporter.

Posteriormente se verificó que el servidor Prometheus estuviera correctamente iniciado y disponible.

4. Instalación de Grafana

Se instaló Grafana como plataforma de visualización para las métricas recopiladas por Prometheus.

Durante la implementación se presentó inicialmente un problema de compatibilidad con Firefox.

Posteriormente se logró acceder correctamente a la interfaz de Grafana.

5. Configuración de Prometheus como Data Source

Se configuró Prometheus como fuente de datos dentro de Grafana.

Conexión

Agregar nueva conexión

Selección de Prometheus

Configuración de la URL

6. Dashboard de monitoreo

Finalmente se importó un dashboard para visualizar las métricas proporcionadas por Node Exporter.

El dashboard permite consultar información relacionada con el estado y utilización de los recursos del sistema.

Métricas monitoreadas

Entre las métricas disponibles se encuentran diferentes indicadores relacionados con:

* CPU
* Memoria RAM
* Uso del sistema
* Disco
* Red
* Procesos
* Disponibilidad del sistema

Evidencias

Las evidencias del laboratorio se encuentran directamente en este repositorio y documentan las principales etapas de implementación:

1. Verificación del sistema y red.
2. Node Exporter.
3. Prometheus.
4. Estado del servidor Prometheus.
5. Instalación de Grafana.
6. Resolución del problema de compatibilidad.
7. Acceso a Grafana.
8. Conexión de Grafana.
9. Configuración de Prometheus.
10. Configuración de la URL.
11. Dashboard final.

Resultado

Se implementó correctamente un entorno básico de Infrastructure Monitoring, integrando:

Node Exporter → Prometheus → Grafana

El laboratorio permite recopilar métricas de un servidor Linux y visualizarlas mediante dashboards, proporcionando una base práctica para tareas de monitoreo y observabilidad de infraestructura.

Aprendizajes

Durante este proyecto se trabajó con:

* Monitoreo de servidores Linux.
* Instalación y configuración de Node Exporter.
* Configuración de Prometheus.
* Integración entre Prometheus y Grafana.
* Configuración de Data Sources.
* Visualización de métricas mediante dashboards.
* Identificación y resolución de problemas durante la implementación.

Portafolio

Orlandy Vilorio | Cloud & Infrastructure

https://orlandyvalvarez.github.io/
