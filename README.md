# Scan-Prix (améliorations UI & technique)

Petit outil personnel de capture OCR de prix depuis la caméra, conversion de devise via frankfurter.app.

But de ces changements
- Séparer JS/CSS pour plus de lisibilité
- Améliorer l'expérience (spinner, état caméra, labels)
- Robustifier le parsing OCR et la gestion réseau
- Sauvegarder préférences (localStorage)

Tester localement
1. Ouvrir index.html dans un serveur local (ex: `npx http-server` ou `python -m http.server`) car la caméra nécessite HTTPS (ou `localhost`).
2. Cliquer sur "Activer la caméra".
3. Ajuster la fenêtre (ROI), zoom et langue OCR.
4. Cliquer sur "Scanner".

Limites & confidentialité
- Les images sont traitées localement dans le navigateur.
- Les taux de change sont récupérés depuis frankfurter.app (service tiers).

Prochaines étapes (optionnel)
- Ajouter fallback pour Tesseract si CDN indisponible (bundle local).
- Ajouter tests unitaires pour les fonctions de parsing.

