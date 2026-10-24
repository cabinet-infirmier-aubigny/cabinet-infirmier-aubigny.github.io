# Site du cabinet infirmier d'Aubigny

Site statique (HTML/CSS/JS, sans dépendance ni build) pour le cabinet infirmier
d'Aubigny-Les Clouzeaux. Une page principale + une page de mentions légales.

## Structure

```
index.html             page principale (accueil, horaires, prestations, équipe, vaccination, fiches pratiques, contact)
mentions-legales.html  mentions légales (obligatoires en France)
styles.css             mise en forme, responsive mobile
script.js              menu mobile + carte Google chargée au clic (pas de cookies sans action du visiteur)
images/                photos du cabinet
```

## Hébergement

Site en ligne : **https://cabinet-infirmier-aubigny.fr/** (domaine OVHcloud, titulaire SCM Infirmières d'Aubigny ; l'adresse cabinet-infirmier-aubigny.github.io redirige vers le .fr)

Hébergé gratuitement par GitHub Pages (*Settings → Pages* : branche `main`, dossier `/ (root)`).
Toute modification poussée sur `main` est en ligne après 1 à 2 minutes.

Nom de domaine propre (ex. `cabinet-infirmier-aubigny.fr`, environ 10 €/an) : à déclarer dans
*Settings → Pages → Custom domain*. L'hébergement reste gratuit.

## Domaine et DNS (OVHcloud)

- Domaine `cabinet-infirmier-aubigny.fr`, titulaire SCM Infirmières d'Aubigny, payé jusqu'en octobre 2029
  (renouvellement ensuite 7,79 € HT/an). Compte OVH : infadom.aubigny85@orange.fr.
- Zone DNS : 4 A (185.199.108-111.153), 4 AAAA (2606:50c0:8000-8003::153), CNAME `www` → `cabinet-infirmier-aubigny.github.io.`,
  plus les NS, SPF et MX d'OVH (compte mail Zimbra).
- **Ne jamais supprimer** la ligne TXT `_github-pages-challenge-cabinet-infirmier-aubigny` : elle prouve à GitHub
  que le domaine appartient à l'organisation (domaine vérifié).
- GitHub Pages : domaine personnalisé déclaré (fichier `CNAME`), HTTPS forcé.

## À compléter avant la mise en ligne

- [ ] Photos des 4 infirmières : déposer `images/prenom.jpg` (format carré) et remplacer
      les initiales dans la section « Notre équipe » par `<img src="images/prenom.jpg" alt="Prénom Nom">`.
- [ ] Prénom de Mme Mengozzi et nom de la 4ᵉ infirmière.
- [ ] Mentions légales : directrice de la publication, n° RPPS de chaque infirmière.
- [ ] Faire relire la section vaccination (liste des vaccins) par l'équipe.
- [ ] Ajouter le lien du site sur la fiche Google Business Profile.
