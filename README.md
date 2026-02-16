# **Diseño de Cámaras y Pilares (Room & Pillar)**

El objetivo principal de este proyecto es demostrar cómo interactúan las variables matemáticas y geológicas en el diseño de una mina subterránea mediante el método de **Room & Pillar** (Cámaras y Pilares). A través de scripts en Python y un simulador interactivo, el usuario puede visualizar el delicado balance entre la seguridad operativa (Factor de Seguridad) y la rentabilidad (porcentaje de recuperación de mineral).

## Enfoque:
El notebook guía al usuario paso a paso para comprender:
* El cálculo de esfuerzos litostáticos basados en la profundidad.
* La estimación dinámica de la resistencia del macizo rocoso utilizando el **Criterio de Falla de Hoek-Brown (2002)** (GSI y UCS).
* La aplicación de la **Teoría del Área Tributaria** para determinar cargas sobre pilares.
* La validación geométrica de la luz máxima en las intersecciones para prevenir el colapso del techo.

## ⚠️ Limitaciones del Modelo (Aviso Importante)
**Este material es estrictamente un ejercicio académico y didáctico.** No debe ser utilizado como base para el diseño, planeación técnica, ni ejecución de operaciones mineras en el mundo real. 

Para mantener la claridad pedagógica, el modelo analítico implementado en este código hace simplificaciones significativas:
* **Medio Continuo:** El simulador asume un macizo rocoso homogéneo e isotrópico. No evalúa el control estructural discreto (fallas mayores, formación de cuñas o familias de diaclasas persistentes) que comúnmente dictan la estabilidad en la realidad.
* **Geometría Idealizada:** Asume cuerpos mineralizados (mantos) perfectamente horizontales y pilares cuadrados sometidos a carga uniforme. No considera buzamientos (manteos) topográficos, geometría irregular, ni redistribución de esfuerzos 3D por tajeos adyacentes.
* **Cargas Estáticas:** El código ignora factores dinámicos cruciales como la sismicidad inducida, el daño por voladura y la deformación de la roca dependiente del tiempo (creep o fluencia).
* **Ausencia de Sostenimiento:** Las simulaciones no contemplan el uso de soporte artificial (anclaje sistemático, mallas, shotcrete).

Cualquier diseño minero real y seguro requiere campañas de perforación, mapeo geomecánico en campo, ensayos mecánicos de laboratorio y modelación numérica tridimensional avanzada.

## 🚀 Cómo utilizar este notebook
Para correr este simulador necesitas tener instalado Python 3.x junto con las siguientes librerías:
* `numpy`
* `pandas`
* `matplotlib`
* `ipywidgets` (Para habilitar el simulador interactivo)
