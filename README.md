# Optuna y Ray Tune ML

Este proyecto entrena un modelo Random Forest para la clasificación del dataset de Disease Prediction Using Machine Learning utilizando métodos de optimización como Optuna y Ray Tune para encontrar la mejor combinación de hiperparámetros y se compara el rendimiento obtenido para los hiperparámetros encontrados por cada método.

## 📋 Descripción

El proyecto incluye:
- **Jupyter Notebook**: Notebook con el código en Python que entrena un modelo Random Forest con el dataset de Disease Prediction Using Machine Learning y utilizando métodos de optimización como Optuna y Ray Tune para encontrar la mejor combinación de hiperparámetros

## 📋 Objetivo

Desarrollar y optimizar un modelo de aprendizaje automático capaz de predecir la probabilidad de que un paciente desarrolle una enfermedad crónica, utilizando técnicas avanzadas de ajuste de hiperparámetros con Optuna y Ray Tune.

## 🚀 Estructura del Proyecto

```
├── Aplicación_Optuna_y_Ray_Tune.ipynb      # Jupyter Notebook
└── README.md          # Este archivo
```

## 📚 Tecnologías Utilizadas

- **Python 3.x**
- **scikit-learn**: Machine Learning
- **pandas**: Manipulación de datos
- **optuna**: Optimización automática de hiperparámetros en modelos de aprendizaje automático
- **ray**: Optimización automática de hiperparámetros y ejecución de aplicaciones en paralelo y de forma distribuida
- **time**: Manipulación de fechas y horas

## 📝 Notas

- El modelo Random Forest fue entrenado con 80% del dataset completo de Disease Prediction Using Machine Learning (3969 muestras)
- Este proyecto es con fines educativos y demostrativos

## 📝 Reflexiones de lo aprendido

Métodos de optimización como Optuna y Ray Tune permiten de forma automatizada encontrar las mejores combinaciones de hiperparámetros al generar múltiples combinaciones de prueba para el modelo que se quiera probar. Ray Tune permite escalar el proceso de optimización en entornos distribuidos, lo cual es útil para problemas grandes y complejos. Al distribuir la carga de trabajo y gracias a la paralelización es posible obtener menores tiempos de ejecución. En este estudio para el diagnóstico de enfermedades, se observa que tanto para la optimización con Optuna como con Ray Tune, para múltiples combinaciones de hiperparámetros, se obtienen muy buenos modelos de Random Forest que consiguen clasificar correctamente el 100% de los datos de validación, es decir, identificar bien las enfermedades a las que corresponden los síntomas presentes en el conjunto de prueba.

Una posible desventaja de Ray Tune es que al ser un método de optimización más complejo, no es recomendable para equipos de trabajo con poca experiencia, dado que para aprovechar la paralelización se requiere contar con conocimientos más avanzados de configuración en computación distribuida y para el mantenimiento de nodos o clústeres. Por lo tanto, para estos equipos de trabajo, podría ser más recomendable utilizar un método de optimización como Optuna, más simple de entender y configurar.