[🔙 Volver a la Portada Principal](README.md)

# 🔢 UNIDAD 3: Ley de Grandes Números

🧩 ¡Del análisis al modelo! Esta unidad representa el cierre del ciclo estadístico: partiendo de los fundamentos del TLC y las distribuciones muestrales, se avanzó hacia la comparación multigrupo, el análisis de relaciones entre variables y la construcción de modelos predictivos y clasificadores. Cada APE añadió una herramienta nueva al arsenal analístico, siempre anclada al dataset real del Proyecto Integrador.

---

## 🧠 Aprendizaje Práctico Experimental (APE)

Tareas diseñadas para aplicar los conocimientos teóricos en escenarios prácticos y controlados.

> [!NOTE]
> **¿No puedes visualizar los archivos `.ipynb`?**
> Al hacer clic en los enlaces, Google Drive mostrará el mensaje *"No hay ninguna aplicación instalada para abrir este archivo"* o una vista previa vacía. Para abrirlo correctamente, haz clic en el botón **"Abrir con Google Colaboratory"** que aparece en la parte superior de Drive. El notebook se cargará completo con todo el código y las celdas ejecutables.

---

#### 🔬 APE11: Inferencia Estadística Multigrupo: ANOVA de 1 Factor y Pruebas Post-Hoc (Tukey)
* **🗒️ Descripción:** 
* **🔗 Enlace:** [Ver Tarea APE 11 (ipynb)](https://drive.google.com/file/d/1GD_CrDPQ25xeo3stS4s__1xq7HEKTPyk/view?usp=drive_link)

#### 📉 APE12: Análisis Bivariado y Predicción: Correlación de Pearson y Regresión Lineal Simple (OLS)
* **🗒️ Descripción:** 
* **🔗 Enlace:** [Ver Tarea APE 12 (ipynb)](https://drive.google.com/file/d/1OjOjrxRhsIVa0dcc84VE0SiMaGj5Nu-E/view?usp=drive_link)

#### 📊 APE13: Análisis Predictivo Multivariado: Regresión Lineal Múltiple y VIF
* **🗒️ Descripción:** 
* **🔗 Enlace:** [Ver Tarea APE 13 (ipynb)](https://drive.google.com/file/d/1cpI5ZiOF_AIJYvq-3UYfGJmg2qeQc5TO/view?usp=sharing)

#### 🎲 APE14: Modelado Probabilístico Avanzado: Regresión Logística y Matrices de Confusión
* **🗒️ Descripción:** 
* **🔗 Enlace:** [Ver Tarea APE 14 (ipynb)](https://drive.google.com/file/d/1dhIZL5A6k8xake0hJOLHHeMRlnp_rhZw/view?usp=drive_link)

#### 📈 APE15: Evaluación Avanzada de Modelos: ROC, AUC y Validación Cruzada K-Fold
* **🗒️ Descripción:** 
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
