# CRM SaaS — Maquettes

Maquettes HTML statiques d'un CRM SaaS (dashboard, CRM, pipeline, devis, compta, RH, tickets, GED, etc.).

## Aperçu local

Ouvre simplement `index.html` dans un navigateur, ou lance un petit serveur depuis le dossier :

```bash
python3 -m http.server 8000
# puis http://localhost:8000
```

## Mise en ligne sur GitHub Pages

1. Crée un repo public (ex. `crm-maquette`) sur GitHub.
2. Depuis ce dossier :

   ```bash
   git init
   git add .
   git commit -m "Initial: maquettes CRM"
   git branch -M main
   git remote add origin https://github.com/<ton-pseudo>/crm-maquette.git
   git push -u origin main
   ```

3. Sur GitHub : **Settings → Pages**, source = `main` / root, puis **Save**.
4. L'URL `https://<ton-pseudo>.github.io/crm-maquette/` sera disponible au bout d'une minute ou deux.

## Structure

- `index.html` — point d'entrée, redirige vers `dashboard.html`
- `shell.html` — état "shell vide" de l'app (référence, non fonctionnel en navigation)
- `dashboard.html` — tableau de bord (vraie page d'accueil)
- `crm.html`, `entreprise.html`, `etablissement.html` — CRM et fiches
- `pipeline.html`, `devis.html` — commercial
- `compta.html`, `compta-facturation.html`, `abonnements.html` — comptabilité & facturation
- `projets.html`, `tickets.html`, `workflows.html`, `ged.html` — opérations
- `rh.html` — RH
- `admin.html`, `utilisateurs.html`, `auth.html` — administration
- `design-system.css` — feuille de style partagée
