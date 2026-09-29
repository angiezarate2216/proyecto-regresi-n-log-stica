# Proyecto Regresión Logística
Proyecto desarrollado para el CADI de Machine Learning, donde se busca crear un conjunto de datos que permitan el uso y aplicación del modelo de Regresión Logística. Dentro de este repositorio se encontrará el notebook creado paso a paso para el cumplimiento del proceso y su análisis.
---

**Autora:** Angie Alejandra Chipatecua Zarate  
**CADI:** Introducción a Machine Learning
**Institución:** Universidad De Cundinamarca
**Fecha:** Septiembre de 2026  

---

## Descripción del Proyecto

Este repositorio contiene el desarrollo técnico y analítico de un modelo de **Machine Learning Supervisado** utilizando **Regresión Logística** para automatizar la evaluación y aprobación de solicitudes de crédito financiero.

El modelo procesa simultáneamente tres variables  (`ingresos_mensuales`, `puntaje_credito` y `antiguedad_laboral`) para determinar si una solicitud debe ser **Aprobada (1)** o **Rechazada (0)**.

---

## Función y Estructura del Código

El cuaderno de Google Colab realiza el siguiente flujo de trabajo completo:

1. **Carga y Estructuración de Datos:** Creación del `DataFrame` en Pandas con la información financiera en pesos colombianos (COP). Este conjunto de datos se generó manualmente.
2. **Análisis Exploratorio de Datos (EDA):** Generación de gráficos de dispersión (*Scatter Plots*) con Matplotlib para evaluar visualmente la separabilidad de las clases.
3. **División de Datos (Train/Test):** Separación en $75\%$ para entrenamiento y $25\%$ para prueba, utilizando estratificación (`stratify=y`) para preservar el balance de clases.
4. **Entrenamiento del Modelo:** Ajuste del algoritmo de `LogisticRegression` de Scikit-learn.
5. **Generación de Predicciones y Probabilidades:** Evaluación de salidas categóricas con `predict()` y probabilidades continuas con `predict_proba()`.
6. **Métricas de Evaluación:** Generación de la Matriz de Confusión, Exactitud (*Accuracy*), Precisión, *Recall* y prueba de ajuste dinámico de umbrales de decisión.

---

## Cómo Abrir y Ejecutar el Código en Google Colab

Para visualizar y ejecutar el código sin necesidad de instalar entornos locales, puedes usar cualquiera de estas dos opciones:

### Opción 1: Abrir directamente en Google Colab (Recomendado)

1. Ingresa a Google Colab.
2. Inicia sesión con tu cuenta de Google.
3. En la ventana emergente, selecciona la pestaña **GitHub** o **Subir**:
   * **Desde GitHub:** Pega el enlace de este repositorio y selecciona el archivo `.ipynb`.
   * **Desde tu equipo:** Si descargaste el archivo `.ipynb`, ve a la pestaña **Subir** y arrastra el archivo.

---

### Opción 2: Abrir desde Google Drive

1. Sube el archivo con extensión `.ipynb` a tu unidad de **Google Drive**.
2. Haz clic derecho sobre el archivo subido.
3. Selecciona **Abrir con** ➔ **Google Colaboratory**.

---

## Instrucciones para Ejecutar el Cuaderno

Una vez abierto el cuaderno en Google Colab:

1. **Asegurar el entorno de ejecución:** Ve al menú superior en `Entorno de ejecución` ➔ `Cambiar tipo de entorno de ejecución` y verifica que esté seleccionado **Python 3**.
2. **Ejecutar todo el código:** Dirígete al menú `Entorno de ejecución` ➔ **Ejecutar todas**.
3. **Ejecución celda por celda:** Puedes ejecutar cada bloque individualmente haciendo clic en el botón de **Play** a la izquierda de cada celda.

> **Nota:** El código utiliza librerías estándar de Python (`pandas`, `numpy`, `matplotlib`, `scikit-learn`), las cuales vienen preinstaladas en Google Colab, por lo que **no se requiere la instalación de dependencias adicionales**.

---
## NOTA 
Este cuaderno y explicación solo aplica para entornos en línea (los más usados en Google Colab), no entornos en la nube, por lo que si lo requieres será necesario investigar.

