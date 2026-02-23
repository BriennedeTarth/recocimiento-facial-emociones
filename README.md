# Reconocimiento facial de emociones

Este proyecto es una herramienta web ligera y eficiente para el reconocimiento de emociones y detección facial en tiempo real. Desarrollado originalmente para un proyecto de Interacción Humano-Computador (HCI), permite analizar las expresiones faciales de los usuarios mediante la cámara web, extrayendo datos valiosos sobre el estado emocional en tiempo real.

![ejemplo](https://github.com/BriennedeTarth/recocimiento-facial-emociones/blob/main/results/sergio.jpg)
## Características
- **Reconocimiento en tiempo real:** Utiliza `face-api.js` para detectar rostros y clasificar expresiones (feliz, triste, enojado, neutral, etc.).
- **Modelos pre-cargados:** Incluye los pesos necesarios para el detector de rostros (Tiny Face Detector), reconocimiento de expresiones, landmarks faciales y estimación de edad/género.
- **Ligero y Modular:** Basado en tecnologías web estándar (HTML5, JS), ideal para ser integrado en aplicaciones de análisis de usabilidad, marketing emocional o sistemas interactivos.
- **Acceso mediante webcam:** Integración directa con `navigator.mediaDevices.getUserMedia`.

## Tecnologías Utilizadas
- **[face-api.js](https://github.com/justadudewhohacks/face-api.js):** La librería central para el procesamiento de redes neuronales en el navegador.
- **JavaScript (ES6+):** Lógica del sistema y manejo del flujo de video.
- **HTML5/Canvas:** Visualización de los resultados y cajas delimitadoras (bounding boxes) sobre el video.

## Requisitos Previos
Para ejecutar este proyecto, necesitas:
1. Un navegador moderno con soporte para webcam.
2. Un servidor local (como *Live Server* de VS Code o `http-server`) para evitar errores de CORS al cargar los modelos.

## Configuración y Ejecución
1. Clona este repositorio:
   ```bash
   git clone [URL-de-tu-repositorio]
   Servidor Local:
2. Debido a que el navegador restringe el acceso a la cámara y la carga de modelos locales por seguridad (CORS), necesitas ejecutar el proyecto usando un servidor local.

    Si usas VS Code, te recomiendo la extensión Live Server.


## Permisos:
Al abrir la página, asegúrate de otorgar permisos de acceso a la cámara web.

## Notas Técnicas

    El proyecto utiliza tiny_face_detector para un mejor rendimiento en dispositivos con recursos limitados.

    Se recomienda el uso de un entorno con HTTPS (o localhost) para que el navegador permita el acceso a la cámara.
