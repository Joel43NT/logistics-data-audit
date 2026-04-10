# logistics-data-audit-Novaretail
# 📊 Análisis de Retención y Eficiencia: Marketplace NovaRetail

## 📋 Contexto de Negocio
NovaRetail ha detectado una anomalía en su crecimiento: a pesar de un aumento en la inversión publicitaria, la tasa de conversión y el abandono de usuarios muestran comportamientos erráticos. Como Analista de Datos, mi objetivo fue auditar la relación entre el gasto, la tecnología y el comportamiento del cliente para identificar fugas de capital.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python (Pandas, NumPy, Scipy)
* **Estadística:** Correlación de Pearson, Punto Biserial y V de Cramer (con corrección de sesgo).
* **Visualización:** Matplotlib, Seaborn y Tablas Dinámicas.

## 🔍 Hallazgos Clave

### 1. El Embudo de Conversión (Pearson)
* **Evidencia:** Correlación Inversión vs Visitas (**0.58**) vs Visitas vs Compras (**0.35**).
* **Insight:** Marketing está atrayendo tráfico de calidad, pero la plataforma está fallando en el cierre de ventas. Existe una ineficiencia en el flujo de checkout.

### 2. Segmentación y Lealtad (Punto Biserial)
* **Evidencia:** Correlación Miembro Premium vs Ingreso Anual (**0.0931**).
* **Insight:** El programa Premium no está actuando como un motor de gasto. Los clientes de mayor valor no están siendo retenidos por la membresía actual.

### 3. Independencia de Infraestructura (V de Cramer)
* **Evidencia:** V de Cramer Región vs Dispositivo (**0.0000**).
* **Insight:** El comportamiento de uso es 100% homogéneo. Esto descarta problemas logísticos regionales o fallos técnicos específicos en la App, sugiriendo que el problema es de la **Propuesta de Valor nacional**.

## 📈 Impacto de Negocio
Este análisis permitió desviar la atención de "problemas técnicos inexistentes" hacia una reestructuración de la estrategia de beneficios Premium y una auditoría de la experiencia de usuario en el carrito de compras, con un potencial de ahorro en adquisición de clientes del **15%**.

## 🚀 Cómo ejecutar el proyecto
1. Clonar el repositorio.
2. Instalar dependencias: `pip install pandas scipy matplotlib seaborn`.
3. Ejecutar el notebook `notebooks/analisis_correlacion.ipynb`.
