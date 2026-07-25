[🔙 Volver a la Portada Principal](README.md)

# 🔢 UNIDAD 3: Ley de Grandes Números

🧩 ¡Del análisis al modelo! Esta unidad representa el cierre del ciclo estadístico: partiendo de los fundamentos del TLC y las distribuciones muestrales, se avanzó hacia la comparación multigrupo, el análisis de relaciones entre variables y la construcción de modelos predictivos y clasificadores. Cada APE añadió una herramienta nueva al arsenal analístico, siempre anclada al dataset real del Proyecto Integrador.

---

## 🧠 Aprendizaje Práctico Experimental (APE)

Tareas diseñadas para aplicar los conocimientos teóricos en escenarios prácticos y controlados.

> [!NOTE]
> **¿No puedes visualizar los archivos `.ipynb`?**
> Al hacer clic en los enlaces, Google Drive mostrará el mensaje *"No hay ninguna aplicación instalada para abrir este archivo"* o una vista previa vacía. Para abrirlo correctamente, haz clic en el botón **"Abrir con Google Colaboratory"** que aparece en la parte superior de Drive. El notebook se cargará completo con todo el código y las celdas ejecutables.

#### 🔬 APE11: Inferencia Estadística Multigrupo: ANOVA de 1 Factor y Pruebas Post-Hoc (Tukey)
* **🗒️ Descripción:** Se aplicó ANOVA de 1 factor sobre la variable Remuneración Mensual Unificada segmentada por los 4 regímenes laborales del dataset de Loja (LOSEP=1425, Código de Trabajo=1308, LOSEP-SOC=139, LOSEP-CONCEJAL=11), obteniendo F=22.61 y p=1.24e-08, rechazando H₀. La prueba Post-Hoc de Tukey identificó diferencias significativas entre los pares Código de Trabajo vs LOSEP (p-ajustado=0.0000), entre otros. Se verificó el supuesto de homogeneidad de varianzas con Levene y se discutió Kruskal-Wallis como alternativa no paramétrica cuando el supuesto no se cumple.
* **🔗 Enlace:** [Ver Tarea APE 11 (ipynb)](https://drive.google.com/file/d/1GD_CrDPQ25xeo3stS4s__1xq7HEKTPyk/view?usp=drive_link)
  
#### 📉 APE12: Análisis Bivariado y Predicción: Correlación de Pearson y Regresión Lineal Simple (OLS)
* **🗒️ Descripción:** Se calculó la Correlación de Pearson entre la Décimo Tercera Remuneración y la Remuneración Mensual Unificada del dataset de Loja, obteniendo r=0.9646 (p≈0) — correlación positiva muy fuerte. El modelo OLS ajustado alcanzó R²=0.930, explicando el 93% de la variabilidad salarial. La predicción para un Décimo Tercero de USD 600 (fuera del dominio observado) estimó una Remuneración Mensual de USD 7,014.47, evidenciando el riesgo de extrapolación. El diagnóstico de residuos con Shapiro-Wilk (W=0.5733, p=2.21e-64) rechazó su normalidad, detectando heterocedasticidad en patrón de abanico.
* **🔗 Enlace:** [Ver Tarea APE 12 (ipynb)](https://drive.google.com/file/d/1OjOjrxRhsIVa0dcc84VE0SiMaGj5Nu-E/view?usp=drive_link)

#### 📊 APE13: Análisis Predictivo Multivariado: Regresión Lineal Múltiple y VIF
* **🗒️ Descripción:** Se ajustó un modelo de Regresión Lineal Múltiple (OLS) con tres predictores del dataset de Loja: Décimo Tercera (X1), Horas Suplementarias (X2) e Ingresos Adicionales (X3). El diagnóstico de multicolinealidad con VIF reveló que X2 (VIF=11.95) y X3 (VIF=13.86) superan el umbral crítico de 10, indicando colinealidad problemática. Se demostró que incluir la Remuneración Anual como predictor adicional eleva el VIF drásticamente, y que el R²=1.0 persistente en el modelo regional es señal de una relación funcional entre variables más que de un modelo genuinamente predictivo.
* **🔗 Enlace:** [Ver Tarea APE 13 (ipynb)](https://drive.google.com/file/d/1cpI5ZiOF_AIJYvq-3UYfGJmg2qeQc5TO/view?usp=sharing)

#### 🎲 APE14: Modelado Probabilístico Avanzado: Regresión Logística y Matrices de Confusión
* **🗒️ Descripción:** Se implementó un clasificador binario de Regresión Logística para predecir si un empleado del Municipio de Loja tiene remuneración alta (sobre la media de $713.81). El modelo logró accuracy=0.9993 con umbral=0.50, pero el diagnóstico detectó cuasi-separación completa y fuga de datos (data leakage) producida por la variable Total Ingresos Adicionales — matemáticamente derivada de la variable respuesta. Se analizó el impacto del umbral: bajarlo de 0.50 a 0.20 reduce los falsos negativos pero dispara los falsos positivos. El modelo simulado de temperatura de CPU vs. caída de servidor alcanzó accuracy=0.73, más representativo de un escenario real.
* **🔗 Enlace:** [Ver Tarea APE 14 (ipynb)](https://drive.google.com/file/d/1dhIZL5A6k8xake0hJOLHHeMRlnp_rhZw/view?usp=drive_link)

#### 📈 APE15: Evaluación Avanzada de Modelos: ROC, AUC y Validación Cruzada K-Fold
* **🗒️ Descripción:** Se construyeron curvas ROC para los tres modelos trabajados. El modelo simulado de servidor obtuvo AUC=0.814 — capacidad discriminativa genuina. El modelo regional original marcó AUC=0.998, pero la validación cruzada K-Fold (K=5) confirmó el diagnóstico de fuga de datos: al eliminar la variable contaminada, el AUC cayó a 0.628 (±0.013), revelando que la relación real entre horas suplementarias y nivel salarial es débil. El modelo simulado resultó estable con AUC promedio=0.793 (±0.040). El hallazgo central de la práctica fue que un AUC perfecto es una señal de alarma, no de éxito.
* **🔗 Enlace:** [Ver Tarea APE 15 (ipynb)](https://drive.google.com/file/d/1Uok_8EgxTy8t-ZQbVqWk0I7tsESk3p7Y/view?usp=drive_link)

---

### 🏆 Evaluación Final de Unidad

Examen integrador que consolidó los contenidos de la Unidad 3 mediante un componente centrado en las simulaciones algorítmicas desarrolladas a lo largo de la unidad.

#### 📓 Documento Técnico
* **🗒️ Descripción:** 
* **🔗 Enlace:** [Ver documento del Examen Final]()

---

## ⚠️ Principales Dificultades de la Unidad 3

* **Distinguir ANOVA de comparaciones múltiples t-test:** Al principio no era claro por qué no se podían aplicar múltiples t-tests en lugar de ANOVA. Comprender que hacerlo infla el error Tipo I fue el punto de quiebre conceptual que justificó el uso de Tukey como corrección Post-Hoc.

* **Interpretación del coeficiente de correlación de Pearson vs. causalidad:** Obtener r alto entre dos variables generó la tentación de asumir relación causal. Interiorizar que correlación no implica causalidad, y que el modelo OLS solo cuantifica asociación lineal, requirió revisión cuidadosa de los supuestos del modelo.

* **Diagnóstico de colinealidad con VIF:** Interpretar el Factor de Inflación de la Varianza no fue inmediato. Entender que VIF > 10 indica redundancia entre predictores y distorsiona los coeficientes del modelo fue un aprendizaje técnico nuevo sin referencia previa en las unidades anteriores.

* **Umbral de decisión en Regresión Logística:** El modelo logístico no entrega una clase directamente sino una probabilidad. Decidir el umbral de corte (por defecto 0.5, pero ajustable según el contexto) y su impacto sobre la matriz de confusión fue una de las decisiones más difíciles de justificar técnicamente.

* **Interpretación conjunta de ROC y AUC:** Entender que AUC=0.5 equivale a un clasificador aleatorio y AUC=1.0 a uno perfecto es sencillo, pero interpretar valores intermedios en términos del problema real del dataset de Loja —y decidir si el modelo tiene utilidad práctica— requirió conectar la métrica con el contexto del negocio.

---

## 💡 Conclusión de la Unidad 3

La Unidad 3 demostró que la estadística no termina en la descripción ni en la inferencia: su verdadero poder está en la predicción y la clasificación. El camino recorrido desde el ANOVA —que compara grupos— hasta la curva ROC —que evalúa un clasificador binario— es en realidad un único hilo conductor: cuantificar relaciones entre variables con el mayor rigor posible y comunicar la incertidumbre de cada modelo con honestidad. El dataset del Municipio de Loja, trabajado desde la Unidad 1, llegó a su análisis más complejo aquí, siendo sometido a modelos de regresión y clasificación que en la práctica profesional se usan para tomar decisiones de política pública, asignación de recursos y detección de anomalías.
