# Checklist LIDL — Generador

App web para generar checklists de mantenimiento trimestral de LIDL.

## Archivos
- `server.py` — servidor Flask (backend)
- `index.html` — interfaz web (frontend)
- `plantilla.xlsx` — plantilla Excel original con logos y formato
- `requirements.txt` — dependencias Python
- `Procfile` — configuración para Render/Railway

## Subir a Render (gratis)

1. Crea una cuenta en https://render.com
2. Haz clic en **New > Web Service**
3. Conecta tu cuenta de GitHub y sube esta carpeta como repositorio
4. Configura:
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `gunicorn server:app`
5. Haz clic en **Deploy**

## Subir a Railway (gratis)

1. Crea una cuenta en https://railway.app
2. Haz clic en **New Project > Deploy from GitHub**
3. Sube esta carpeta como repositorio
4. Railway detecta automáticamente el Procfile y despliega

## Uso local (sin servidor)

1. Instala Python 3 y ejecuta:
   ```
   pip install -r requirements.txt
   python server.py
   ```
2. Abre http://localhost:5050 en el navegador
