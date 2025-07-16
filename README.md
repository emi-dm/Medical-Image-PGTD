# Medical Image-PGTD 🩺🖼️


## 📝 Descripción de la formación y cuadernos

Esta formación está diseñada para proporcionar una experiencia práctica y progresiva en el procesamiento y análisis de imágenes médicas utilizando MONAI y PyTorch. A través de una serie de notebooks, el participante aprenderá desde los fundamentos hasta técnicas avanzadas de segmentación, integración con Hugging Face y automatización de pipelines. Cada notebook aborda un aspecto clave del flujo de trabajo en imágenes médicas, permitiendo adquirir competencias aplicables tanto en investigación como en desarrollo clínico.

### Estructura de la formación

#### Día 1

- **Intro to MONAI.ipynb**: Introducción al framework MONAI, su arquitectura, filosofía de diseño y componentes principales. Incluye ejemplos prácticos de transforms, datasets, caché y redes, así como buenas prácticas para reproducibilidad y eficiencia en deep learning médico.
- **hugging_face_pipeline_for_monai.ipynb**: Integración de modelos de segmentación de MONAI en pipelines de Hugging Face. Explica cómo envolver un modelo MONAI en una pipeline compatible con Transformers, facilitando la reutilización y despliegue de modelos en aplicaciones clínicas y de investigación.
- **finetune_vista3d_for_hugging_face_pipeline.ipynb**: Ajuste fino de un modelo VISTA3D preentrenado con datos específicos (bazo) y su integración en una pipeline de Hugging Face. Incluye descarga y preparación de datos, entrenamiento, evaluación y comparación entre el modelo base y el ajustado.
- **inverse_transforms_and_test_time_augmentations.ipynb**: Demostración del uso de transformaciones invertibles y aumentaciones en tiempo de prueba. Enseña cómo aplicar y revertir transforms, así como técnicas de Test Time Augmentation para mejorar la robustez y evaluación de modelos.
- **Auto3DSeg Hello World.ipynb**: Ejemplo práctico de Auto3DSeg, la solución automatizada de MONAI para segmentación 3D. Muestra cómo configurar datasets simulados, ejecutar el pipeline AutoRunner y analizar predicciones, con un enfoque en la facilidad de uso y la modularidad.

#### Día 2

- **spleen_segmentation_3d.ipynb**: Ejemplo completo de segmentación 3D del bazo usando MONAI y PyTorch. Se cubren transforms para datos médicos, carga y preprocesamiento de imágenes NIfTI, entrenamiento y validación de un modelo UNet 3D, y evaluación de resultados en imágenes reales del Medical Decathlon.

Esta secuencia de notebooks permite al participante avanzar desde los conceptos básicos hasta la automatización avanzada, cubriendo todo el ciclo de vida de un proyecto de deep learning en imágenes médicas.

---

> **Nota:** Esta formación forma parte del curso de procesamiento de imagen del PGTD.

MedicalImage-PGTD es una parte de la formación profesional orientada al procesamiento, gestión y análisis de imágenes. Su objetivo es facilitar la adquisición de conocimiento para el manejo eficiente de datos médicos visuales, apoyando tareas de investigación y desarrollo clínico.

## 🚀 Características principales

- Procesamiento avanzado de imágenes médicas 2D y 3D.
- Gestión centralizada y eficiente de archivos y metadatos.
- Arquitectura modular, extensible y fácil de mantener.
- Ejemplos y notebooks didácticos para autoaprendizaje.
- Pruebas unitarias integradas para garantizar la calidad del código.

## 📦 Instalación

Este proyecto utiliza [uv](https://github.com/astral-sh/uv) para la gestión de dependencias, asegurando un entorno reproducible y seguro. Se recomienda trabajar en un entorno virtual limpio.

### Requisitos previos

- Python 3.11 o superior
- [uv](https://github.com/astral-sh/uv) instalado

#### Instalación de uv

**Linux/macOS:**
```sh
curl -Ls https://astral.sh/uv/install.sh | sh
```

**Windows (PowerShell):**
```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### Instalación de dependencias

En la raíz del proyecto, ejecuta:

```sh
uv sync
```

> 💡 En Windows, asegúrate de ejecutar el comando en PowerShell o CMD.


## 🛠️ Uso

1. Abre VSCode y navega a la carpeta del proyecto.
2. Abre el notebook de tu interés desde la carpeta `notebooks/`.
3. Selecciona el kernel correspondiente al entorno creado con `uv`.
4. Ejecuta las celdas siguiendo el orden propuesto en la sección "Estructura de la formación".

**Ejemplo de inicio rápido en Jupyter:**

```sh
uv sync
# Abre un notebook y selecciona el kernel .venv
```


## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Puedes colaborar de las siguientes formas:

- Proponiendo mejoras o reportando errores mediante issues.
- Enviando pull requests con nuevas funciones, correcciones o notebooks.
- Sugiriendo mejoras en la documentación.

Por favor, sigue las buenas prácticas de la comunidad y revisa la documentación interna antes de enviar tu contribución.

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Puedes consultar el archivo LICENSE para más detalles.

---

## 📬 Soporte y contacto

Para cualquier duda, sugerencia o problema, abre un issue en el repositorio o contacta con el equipo de formación. ¡Gracias por tu interés en MedicalImage-PGTD! 😊
