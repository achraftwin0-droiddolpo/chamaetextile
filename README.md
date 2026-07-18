# Site CHAMAE TEXTILES

Site vitrine statique, responsive et accessible pour CHAMAE TEXTILES, société marocaine de commerce de textiles import-export. Le contenu public repose sur les dossiers fournis (DUNS, données publiques et bulletin fiscal). Aucun framework, traqueur, cookie ou service externe n'est utilisé.

## Structure

- `index.html` : accueil, activité, approche, identité, FAQ et contact
- `privacy-policy.html` : politique adaptée au fonctionnement réel du site
- `404.html` : page d'erreur
- `assets/css/` : design, animations et responsive
- `assets/js/` : navigation, formulaire et animations
- `assets/images/` : favicon et image sociale temporaire en SVG
- `robots.txt` et `sitemap.xml` : fondations SEO

## Utilisation locale

Ouvrir `index.html` directement, ou lancer depuis ce dossier :

```powershell
python -m http.server 8000
```

Puis visiter `http://localhost:8000`.

## Personnalisation

- Informations et services : modifier le HTML de `index.html`.
- Couleurs : modifier les variables au début de `assets/css/style.css`.
- Logo : aucun logo officiel n'a été fourni. Remplacer les éléments `.brand-mark` par une image locale avec texte alternatif et dimensions définies.
- Images : placer des fichiers optimisés (WebP/AVIF) dans `assets/images/`, employer des noms descriptifs, `loading="lazy"`, un texte alternatif et des dimensions.
- E-mail / WhatsApp : aucune coordonnée n'est disponible. Une fois vérifiée, ajouter un lien `mailto:` ou `https://wa.me/NUMERO` sans espaces, puis actualiser la politique de confidentialité.
- Formulaire : il valide et copie le message localement, sans envoi ni stockage. Pour une API, remplacer ce comportement dans `assets/js/main.js`, utiliser HTTPS, validation serveur, protection anti-spam et messages d'état exacts. Actualiser la politique avant mise en ligne.
- SEO : remplacer `example.com` dans `robots.txt` et `sitemap.xml`, ajouter URL canonique et image sociale officielle sur chaque page.
- Confidentialité : actualiser la date et le contenu à chaque changement fonctionnel. Si des outils non essentiels sont ajoutés, les bloquer avant consentement et créer une préférence modifiable.

## Déploiement

- GitHub Pages : pousser le dossier dans un dépôt, puis activer Pages sur la branche principale/racine.
- Netlify : glisser le dossier dans Netlify ou connecter le dépôt ; aucun build n'est requis.
- Vercel : importer le dépôt comme projet statique, sans commande de build.
- Hébergement classique : téléverser tout le contenu en conservant l'arborescence et servir en HTTPS.

En production, recommander notamment les en-têtes `Content-Security-Policy: default-src 'self'; img-src 'self' data:; style-src 'self'; script-src 'self'; base-uri 'self'; form-action 'self'`, `X-Content-Type-Options: nosniff`, `Referrer-Policy: strict-origin-when-cross-origin` et une politique `Permissions-Policy` restrictive. Ajuster la CSP si des services sont ajoutés.

## Sources et hypothèses

Les sources indiquent : CHAMAE TEXTILES ; SARL à associé unique ; activité « commerce de textiles import-export » ; ICE 003618970000081 ; RC et identifiant fiscal 651351 ; adresse « Quartier Industriel Route de Tétouan C/o Tantex ». La ville est contradictoire (Casablanca dans une source, Tanger dans D&B et dans le libellé de l'adresse) : elle est volontairement omise de l'affichage public jusqu'à confirmation. La mention « société active » est appuyée par les fichiers de vérification datés de juillet 2026, mais doit être recontrôlée avant publication.

Les formulations de services décrivent uniquement le champ de l'activité déclarée ; elles ne promettent ni stock, ni prix, ni délai, ni certification. Aucun témoignage, statistique, téléphone, e-mail, réseau social ou horaire n'a été inventé. Le monogramme `CT` est une identité visuelle temporaire, pas un logo officiel.

## Information required before production launch

- [ ] Domaine de production et URL canonique
- [ ] Logo officiel, favicon et visuel de partage définitif
- [ ] Confirmation de l'adresse complète et de la ville
- [ ] Téléphone professionnel et numéro WhatsApp
- [ ] E-mail commercial et e-mail de confidentialité
- [ ] Nom légal exact à afficher et éventuel représentant légal
- [ ] Confirmation des numéros RC, ICE et identifiant fiscal pour affichage public
- [ ] Horaires et réseaux sociaux officiels, si souhaités
- [ ] Description détaillée des catégories de textiles, marchés et capacités
- [ ] Hébergeur et pays d'hébergement
- [ ] Backend du formulaire, règles de conservation et destinataires
- [ ] Choix analytique ; s'il est non essentiel, gestion du consentement
- [ ] Domaine final dans `robots.txt` et `sitemap.xml`
- [ ] Test des métadonnées sociales et ajout des URL canoniques
- [ ] Relecture linguistique, commerciale et légale finale

## Avis juridique

La politique de confidentialité reflète le site statique actuel : pas de cookies, analyse, carte, police externe ou transmission serveur. Elle ne constitue pas un conseil juridique. Faites examiner le texte final par un professionnel qualifié avant publication, particulièrement après ajout de coordonnées, hébergement, formulaire serveur, analytics ou services tiers.
