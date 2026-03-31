# Data Engineering en Microsoft Fabric: Ingesta, Transformación, Modelado Analítico y Power BI dashboard.

[![Microsoft Fabric](https://img.shields.io/badge/Microsoft%20Fabric-End--to--End%20Analytics-0078D4)](https://learn.microsoft.com/fabric/)
[![Spark Notebooks](https://img.shields.io/badge/Spark-Data%20Transformation-E25A1C)](https://spark.apache.org/)
[![Power BI](https://img.shields.io/badge/Power%20BI-Interactive%20Dashboard-F2C811)](https://powerbi.microsoft.com/)

## 1. 🧾 Introducción

Este proyecto presenta la implementación de un flujo de datos end-to-end utilizando Microsoft Fabric, integrando herramientas modernas de ingeniería y análisis de datos como Spark Notebooks y Power BI. El objetivo principal es construir una solución completa que permita transformar datos operacionales en información analítica útil para la toma de decisiones.

El proceso inicia con la ingesta de datos desde Azure SQL Database hacia OneLake, específicamente en la capa Bronze, donde los datos son almacenados en su estado original. Posteriormente, mediante el uso de Spark, se realizan tareas de limpieza, transformación y enriquecimiento de datos en la capa Silver, garantizando su calidad y consistencia.

En la capa Gold, se implementa un modelo dimensional en esquema estrella, optimizado para el análisis, el cual es almacenado en un Data Warehouse dentro de Fabric. Sobre este modelo, se construye un modelo semántico que permite estructurar y relacionar la información de manera eficiente.

Finalmente, el proyecto culmina con la creación de dashboards interactivos en Power BI, donde se visualizan indicadores clave de negocio como ventas, costos y rentabilidad, facilitando el análisis y la toma de decisiones basada en datos.

Este laboratorio permite comprender de manera práctica la arquitectura tipo Medallion (Bronze, Silver, Gold) y el potencial de Microsoft Fabric como plataforma integral de analítica de datos.

## 2. 🏗️ Arquitectura

La arquitectura del flujo está compuesta por los siguientes elementos:





## 3. 🧩 Componentes del Proyecto

- Capa Bronze (Ingesta): Almacena los datos crudos de Azure SQL Database en OneLake, preservando su formato original.
- Capa Silver (Transformación): Limpia, normaliza y enriquece los datos con Spark Notebooks, calculando métricas como ImporteVenta, Costo Total y Rentabilidad.
- Capa Gold (Modelado): Construye un modelo dimensional en esquema estrella con tablas de hechos y dimensiones, optimizado para análisis.
- Modelo Semántico: Estructura las relaciones entre las tablas Gold y crea la tabla Medidas, permitiendo consultas rápidas y análisis de KPIs.
- Dashboard Power BI: Visualiza indicadores clave mediante gráficos interactivos (ventas por tiempo, categoría y sucursal, rentabilidad, etc.), facilitando la toma de decisiones.

## 4. ✅ Beneficios del Proyecto
Aprendizaje práctico end-to-end: Permite experimentar todo el flujo de datos desde ingesta hasta visualización, consolidando conceptos de ingeniería y análisis de datos.
Uso de Microsoft Fabric integral: Enseña a aprovechar pipelines, Spark Notebooks, Data Warehouse, modelos semánticos y dashboards dentro de la misma plataforma.
Calidad y consistencia de datos: La capa Silver asegura limpieza y transformación correcta, mejorando la confiabilidad de la información.
Optimización para análisis: La capa Gold y el modelo dimensional facilitan consultas rápidas y eficientes sobre grandes volúmenes de datos.
Facilidad de análisis con modelo semántico: Permite relacionar tablas y calcular KPIs de manera sencilla, sin necesidad de conocimientos avanzados en SQL.
Visualización interactiva: Los dashboards en Power BI facilitan la interpretación de resultados y la toma de decisiones basada en datos.
Automatización y repetibilidad: Los pipelines permiten ejecutar el flujo completo de manera automática, reduciendo errores y esfuerzo manual.
