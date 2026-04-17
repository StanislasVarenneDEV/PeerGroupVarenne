# Déploiement — Varenne Peer Group

## Fichiers à uploader
- app.py
- requirements.txt
- packages.txt  ← créer ce fichier avec le contenu ci-dessous

## Contenu de packages.txt
chromium
chromium-driver

## Étapes Streamlit Cloud (gratuit)

1. Crée un compte GitHub → https://github.com
2. Nouveau repo → "varenne-peer-group" → Public
3. Upload les 3 fichiers (app.py, requirements.txt, packages.txt)
4. Va sur https://streamlit.io/cloud → "New app"
5. Sélectionne ton repo → Main file : app.py → Deploy

## URL finale
https://[username]-varenne-peer-group-app-[hash].streamlit.app

## Alternative : Render.com
- New Web Service → Connect GitHub
- Build : pip install -r requirements.txt && playwright install chromium
- Start : streamlit run app.py --server.port $PORT --server.address 0.0.0.0
