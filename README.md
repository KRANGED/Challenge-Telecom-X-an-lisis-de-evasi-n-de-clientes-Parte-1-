# TelecomX LATAM: Análisis de Abandono de Clientes (Churn)

Este proyecto realiza un proceso completo de **ETL** (Extracción, Transformación y Carga) y un **Análisis Estratégico** sobre los datos de TelecomX para identificar los factores que impulsan la pérdida de clientes y proponer soluciones de retención.

---

## 📋 Resumen del Proyecto

El análisis se basa en un conjunto de datos complejo en formato JSON que contiene información demográfica, servicios contratados y detalles de facturación. El objetivo principal es transformar estos datos anidados en una estructura útil para la toma de decisiones de negocio.

## 🛠️ Stack Tecnológico

* **Lenguaje:** Python 3.x
* **Librerías:** Pandas (específicamente `json_normalize` para el manejo de estructuras anidadas).
* **Plataforma:** Google Colab.

## ⚙️ Estructura del Notebook

1.  **Extracción:** Carga inicial del archivo `TelecomX_Data.json`.
2.  **Transformación y Limpieza:** * Desanidado de diccionarios internos: `customer`, `phone`, `internet` y `account`.
    * Creación de un DataFrame unificado de 21 columnas.
3.  **Análisis de Datos:** Exploración de variables críticas como el método de pago, tipos de servicios y estabilidad del cliente.
4.  **Insights de Negocio:** Identificación de los "momentos de la verdad" en el ciclo de vida del cliente.

## 🔍 Hallazgos Principales

* **Puntos de Fricción:** El método de "Cheque Electrónico" presenta una mayor tasa de rotación en comparación con los pagos automáticos.
* **Segmentación por Dependencia:** Los clientes con pareja y dependientes actúan como un "ancla", mostrando mayor lealtad y preferencia por contratos de largo plazo.
* **Competitividad del Servicio:** Mientras que la telefonía se mantiene estable, el servicio de internet muestra una volatilidad mucho más alta debido a la competencia.

## 💡 Recomendaciones Estratégicas

1.  **Migración de Pago:** Incentivar el cambio de "Cheque Electrónico" a "Cargo Automático" para reducir la fricción mensual.
2.  **Estrategia de Adherencia:** Fomentar el uso de soporte técnico preventivo o pruebas de streaming para aumentar el valor percibido.
3.  **Planes Flexibles:** Crear ofertas intermedias para el perfil joven/soltero que no desea la rigidez de un contrato anual pero busca beneficios de permanencia.

---
*
