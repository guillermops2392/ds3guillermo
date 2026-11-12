Documentación del Entregable

1. Justificación del Modelo Elegido
Regresión Logística: Se seleccionó porque funciona excepcionalmente bien en representaciones dispersas de alta dimensionalidad como las de TF-IDF. Al trabajar con texto linealmente separable, suele ser superior a clasificadores basados en conteo simple.
Multinomial Naive Bayes: Se incluyó como un baseline estadístico clásico para tareas de procesamiento de lenguaje natural debido a su altísima velocidad de cómputo y buen rendimiento inicial.

3. Análisis Preliminar (Matriz de Confusión)
Basándonos en los resultados de entrenamiento y prueba:
Categorías más fáciles de predecir: Sports es la categoría más fuerte con un F1-score de 0.96 (Naive Bayes) / 0.95 (Regresión Logística), seguida de World con 0.90.
Categorías con mayor confusión: El solapamiento más importante se da entre Business y Sci_Tech (ambas rondando el 0.85-0.87 de F1-score). Esto se debe a que la terminología de empresas de tecnología, cotizaciones de mercado tecnológico, lanzamientos de software corporativo y finanzas empresariales a menudo comparten palabras clave comunes.

3. Requerimientos de Entorno 
pandas==2.0.3
scikit-learn==1.2.2
nltk==3.8.1
matplotlib==3.7.1
seaborn==0.12.2
