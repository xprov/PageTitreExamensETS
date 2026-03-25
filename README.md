# Page titre pour les examen intra et finaux à l'ÉTS

Le but de ce projet est d'offrir une alternative en LaTeX à la page titre au format Word publiée par le bureau de la registraire (BDR).

**Avertissement** : le BDR effectue régulièrement des mises à jour de sa page titre. Il est de votre responsabilité de vous assurer que la version que vous utilisez contient toutes les informations requises. En cas de disparité, veuillez utiliser la version officielle.

<a href="https://profs.etsmtl.ca/xprovencal/pagetitre/exemple_simple.png"><img src="https://profs.etsmtl.ca/xprovencal/pagetitre/exemple_simple.png" width="300"/></a>


## Utilisation

1. Ajouter les fichiers suivants à votre projet :
 - `pagetite-ets.sty`
 - `logo_ets.png`
 - `configPageTitre.tex`

2. Inclure la page-titre et le fichier de configuration. En entête de votre
   document ajouter les lignes:
```latex
\usepackage{pagetitre-ets}
\input{configPageTitre.tex}
```

3. Configurer la page titre en modifiant le fichier `configPageTitre.tex`.

4. Immédiatement après la commande `\begin{document}`, ajouter la ligne
```latex
\pagetitreETS
```
