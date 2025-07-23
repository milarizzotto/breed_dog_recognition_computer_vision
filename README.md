# 🐾 Clasificador de Razas de Perros – Aplicación Gradio

## Descripción

Este proyecto permite identificar perros en imágenes reales y clasificar su raza mediante un sistema de detección y clasificación automática. Utiliza **YOLOv8m** para la detección de objetos y un **modelo ResNet18 entrenado** para la clasificación de razas.

La aplicación fue implementada en **Google Colab**, utilizando Gradio como interfaz interactiva para visualizar resultados en tiempo real.

---

## 🚀 ¿Cómo ejecutar la aplicación?

### Ejecución en Google Colab (Recomendada)

1. Realizá la descarga del notebook presente en este repositorio y abrilo en Google Colab.

2. Ejecutá todas las celdas del notebook.

3. Al llegar al bloque que lanza la aplicación (`gradio_app.launch(share=True)`), se generará un enlace público.

4. Accedé al enlace generado para interactuar con la aplicación Gradio.

---

### Ejecución local (opcional)

Este proyecto no incluye un archivo `app.py`, ya que toda la lógica fue construida dentro del notebook. Sin embargo, si se desea adaptar el sistema para uso local, se pueden migrar las funciones principales a un archivo `.py`.

#### 📦 Instalación de dependencias

```bash
pip install gradio torch torchvision numpy opencv-python pillow faiss-cpu ultralytics
```

## 📁 Estructura del proyecto
- cv_tp_final_rizzotto.ipynb: Notebook principal con todo el desarrollo.
- conjunto_prueba_perritos: Carpeta de imágenes reales para evaluación.
- anotaciones_perritos: Archivos .txt con anotaciones manuales en formato YOLO.
- README.md: Este archivo de instrucciones.
El resto de archivos importantes que son más pesados (como los modelos resultantes, embeddings, índices) se encuentran disponibles [acá](https://drive.google.com/drive/folders/1nI-6aI5QFPqusjmQ_bAEup5IIf-KEsU3?usp=sharing).

## 📝 Notas
- La aplicación fue diseñada y optimizada para ejecutarse en Google Colab, y validada allí en múltiples etapas.
- La interfaz Gradio se lanza temporalmente mediante share=True, lo cual crea un enlace público válido por tiempo limitado.
- Se recomienda usar el notebook como entorno principal para reproducir y evaluar el sistema completo.

---

# 🐾 Dog Breed Classifier – Gradio Application

## Description

This project implements a full pipeline for detecting dogs in real-world images and classifying their breed. It uses **YOLOv8m** for object detection and a fine-tuned **ResNet18 model** for breed classification.

The application was developed entirely within **Google Colab**, and it uses Gradio as an interactive interface for real-time results.

---

## 🚀 How to Run the Application

### ✅ Option 1: Run in Google Colab (Recommended)

1. Download the notebook available in this repository and open it with Google Colab.

2. Run all code cells in order.

3. When reaching the Gradio launch block (`gradio_app.launch(share=True)`), a public link will be generated.

4. Click the generated link to use the interactive application.

---

### ⚙️ Option 2: Run Locally (Optional)

This project does not include a separate `app.py` file since all logic was developed inside the notebook. However, if desired, the core functions can be migrated to a standalone Python script.

#### 📦 Install Dependencies

```bash
pip install gradio torch torchvision numpy opencv-python pillow faiss-cpu ultralytics
```
## 📁 Project Structure
- cv_tp_final_rizzotto.ipynb: Main notebook containing the full pipeline and interface.
- conjunto_prueba_perritos: Folder with test images used for evaluation.
- anotaciones_perritos: YOLO-format .txt annotation files created manually.
- README.md: This instruction file.
The rest of the files that are important but big in size (like final models, embeddings) had to be uploaded in Google Drive. Available [here](https://drive.google.com/drive/folders/1nI-6aI5QFPqusjmQ_bAEup5IIf-KEsU3?usp=sharing).

## 📝 Notes
- The application is designed and validated entirely within Google Colab.
- Gradio launches a temporary public link using share=True, accessible for a limited time.
- For reproducibility and testing, running the notebook directly is recommended.
