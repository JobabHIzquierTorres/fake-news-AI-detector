# fake-news-AI-detector
Clasificador de NLP utilizando Regresión Logística para la detección de noticias falsas en textos y artículos de prensa.

Este proyecto consiste en un modelo de **Machine Learning (Aprendizaje Supervisado)** capaz de clasificar noticias y determinar si son reales o falsas (*fake news*). El desarrollo se ha realizado utilizando procesamiento de lenguaje natural (NLP) para la limpieza del texto y un modelo de clasificación binaria.

---

## ⚙️ Marco Teórico Matemático

El proceso que sigue el modelo para la clasificación de las noticias está basado en las siguientes funciones matemáticas:

* **A)** **Función hipótesis (sigmoide):**  
  ![hipotesis.jpeg](https://raw.githubusercontent.com/JobabHIzquierTorres/fake-news-AI-detector/main/imgs/hipotesis.jpeg)
  
* **B)** **Función de Coste ($y = 1$ y $y = 0$):**  
  ![coste.jpeg](https://raw.githubusercontent.com/JobabHIzquierTorres/fake-news-AI-detector/main/imgs/coste.jpeg)
  
* **C)** **Función de Optimización:**  
  ![optimizacion.jpeg](https://raw.githubusercontent.com/JobabHIzquierTorres/fake-news-AI-detector/main/imgs/optimizacion.jpeg)

---

## 📊  Conjunto de Datos

Los datos han sido obtenidos de la plataforma **Kaggle**. El dataset consta de dos archivos en formato CSV:
* `True.csv`: Contiene noticias reales y verificadas.
* `Fake.csv`: Contiene noticias identificadas como falsas (*fake news*).

### ⚠️ Nota importante sobre la descarga de datos

Debido al límite de tamaño para la subida de archivos en GitHub (los datasets pesan más de lo permitido), **los archivos `True.csv` y `Fake.csv` no se encuentran dentro de este repositorio**. 

Para ejecutar el proyecto, deberás descargarlos manualmente siguiendo estos pasos:

1. Entra al dataset en Kaggle: [Fake and Real News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset).
2. Descarga el archivo ZIP presionando el botón **"Download"** (requiere cuenta gratuita en Kaggle).
3. Descomprime el archivo y coloca los ficheros `True.csv` y `Fake.csv` dentro de la carpeta `data/` en la raíz de tu proyecto local para que el código funcione sin modificar las rutas.

---

## 🛠️ Tecnologías y Librerías Utilizadas

El entorno se ha desarrollado con **Python** y las siguientes herramientas principales:
* **Procesamiento de Datos:** `pandas`
* **Limpieza de Texto y NLP:** `nltk` (tokenización, stopwords y stemming), `beautifulsoup4` (limpieza de marcado HTML), `re` y `string`.
* **Modelado y Métricas:** `scikit-learn` (`CountVectorizer`, `LogisticRegression`, `accuracy_score`).

---

## 💻 Instalación y Uso

Si deseas clonar este repositorio y ejecutarlo en tu entorno local, sigue estos pasos:

1. **Clona el repositorio:**
   ```bash
   git clone [https://github.com/JobabHIzquierTorres/fake-news-AI-detector.git](https://github.com/JobabHIzquierTorres/fake-news-AI-detector.git)
   cd fake-news-AI-detector

2. **Instala las dependencias necesarias:**
   ```bash
   pip install -r requirements.txt

3. **Ejecuta el cuaderno:**
   * Abre el archivo ipynb usando Jupyter Notebook, VS Code o súbelo directamente a Google Colab.
  
---

## 📄 Licencia

Este proyecto está bajo la **Licencia MIT**. Siéntete libre de usar, modificar y distribuir el código respetando los términos de la licencia.
