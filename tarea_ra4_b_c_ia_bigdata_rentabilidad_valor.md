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

---

## 6) Diagrama del pipeline

```mermaid
flowchart LR
A[Fuentes de datos] --> B[Ingesta]
B --> C[Limpieza y normalización]
C --> D[Data Lake]
D --> E[Feature Engineering]
E --> F[Modelo IA (LSTM)]
F --> G[Predicción demanda]
G --> H[Decisiones logísticas]
H --> I[Impacto en KPIs]
```

---

## 7) Riesgos y mitigación

**Riesgo 1:** Datos incompletos o sesgados.

* **Mitigación:** Validación automática y auditorías periódicas de calidad de datos.

**Riesgo 2:** Sobredependencia del modelo (errores de predicción).

* **Mitigación:** Supervisión humana + actualización continua del modelo (retraining mensual).

---

## 8) Valoración (criterio c): importancia presente y futura de la IA

* **Importancia actual (hoy):**
  La IA ya es clave en retail para previsión de demanda, personalización y optimización logística. Permite decisiones basadas en datos en tiempo real y mejora directa de la rentabilidad. Empresas como Amazon han demostrado que la ventaja competitiva depende del uso intensivo de datos e IA.

* **Importancia futura (3–5 años):**
  La IA será aún más estratégica con modelos generativos, automatización total de cadenas de suministro y decisiones autónomas. La integración con IoT y análisis predictivo avanzado permitirá cadenas casi auto-gestionadas.

* **Condiciones/limitaciones:**
  Necesidad de datos de calidad, inversión tecnológica alta, regulación (RGPD), ciberseguridad y formación del personal. Riesgo ético si se usan datos personales sin transparencia.

* **Conclusión razonada:**
  La IA no solo optimiza procesos actuales sino que redefine el modelo de negocio. Las empresas que integren Big Data e IA de forma estratégica serán más competitivas, eficientes y rentables en el medio y largo plazo.

---

## 9) Fuentes oficiales

* **Big Data/analítica:** Comisión Europea – Estrategia Europea de Datos
  [https://commission.europa.eu/strategy-and-policy/priorities-2019-2024/europe-fit-digital-age/european-data-strategy_es](https://commission.europa.eu/strategy-and-policy/priorities-2019-2024/europe-fit-digital-age/european-data-strategy_es)

* **IA/técnica/modelo:** Documentación oficial TensorFlow (LSTM y redes neuronales)
  [https://www.tensorflow.org/guide/keras/rnn](https://www.tensorflow.org/guide/keras/rnn)

---
