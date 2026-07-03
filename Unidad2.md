[🔙 Volver a la Portada Principal](PortafolioDigital.md)

# 📊 UNIDAD 2: Grupos de Variables Aleatorias. Funciones de una Variable Aleatoria

🔍 ¡De la teoría a la decisión! Esta unidad fue clave para comprender cómo los datos reales —aunque imperfectos y asimétricos— pueden someterse a un análisis inferencial riguroso. A través del dataset regional de Remuneraciones del Municipio de Loja, se recorrió el camino completo de la estadística inferencial: desde modelar una distribución, validar supuestos, estimar parámetros y finalmente tomar decisiones formales con evidencia estadística.

---

## 🧠 Aprendizaje Práctico Experimental (APE)

Tareas diseñadas para aplicar los conocimientos teóricos en escenarios prácticos y controlados.

#### 🔔 APE07: Distribuciones Continuas Notables
* **🗒️ Descripción:** Introducción a las distribuciones continuas más importantes, con énfasis en la distribución Normal (Gaussiana). Se trabajó la función de densidad de probabilidad (PDF), el cálculo de probabilidades acumuladas y la estandarización mediante el puntaje Z. Aplicado al dataset de Loja, se estimó que el 83.08% de los servidores gana entre $460 y $4.144 bajo el supuesto de normalidad. Sin embargo, el test de Shapiro-Wilk (W=0.5988, p=3.22×10⁻⁶³) y el gráfico Q-Q demostraron que los datos reales no siguen una distribución normal, con una asimetría de 3.75 causada por los sueldos de cargos directivos.
* **🔗 Enlace:** [Ver Tarea APE 7 (ipynb)](https://drive.google.com/file/d/1c2GUKk6Jnk8Qd-goSLBKLJ-Q1asWfuLw/view?usp=drive_link)

#### 🔁 APE08: Distribuciones Muestrales y TLC mediante Simulación Estocástica
* **🗒️ Descripción:** Estudio y demostración computacional del Teorema del Límite Central como puente entre datos individuales no normales y medias muestrales normales. Se generaron 1.000 muestras de una distribución exponencial (asimétrica) y se demostró que sus medias convergen a una campana normal, con una media poblacional de 1.9919 vs. media de muestras de 1.9923 (diferencia de 0.0004). Replicado con bootstrapping sobre el dataset real de Loja (n=40, 500 muestras), confirmando la convergencia a pesar de la asimetría original de 3.75. También se analizó el Error Estándar y su relación no lineal con n: para reducirlo a la mitad, hay que cuadruplicar el tamaño de muestra.
* **🔗 Enlace:** [Ver Tarea APE 8 (ipynb)](https://drive.google.com/file/d/168E2DfgsJZEsA2AEV2OOO0zy6YCVmfsI/view?usp=drive_link)

#### 📏 APE09: Estimación de Parámetros e Intervalos de Confianza (Z y T de Student
* **🗒️ Descripción:** Construcción de intervalos de confianza para la remuneración promedio del Municipio de Loja usando distribución Z (muestras grandes, σ conocida) y T de Student (muestras pequeñas, σ desconocida). Se exploró el trade-off entre nivel de confianza y margen de error sobre el dataset real: al 80% el margen fue ±$343.24, al 90% fue ±$441.74, al 95% fue ±$527.89 y al 99% fue ±$698.74. El análisis demostró que exigir mayor confianza tiene un costo directo en precisión, justificando el 95% como estándar de la industria por su equilibrio entre seguridad estadística y utilidad práctica.
* **🔗 Enlace:** [Ver Tarea APE 9 (ipynb)](https://drive.google.com/file/d/1iNJ0ndKJ25hYlaJCI6hnOvPIFf3RPIni/view?usp=drive_link)

#### 🧪 APE10: Pruebas de Hipótesis Paramétricas (Z y T) y Análisis del Valor-p
* **🗒️ Descripción:** Implementación formal de pruebas de hipótesis Z y T de Student para una muestra, aplicadas al dataset regional. Se planteó la hipótesis nula de que la remuneración promedio es de $1.200 (referente del sector público ecuatoriano), obteniendo un valor-p prácticamente cero que llevó a rechazar H₀ con contundencia. Se trabajaron los conceptos de Error Tipo I y Tipo II, la interpretación correcta del valor-p (no es la probabilidad de que H₀ sea cierta), y el fenómeno del Big Data: con muestras grandes, diferencias mínimas e irrelevantes resultan estadísticamente significativas, lo que obliga a distinguir entre significancia estadística y significancia práctica.
* **🔗 Enlace:** [Ver Tarea APE 10 (ipynb)](https://drive.google.com/file/d/1SYMwx0MR6yJ2BgNDBka4Xbq56MarFRKf/view?usp=drive_link)

---

### 🏆 Evaluación Final de Unidad
Examen integrador que consolidó los contenidos de la Unidad 2 en dos componentes: una prueba de hipótesis unimuestral (T de Student) y un A/B Testing con comparación de grupos independientes, ambos aplicados al dataset regional de Loja usando `scipy.stat`.

#### **📓 Componente 1 — Documento Técnico (Jupyter Notebook)**
* **🗒️ Descripción:** Notebook de examen con prueba T unimuestral (H₀: μ=$1.200, rechazada con t=−98.47 y p≈0) y A/B Testing entre servidores con y sin horas suplementarias y extraordinarias (T de Welch + Mann-Whitney U + d de Cohen=0.61, efecto mediano). Código documentado con comentarios en cada bloque y teoría en LaTeX dentro de celdas Markdown.
* **🔗 Enlace:** [Ver Notebook del Examen Final (ipynb)](https://drive.google.com/file/d/1OHwjdN56P5cCQJrxm04Azzeh3_cm8ygH/view?usp=drive_link)

### 🎬 Componente 2 — Video de Defensa
* **🗒️ Descripción:** Video de defensa oral (6–8 minutos) explicando el criterio de selección de la prueba T de Student, la ejecución en vivo del código y la interpretación del valor-p aplicado al problema regional.
* **🔗 Enlace:** [Ver Video de Defensa](https://drive.google.com/file/d/18tvvjDGCM9DKWZvm-p3KVo3drlYFOSgR/view?usp=drive_link)
* **🔗 Enlace:** [Ver Diapositivas](https://drive.google.com/file/d/1H4MWnYvfRuUkrtVlumPrRjSvxJbReL3L/view?usp=drive_link)

---

##💡 **Conclusiones de la Unidad 2**
* **El dato imperfecto no impide la inferencia.** El hallazgo más importante de la unidad fue que los sueldos del Municipio de Loja son profundamente asimétricos (skewness = 3.75) y no normales, pero el Teorema del Límite Central permitió igualmente construir toda la inferencia estadística sobre ellos. La lección práctica es que la estadística no exige datos perfectos: exige herramientas adecuadas para la realidad tal como es.
* **El valor-p tiene una definición exacta que no debe confundirse.** A lo largo de la unidad quedó claro que el valor-p no es la probabilidad de que la hipótesis nula sea cierta, sino la probabilidad de obtener un resultado igual o más extremo al observado asumiendo que H₀ es verdadera. Comprender esta distinción fue uno de los aprendizajes más importantes y evita uno de los errores más frecuentes en estadística aplicada.
* **Significancia estadística no es lo mismo que significancia práctica.** Con un dataset de casi 3.000 registros, cualquier diferencia mínima produce un valor-p cercano a cero. El coeficiente d de Cohen fue la herramienta que permitió ir más allá del valor-p y cuantificar si la diferencia detectada entre los grupos realmente importa en el contexto real de las políticas salariales del municipio. Ese es el matiz más valioso de toda la unidad.
* **El hilo conductor de los cuatro APE formó un análisis completo.** Describir los datos con la Normal (APE 06) → validar que las medias muestrales son normales gracias al TLC (APE 07) → estimar con intervalos de confianza (APE 08) → tomar decisiones formales con pruebas de hipótesis (APE 09) es exactamente el camino que sigue cualquier análisis estadístico real. Ver ese proceso completo aplicado al mismo dataset regional desde el inicio hasta el examen final fue lo que le dio coherencia y profundidad a esta unidad.
