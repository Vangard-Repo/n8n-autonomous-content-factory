🤖 Autonomous AI Content Factory (n8n + FFmpeg + DeepSeek)
![alt text](https://raw.githubusercontent.com/Vangard-Repo/n8n-autonomous-content-factory/main/autonomous-content-factory.PNG)

🚀 Sobre este Proyecto
Este repositorio contiene la arquitectura de un Agente Autónomo de Creación de Contenido. No es una simple automatización; es una fábrica de contenido operando en piloto automático.
Diseñado para Agencias de Marketing, Creadores de Contenido y Startups que necesitan escalar su presencia digital en múltiples plataformas (Instagram, TikTok, YouTube Shorts, Facebook y WhatsApp) sin invertir cientos de horas semanales en edición y copywriting.

📺 Mira la demostración en video de este sistema funcionando aquí

⚙️ ¿Cómo funciona el "Cerebro" de este Agente?
Este flujo de n8n orquesta múltiples inteligencias artificiales y motores de renderizado en la nube para ejecutar el ciclo completo de vida de un video viral:

📡 Curaduría de Tendencias (Scraping): Monitorea feeds RSS (ej. Reddit) para encontrar videos virales en tendencia, aplicando un filtro anti-duplicados en base de datos.

📥 Extracción y Procesamiento: Descarga el video original y extrae el audio de forma asíncrona.

🧠 Transcripción y Traducción AI (Gladia + DeepSeek): Envía el audio a Gladia AI para generar transcripciones precisas, y luego usa el modelo LLM de DeepSeek (con prompting avanzado) para transcrear y localizar el guion al español neutro, adaptando el humor y el contexto.

🎬 Motor de Edición Visual (FFmpeg + CloudConvert): Mediante comandos crudos de FFmpeg, el sistema quema los subtítulos (.srt) en el video, renderiza fondos dinámicos, superpone imágenes (Slides) y formatea la resolución para formato vertical (9:16).

✍️ Copywriting Omnicanal: DeepSeek analiza el contexto visual y social del video para redactar Ganchos, Llamados a la Acción (CTAs) y Captions optimizados específicamente para los algoritmos de Instagram, TikTok y YouTube.

🚀 Distribución Autónoma (Postiz & Meta API): Programa y publica automáticamente los videos, Reels, Historias y Carruseles en todas las plataformas sociales con márgenes de tiempo calculados para evitar baneos por spam.

🛠️ Stack Tecnológico Utilizado
Orquestador: n8n (Self-hosted)
Modelos LLM: DeepSeek (Reasoning & Copywriting) / OpenAI (Image Vision)
Procesamiento de Audio/Video: FFmpeg, CloudConvert API, Gladia API
Publicación: Postiz API, Meta Graph API, TikTok API, Evolution API (WhatsApp/Telegram)
Almacenamiento: GitHub (Hosting temporal de assets), Cloudinary

⚠️ Nota Importante sobre la Implementación
El archivo .json proporcionado en este repositorio está limpio y sin credenciales (tokens, passwords, API keys eliminadas) por razones de seguridad.
La implementación de este sistema requiere configuración de servidores VPS, manejo de Webhooks, configuración de dominios, APIs de Meta (Facebook/Instagram), cuotas de CloudConvert y conexión a bases de datos. No es un script de tipo "plug-and-play" para principiantes.

💼 ¿Buscas implementar esto en tu negocio?
Si tienes una empresa o agencia y quieres que diseñe, instale y mantenga una fábrica de contenido autónoma adaptada a tu marca, contáctame.

🌐 Visita mi web y conoce mis servicios: vangard-ai.com

📩 O contrátame a través de Workana: Mi Perfil de Workana
