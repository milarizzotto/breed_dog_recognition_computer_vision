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
- modelo_resnet18: Variable en memoria que contiene el modelo entrenado.
- conjunto_prueba_perritos: Carpeta de imágenes reales para evaluación.
- anotaciones_perritos: Archivos .txt con anotaciones manuales en formato YOLO.
- anotaciones_yolo: Salida generada automáticamente en formato YOLOv5.
- anotaciones_coco.json: Salida generada automáticamente en formato COCO.
- README.md: Este archivo de instrucciones.

## 📝 Notas
- La aplicación fue diseñada y optimizada para ejecutarse en Google Colab, y validada allí en múltiples etapas.
- La interfaz Gradio se lanza temporalmente mediante share=True, lo cual crea un enlace público válido por tiempo limitado.
- Se recomienda usar el notebook como entorno principal para reproducir y evaluar el sistema completo.
