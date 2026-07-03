[🔙 Volver a la Portada Principal](PortafolioDigital.md)

# 📊 UNIDAD 2: Grupos de Variables Aleatorias. Funciones de una Variable Aleatoria

🔍 ¡De la teoría a la decisión! Esta unidad fue clave para comprender cómo los datos reales —aunque imperfectos y asimétricos— pueden someterse a un análisis inferencial riguroso. A través del dataset regional de Remuneraciones del Municipio de Loja, se recorrió el camino completo de la estadística inferencial: desde modelar una distribución, validar supuestos, estimar parámetros y finalmente tomar decisiones formales con evidencia estadística.

---

## 🧠 Aprendizaje Práctico Experimental (APE)

Tareas diseñadas para aplicar los conocimientos teóricos en escenarios prácticos y controlados.

#### 🔔 APE07: Distribuciones Continuas Notables
* **🗒️ Descripción:** Se trabajó la distribución Normal sobre el dataset de Loja: el 83.08% de servidores gana entre $460 y $4.144 bajo supuesto de normalidad, pero el test de Shapiro-Wilk (W=0.5988, p=3.22×10⁻⁶³) rechazó esa normalidad, con asimetría de 3.75 causada por sueldos directivos.
* **🔗 Enlace:** [Ver Tarea APE 7 (ipynb)](https://drive.google.com/file/d/1c2GUKk6Jnk8Qd-goSLBKLJ-Q1asWfuLw/view?usp=drive_link)

#### 🔁 APE08: Distribuciones Muestrales y TLC mediante Simulación Estocástica
* **🗒️ Descripción:** Se demostró computacionalmente el Teorema del Límite Central: 1.000 muestras de una distribución asimétrica convergen a una campana normal. Replicado con bootstrapping sobre el dataset real (n=40, 500 muestras). También se analizó que para reducir el error estándar a la mitad, hay que cuadruplicar n.
* **🔗 Enlace:** [Ver Tarea APE 8 (ipynb)](https://drive.google.com/file/d/168E2DfgsJZEsA2AEV2OOO0zy6YCVmfsI/view?usp=drive_link)

#### 📏 APE09: Estimación de Parámetros e Intervalos de Confianza (Z y T de Student
* **🗒️ Descripción:** Se construyeron intervalos de confianza para la remuneración promedio con distribuciones Z y T. A mayor nivel de confianza, mayor margen de error: 80%→±$343, 90%→±$442, 95%→±$528, 99%→±$699. El 95% es el estándar por su equilibrio entre seguridad y precisión.
* **🔗 Enlace:** [Ver Tarea APE 9 (ipynb)](https://drive.google.com/file/d/1iNJ0ndKJ25hYlaJCI6hnOvPIFf3RPIni/view?usp=drive_link)

#### 🧪 APE10: Pruebas de Hipótesis Paramétricas (Z y T) y Análisis del Valor-p
* **🗒️ Descripción:** Se aplicaron pruebas Z y T unimuestrales al dataset. Con H₀: μ=$1.200, el valor-p≈0 rechazó H₀ contundentemente. Se trabajó la interpretación correcta del valor-p y el fenómeno Big Data: con n grande, diferencias mínimas resultan significativas estadísticamente aunque sean irrelevantes en la práctica.
* **🔗 Enlace:** [Ver Tarea APE 10 (ipynb)](https://drive.google.com/file/d/1SYMwx0MR6yJ2BgNDBka4Xbq56MarFRKf/view?usp=drive_link)

---

### 🏆 Evaluación Final de Unidad
Examen integrador que consolidó los contenidos de la Unidad 2 en dos componentes: una prueba de hipótesis unimuestral (T de Student) y un A/B Testing con comparación de grupos independientes, ambos aplicados al dataset regional de Loja usando `scipy.stat`.

#### **📓 Componente 1 — Documento Técnico (Jupyter Notebook)**
* **🗒️ Descripción:** Notebook de examen con prueba T unimuestral (H₀: μ=$1.200, rechazada con t=−98.47 y p≈0) y A/B Testing entre servidores con y sin horas suplementarias y extraordinarias (T de Welch + Mann-Whitney U + d de Cohen=0.61, efecto mediano). Código documentado con comentarios en cada bloque y teoría en LaTeX dentro de celdas Markdown.
* **🔗 Enlace:** [Ver Notebook del Examen Final (ipynb)](https://drive.google.com/file/d/1OHwjdN56P5cCQJrxm04Azzeh3_cm8ygH/view?usp=drive_link)

#### 🎬 Componente 2 — Video de Defensa
* **🗒️ Descripción:** Video de defensa oral (6–8 minutos) explicando el criterio de selección de la prueba T de Student, la ejecución en vivo del código y la interpretación del valor-p aplicado al problema regional.
* **🔗 Enlace:** [Ver Video de Defensa](https://drive.google.com/file/d/18tvvjDGCM9DKWZvm-p3KVo3drlYFOSgR/view?usp=drive_link)
* **🔗 Enlace:** [Ver Diapositivas](https://drive.google.com/file/d/1H4MWnYvfRuUkrtVlumPrRjSvxJbReL3L/view?usp=drive_link)

---

## 💡 **Conclusión de la Unidad 2**
La asimetría severa del dataset no impidió la inferencia gracias al TLC. El valor-p no es la probabilidad de que H₀ sea cierta, sino la probabilidad de obtener datos tan extremos asumiendo que H₀ es verdadera. Con casi 3.000 registros, cualquier diferencia produce p≈0, por lo que el coeficiente d de Cohen fue clave para distinguir significancia estadística de significancia práctica. Los cuatro APE formaron un análisis completo y coherente: describir → validar → estimar → decidir, todo aplicado al mismo dataset regional.
