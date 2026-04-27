# 🎲 Simulación Montecarlo: Juego de Yahtzee

Este repositorio contiene la implementación y el análisis estadístico del juego **Yahtzee** para dos jugadores. El proyecto fue desarrollado en un entorno de **Google Colab** y utiliza el **Método de Montecarlo** para evaluar el rendimiento de una estrategia de juego automatizada.

## 📄 Descripción del Proyecto
El objetivo principal es aplicar conceptos de simulación para comprender cómo la aleatoriedad influye en los resultados de un juego de reglas complejas. El programa simula 13 rondas de juego por cada jugador, aplicando una estrategia de "bloqueo de dados" basada en la frecuencia de los valores obtenidos en cada lanzamiento.

### Características principales:
* **Generación Aleatoria:** Uso de una distribución uniforme para el lanzamiento de 5 dados convencionales.
* **Lógica de Juego:** Evaluación automática de jugadas (Tercia, Full House, Póker, Escaleras y Yahtzee).
* **Simulación Masiva:** Motor de Montecarlo capaz de ejecutar miles de iteraciones para obtener datos significativos.
* **Análisis Estadístico:** Cálculo de la media de puntajes, desviación estándar y tasa de éxito (victorias).

## 🛠️ Requisitos 
El proyecto está diseñado para ejecutarse en Python 3. Se requieren las siguientes librerías:
* `matplotlib`: Para la visualización de histogramas.
* `collections`: Para el procesamiento de frecuencias de los dados.
* `random`: Para la generación de números aleatorios.


## 🚀 Cómo utilizar el Notebook
1. Carga el archivo `SimulaciónEA1Principal.ipynb` en **Google Colab**.
2. Ejecuta las celdas iniciales para definir las funciones de lógica y puntuación.
3. Utiliza la función `simular_montecarlo(iteraciones=N)` para iniciar el experimento.
4. Observa el histograma generado al final para analizar la distribución de los puntajes.

## 📊 Resultados Obtenidos
La simulación permite observar la **Ley de los Grandes Números** en acción:
* **Histograma:** Los resultados tienden a formar una campana de Gauss, centrada en el puntaje promedio esperado.
* **Probabilidad:** El sistema calcula el porcentaje de victorias del Jugador 1 frente al Jugador 2 tras $N$ juegos, validando la equidad del modelo o el impacto de la estrategia.

