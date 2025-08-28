(cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF'
diff --git a/README.md b/README.md
--- a/README.md
+++ b/README.md
@@ -1,2 +1,27 @@
-# Stage-Leker-Lilian
-Site pour stage en Ruby on Rails.
+# Rapport de stage – site statique (multi‑pages)
+
+Site professionnel, découpé en 5 pages, avec menu déroulant et styles responsive/print.
+
+## Pages
+- `index.html` (Accueil)
+- `informations.html` (1. Informations sur le stage)
+- `entreprise.html` (2. Présentation de l’entreprise)
+- `retour.html` (3. Retour d’expérience)
+- `analyse.html` (4. Analyse critique)
+- `projet.html` (5. Projet professionnel)
+
+## Modifier les informations
+- Nom, période, tuteur et e‑mail sont déjà renseignés.
+- Entreprise: activité (SaaS éthique/écologique), année 2023, contexte de création, équipe.
+- Vous pouvez éditer directement les fichiers HTML.
+
+## Publication (GitHub Pages)
+1. Create repository (public) > Upload files > Commit changes
+2. Settings > Pages > Build and deployment
+   - Source: Deploy from a branch
+   - Branch: main / (root)
+3. Attendre ~1–2 min > « Your site is live at … »
+
+## Export PDF
+- Ouvrir la page souhaitée > bouton « Télécharger en PDF » (styles d’impression intégrés).
+
EOF
)
