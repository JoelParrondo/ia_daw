# Práctica IA (RA4 · b+c) — Big Data, análisis, rentabilidad y valoración IA

---

## 1) Caso y objetivo de negocio

* **Empresa/sector (real o ficticia):** Zara (retail moda, perteneciente a Inditex)
* **Problema a resolver:** Roturas de stock y sobrestock por mala previsión de demanda en tiendas físicas y online.
* **Objetivo de negocio (rentabilidad):** Aumentar ventas y reducir costes logísticos mediante una predicción de demanda basada en IA.

---

## 2) Big Data: recogida masiva de datos

Es Big Data porque cumple las 3V:

* **Volumen:** millones de transacciones diarias a nivel global.
* **Velocidad:** datos en tiempo real (ventas online, stock, clics web).
* **Variedad:** datos estructurados y no estructurados (ventas, imágenes, redes sociales).

**Fuentes:**

* **Fuente 1:** Ventas en tiendas físicas (TPV).

* **Fuente 2:** Datos de e-commerce (clics, carritos, búsquedas).

* **Fuente 3:** Redes sociales (tendencias de moda, comentarios).

* **Volumen/velocidad (estimación):** +5 millones de transacciones/día; actualización casi en tiempo real.

* **Formatos:** texto (opiniones), eventos (ventas), series temporales (histórico demanda), imágenes (catálogo productos).

---

## 3) Tratamiento/análisis: pipeline de datos

* **Ingesta (captura/eventos):** APIs de tienda online, integración TPV, scraping de tendencias.
* **Limpieza/normalización:** Eliminación de duplicados, corrección de errores de stock, homogeneización de fechas y monedas.
* **Almacenamiento:** Data Lake en la nube (ej. Amazon Web Services).
* **Preparación de variables (features):**

  * Ventas históricas por tienda
  * Estacionalidad (mes, clima)
  * Tendencia en redes
  * Precio y promociones
* **Análisis/BI (opcional):** Cuadros de mando en herramientas como Microsoft Power BI.

---

## 4) IA aplicada: modelo y decisión

* **Tipo de IA/técnica:** Predicción de demanda con redes neuronales LSTM (series temporales).
* **Entrada del modelo:** Históricos de ventas, estacionalidad, clima, tendencias sociales, precios.
* **Salida del modelo:** Predicción de demanda por producto/tienda (próximas 4 semanas).
* **Decisión que habilita:** Ajustar producción y distribución; redistribuir stock entre tiendas; optimizar reposición automática.

---

## 5) Rentabilidad: KPIs antes/después

**KPI 1 (Ventas totales):**

* Antes: 100 M€/mes
* Después: 108 M€/mes
* Mejora: +8% por menor rotura de stock → más ventas disponibles.

**KPI 2 (Coste de almacenamiento):**

* Antes: 12 M€/mes
* Después: 9 M€/mes
* Mejora: –25% al reducir sobrestock y liquidaciones.

**KPI 3 (Rotación de inventario):**

* Antes: 4 rotaciones/año
* Después: 6 rotaciones/año
* Mejora: Mayor eficiencia del capital invertido en stock.
