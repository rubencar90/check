=== CHECKLIST LIDL - Instrucciones de despliegue ===

ARCHIVOS:
- server.py        -> Servidor Flask (backend)
- plantilla.xlsx   -> Plantilla Excel original con logos y formato
- static/index.html -> Interfaz web
- requirements.txt -> Dependencias Python

DESPLIEGUE EN RENDER (gratuito):
1. Crea cuenta en https://render.com
2. Sube estos archivos a un repositorio de GitHub
3. En Render: "New Web Service" -> conecta tu repo
4. Build Command: pip install -r requirements.txt
5. Start Command: gunicorn server:app
6. ¡Listo! Te da una URL pública para acceder desde cualquier sitio

EJECUCIÓN LOCAL:
1. pip install -r requirements.txt
2. python server.py
3. Abre http://localhost:5050 en el navegador
