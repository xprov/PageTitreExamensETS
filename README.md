# Page titre pour les examen intra et finaux à l'ÉTS


La [page titre officielle](https://www.etsmtl.ca/docs/personnel-enseignant-examens-finaux/documents/page-titre) au format Word ainsi que son [guide de rédaction](https://www.etsmtl.ca/docs/personnel-enseignant-examens-finaux/documents/Explications-de-la-page-titre) sont disponibles à l'adresse suivante :

[https://www.etsmtl.ca/personnel-enseignant-examens-finaux](https://www.etsmtl.ca/personnel-enseignant-examens-finaux)

Le but de ce projet est d'offrir une alternative en LaTeX.

<a href="https://dev.azure.com/xavierprovencal/f67f346b-d011-4c58-a5e3-73080b537fa2/_apis/git/repositories/ca7446aa-e78a-4093-b4e8-40e01ab5d3b6/items?path=/images/exemple_simple.png&versionDescriptor%5BversionOptions%5D=0&versionDescriptor%5BversionType%5D=0&versionDescriptor%5Bversion%5D=master&resolveLfs=true&%24format=octetStream&api-version=5.0&download=true"><img src="https://dev.azure.com/xavierprovencal/f67f346b-d011-4c58-a5e3-73080b537fa2/_apis/git/repositories/ca7446aa-e78a-4093-b4e8-40e01ab5d3b6/items?path=/images/exemple_simple.png&versionDescriptor%5BversionOptions%5D=0&versionDescriptor%5BversionType%5D=0&versionDescriptor%5Bversion%5D=master&resolveLfs=true&%24format=octetStream&api-version=5.0&download=true" width="300"/></a>
<a href="https://dev.azure.com/xavierprovencal/f67f346b-d011-4c58-a5e3-73080b537fa2/_apis/git/repositories/ca7446aa-e78a-4093-b4e8-40e01ab5d3b6/items?path=/images/exemple_complexe.png&versionDescriptor%5BversionOptions%5D=0&versionDescriptor%5BversionType%5D=0&versionDescriptor%5Bversion%5D=master&resolveLfs=true&%24format=octetStream&api-version=5.0&download=true"><img src="https://dev.azure.com/xavierprovencal/f67f346b-d011-4c58-a5e3-73080b537fa2/_apis/git/repositories/ca7446aa-e78a-4093-b4e8-40e01ab5d3b6/items?path=/images/exemple_complexe.png&versionDescriptor%5BversionOptions%5D=0&versionDescriptor%5BversionType%5D=0&versionDescriptor%5Bversion%5D=master&resolveLfs=true&%24format=octetStream&api-version=5.0&download=true" width="300"/></a>


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


## TODO

Bug : la taille du texte de la page titre est affecté par le paramètre de taille de
la commande `\documentclass`.



