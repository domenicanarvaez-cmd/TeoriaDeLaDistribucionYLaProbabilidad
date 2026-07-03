[🔙 Volver a la Portada Principal](PortafolioDigital.md)

# 🚀 UNIDAD 1: Introducción a la Probabilidad. Modelos Probabilísticos
💡 ¡El punto de partida de todo análisis estadístico! Esta unidad estableció las bases para modelar la incertidumbre: desde clasificar variables y calcular probabilidades hasta ajustar distribuciones discretas y continuas a escenarios reales. Todo construido con Python sobre casos prácticos de ingeniería y el dataset regional de Loja.

---

## 🧠 Aprendizaje Práctico Experimental (APE)
Tareas diseñadas para aplicar los conocimientos teóricos en escenarios prácticos y controlados.

> [!NOTE]
> **¿No puedes visualizar los archivos `.ipynb`?**
> Al hacer clic en los enlaces, Google Drive mostrará el mensaje *"No hay ninguna aplicación instalada para abrir este archivo"* o una vista previa vacía. Para abrirlo correctamente, haz clic en el botón **"Abrir con Google Colaboratory"** que aparece en la parte superior de Drive. El notebook se cargará completo con todo el código y las celdas ejecutables.

#### 📊 APE01: Variables Aleatorias y Distribuciones de Probabilidad
* **🗒️ Descripción:** Se modeló la distribución Binomial (n=20, p=0.05) para defectos en manufactura: E[X]=1.0, P(X≤2)=0.9245. En paralelo, tiempo de respuesta de servidor web con Normal (μ=200ms, σ=30ms): P(X<180)=25.25%, percentil 99=269.79ms. Se compararon ambas distribuciones mediante simulación.
* **🔗 Enlace:** [Ver Tarea APE 1 (ipynb)](https://drive.google.com/file/d/1623-7uub8ezbqx8_NNHRPb3SZp_LvW62/view?usp=sharing)

#### 🔔 APE02: Distribuciones Muestrales y Teorema del Límite Central
* **🗒️ Descripción:** Demostración del TLC con distintas distribuciones poblacionales. IC 95% con T de Student para tiempo de exámenes (n=25): [80.87, 89.13] min. IC 95% con Chi-cuadrado para varianza: [60.97, 193.53]. Aplicación práctica: proceso de fabricación de resistencias con IC 99%=[98.43, 100.57Ω] bajo control al contener el valor nominal de 100Ω.
* **🔗 Enlace:** [Ver Tarea APE 2 (ipynb)](https://drive.google.com/file/d/1FWuHLVslDN3iMel0atOaBnoY4UiVXdQx/view?usp=drive_link)

#### 📐 APE03: Variables Aleatorias Discretas y Continuas
* **🗒️ Descripción:** Comparación discreta vs. continua: dado justo (P(X≤3)=0.50) vs. servidor web Normal (percentil 95=249.35ms). Se clasificaron variables reales de la UNL por tipo y distribución. Trabajo autónomo: Uniforme Discreta U(1,8) para balanceo de carga entre servidores, μ=4.5, σ=2.29.
* **🔗 Enlace:** [Ver Tarea APE 3 (ipynb)](https://drive.google.com/file/d/1H8KCojazfIl0bpmV2fybAWmzgp_WsASl/view?usp=drive_link)

#### 📈 APE04: Momentos Estadísticos y Análisis de Tendencia Central con Python
* **🗒️ Descripción:** Momentos estadísticos aplicados al dataset de Loja (n=2,883): remuneración mensual con x̄=$713.81, s²=70,276.27, s=$265.10. Se verificó la distribución Binomial (n=20, p=0.75) con μ=15 y σ²=3.75.
* **🔗 Enlace:** [Ver Tarea APE 4 (ipynb)](https://drive.google.com/file/d/1T9NVgQMiRMq1BzNHao9LiVDBRs1OSN9c/view?usp=drive_link)

#### 🎯 APE05: Distribuciones Discretas Notables
* **🗒️ Descripción:** Binomial para control de calidad de software: P(X≤3)=0.6477. Poisson (λ=4.5) para peticiones erróneas: P(X=6)=0.1281. Aplicado al dataset: λ=30.13 para horas suplementarias. Se demostró la aproximación Binomial→Poisson con diferencia de apenas 6.3×10⁻⁴ entre ambos modelos para P(X=10).
* **🔗 Enlace:** [Ver Tarea APE 5 (ipynb)](https://drive.google.com/file/d/1aUb1xGDv9fkv7p4S7vAAHXwBPzrdHmTB/view?usp=drive_link)

---

## 💡 Conclusión de la Unidad 1
Clasificar correctamente la variable antes de elegir la distribución es el paso más crítico — aplicar el modelo incorrecto invalida cualquier resultado. La diferencia entre discreta (probabilidad en puntos) y continua (área bajo la curva) no es solo conceptual sino operativa. Los parámetros x̄=$713.81 y s=$265.10 del dataset de Loja ya anticipaban la asimetría confirmada en la Unidad 2. La aproximación Binomial→Poisson evidencia que las distribuciones están conectadas, lo que permite elegir el modelo más conveniente sin memorizar fórmulas aisladas.
