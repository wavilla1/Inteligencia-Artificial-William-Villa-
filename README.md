## Clase 1

# 1. Nombre del space
   **Nombre:** Trellis.2
   ***Enlace:** https://huggingface.co/spaces/microsoft/TRELLIS.2
   
# 2. Que hace el agente?
    Es un sistema que hace generacion de modelos tridimencionales apartir de imagenes creando la malla de la figura cargada en la imagen,       permitiendo descargar el archivo tridimencional

# 3. Analisis PEAS
   **Performance** El agente realiza correctamente su trabajo cuando genera un modelo 3D que representa de manera fiel el objeto de la         imagen de entrada,con buena calidad, precisión y en un tiempo razonable.
   **Environment** Usuario, imágenes de entrada, interfaz web de Hugging Face, servidor donde se ejecuta el modelo y sistema de                almacenamiento temporal.
   **Actuators** Genera el modelo 3D, lo muestra en pantalla y permite su descarga.
   **Sensors** Imagen cargada por el usuario y parámetros de generación seleccionados.
   
# 4. Clasificacion del entorno
   **Observable** | Total/**Parcial** | El agente solo conoce la imagen proporcionada por el usuario y no dispone de información completa      sobre el objeto real (como la parte trasera o el interior).
   **Determinista** | Si/**No** | El proceso generativo puede producir resultados ligeramente diferentes debido a la naturaleza                probabilística del modelo. 
   **Episódico** | **Si**/No | Cada generación es independiente de las anteriores.
   **Estático** | **Si**/No | La imagen de entrada no cambia mientras el agente procesa la solicitud.
   **Discreto** | Si/**No** | Trabaja con imágenes y modelos 3D, que representan información continua.
   **Conocido** | **Si**/No | El agente conoce las acciones disponibles y el tipo de información que recibe como entrada.

# 5. Tipo de programa de agente
   **Agente con aprendizaje**
   Cuando un usuario proporciona una imagen, el agente utiliza el conocimiento adquirido durante el entrenamiento para inferir la geometría    del objeto y construir un modelo 3D.
   Aunque el modelo no aprende durante cada interacción con el usuario, su funcionamiento depende completamente del aprendizaje obtenido       durante su entrenamiento, por lo que se clasifica como un **agente con aprendizaje**.


