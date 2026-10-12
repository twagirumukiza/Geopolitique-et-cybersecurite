# Instructions d’intégration — Version académique

## Fichiers fournis

| Fichier | Rôle |
|---------|------|
| `au-dela-du-systeme-d-information.html` | Page HTML dédiée avec métadonnées Google Scholar |
| `au-dela-du-systeme-d-information.pdf` | PDF complet (texte sélectionnable, ~16 Ko) |
| `INSTRUCTIONS-GITHUB-PAGES.md` | Ce fichier |

## 1. Structure recommandée dans ton dépôt GitHub Pages

```
ton-repo/
├── index.html                    # (ta page d’accueil existante)
├── publications/
│   ├── index.html                # (liste optionnelle des publications)
│   ├── au-dela-du-systeme-d-information.html
│   └── au-dela-du-systeme-d-information.pdf
└── ...
```

**URL stable attendue :**  
`https://twagirumukiza.github.io/publications/au-dela-du-systeme-d-information.html`  
(adapte le chemin si ton dépôt utilise un autre nom ou une branche `gh-pages`).

## 2. Métadonnées Google Scholar déjà présentes

Dans le `<head>` de la page HTML :

```html
<meta name="citation_title" content="La géopolitique de la cybersécurité : dépendances numériques et résilience organisationnelle">
<meta name="citation_author" content="Twagirumukiza, Innocent">
<meta name="citation_publication_date" content="2026/10/13">
<meta name="citation_online_date" content="2026/10/13">
<meta name="citation_pdf_url" content="https://twagirumukiza.github.io/publications/au-dela-du-systeme-d-information.pdf">
<meta name="citation_language" content="fr">
<meta name="citation_keywords" content="cybersécurité; gestion des risques; ...">
```

**Important :**  
Après dépôt, vérifie que l’URL dans `citation_pdf_url` correspond **exactement** à l’adresse réelle du PDF sur ton site.  
Si ton nom d’utilisateur GitHub ou le chemin du dépôt diffère, mets à jour cette balise.

## 3. Critères Google Scholar respectés

| Exigence | Statut |
|----------|--------|
| Une URL par article | Oui (page HTML distincte) |
| Résumé visible | Oui (directement sur la page, sans clic) |
| PDF complet, texte sélectionnable, < 5 Mo | Oui (~16 Ko) |
| Auteur et titre sur la 1ère page du PDF | Oui |
| Bibliographie formelle | Oui (section Références) |
| Métadonnées citation_* | Oui |
| Liens HTML simples | Oui |

## 4. Dépôt sur Zenodo (fortement recommandé)

1. Crée un compte sur [https://zenodo.org](https://zenodo.org) (ou connecte-toi via ORCID / GitHub).
2. « New upload » → dépose le PDF.
3. Remplis :
   - **Title** : La géopolitique de la cybersécurité : dépendances numériques et résilience organisationnelle
   - **Authors** : Twagirumukiza, Innocent
   - **Publication date** : 2026-10-13
   - **Description** : (copie le résumé français)
   - **Keywords** : cybersécurité, gestion des risques, dépendances numériques, résilience organisationnelle, géopolitique, chaîne d’approvisionnement, GRC
   - **License** : Creative Commons Attribution 4.0 (recommandé pour maximiser la réutilisation)
4. Publie → Zenodo attribue un **DOI** (ex. 10.5281/zenodo.XXXXXXX).
5. Ajoute le DOI dans :
   - la page HTML (`citation_doi` si tu veux) ;
   - le PDF (version mise à jour) ;
   - ta page LinkedIn / site perso.

Le DOI renforce l’indexation et la citabilité, indépendamment de Google Scholar.

## 5. Lien depuis ta tribune existante

Sur ta page tribune actuelle, ajoute un encadré discret :

> **Version académique documentée**  
> Une version révisée avec bibliographie formelle et métadonnées d’indexation est disponible :  
> [Lire la version académique](../publications/au-dela-du-systeme-d-information.html) · [PDF](../publications/au-dela-du-systeme-d-information.pdf)

Cela préserve la tribune originale tout en orientant les lecteurs académiques vers la version structurée.

## 6. Contrôle d’indexation Google Scholar

- L’indexation est **automatique** (pas de soumission manuelle nécessaire).
- Délai typique : quelques semaines à quelques mois.
- Tu peux accélérer la découverte en :
  - déposant sur Zenodo (DOI) ;
  - citant l’article depuis d’autres pages indexées ;
  - partageant le lien sur LinkedIn / X avec le titre exact.

## 7. Points de vigilance

- Les commentaires affichés dans la tribune originale ne sont pas nécessaires sur la page académique (ils ont été omis).
- Les liens de partage de la tribune pointent encore vers `example.com` : corrige-les séparément si tu conserves la tribune.
- Ne présente **pas** cette version comme « peer-reviewed ». La note d’auteur le précise clairement.

## 8. Prochaines étapes suggérées

1. Déposer les deux fichiers dans `/publications/` de ton dépôt.
2. Mettre à jour l’URL du PDF dans les métadonnées HTML.
3. Créer le dépôt Zenodo et obtenir le DOI.
4. Ajouter le lien depuis ta tribune et ton site personnel.
5. (Optionnel) Préparer la version anglaise complète du corps de texte si tu vises un public international plus large.

---

**Auteur de cette préparation :** version académique préparée à partir de la tribune originale d’Innocent Twagirumukiza, avec sources ENISA 2025/2026 et conclusions du Conseil de l’UE (mars 2026).
