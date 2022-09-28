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

2. Inclure la page-titre. En entête de votre document ajouter la commande :
```
\usepackage{pagetitre-ets}
```

3. Configurer la page titre. Avant la ligne `\begin{document}`, copiez le bloc
   suivant et configurez-le selon vos besoin.
```latex

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%%%%% PAGE TITRE (début) %%%%%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%


% AVERTISSEMENT : en cas de doute, toujours vous référer au document
% ``Explication de la page titre 2022'' disponible sur le site web de l'ÉTS :
% https://www.etsmtl.ca/personnel-enseignant-examens-finaux


%%% Les tailles des boites sont fixes et ne tiennent pas compte de ce
%%% qui y est écrit. Si vous souhaite modifier la taille d'une boite, 
%%% utilisez les commandes suivantes:
%\setHauteurBoiteOuEcrireLesReponses{2.0}
%\setHauteurBoiteCalculatrice{1.4}
%\setHauteurBoiteDocumentation{1.4}
%\setHauteurBoiteAnnexes{0.9}
%\setHauteurBoiteDirectivesParticulieres{2.0}

%%%  Sélectionner le type d'examen
% Note : si l'examen est en deux parties, chaque partie doit avoir sa page titre.
\setType{Mini-test $\#$1}
%\setType{EXAMEN INTRA -- Partie 1 de 2}
%\setType{EXAMEN INTRA -- Partie 2 de 2}
%\setType{EXAMEN INTRA DIFFÉRÉ}
%\setType{EXAMEN INTRA DIFFÉRÉ -- Partie 1 de 2}
%\setType{EXAMEN INTRA DIFFÉRÉ -- Partie 2 de 2}
%\setType{EXAMEN FINAL}
%\setType{EXAMEN FINAL -- Partie 1 de 2}
%\setType{EXAMEN FINAL -- Partie 2 de 2}
%\setType{EXAMEN FINAL DIFFÉRÉ}
%\setType{EXAMEN FINAL DIFFÉRÉ -- Partie 1 de 2}
%\setType{EXAMEN FINAL DIFFÉRÉ -- Partie 2 de 2}


%%%  Quand l'examen aura-t-il lieu ?
\setAnnee{2022}
\setSaison{Automne} % Choisir parmi : Hiver, Été, Automne
\setDate{6 octobre} % Jour et mois (l'année est déjà spécifiée avec \setAnnee)
\setHeure{13h30} % Début de l'examen
\setDuree{1h00}  % Je pense que c'est évident.


%%%  Informations générales
\setSigleEtTitre{MAT472 -- Algèbre linéaire et géométrie de l'espace}
\setGroupes{01}
\setEnseignants{
  Xavier Provençal
}


%%  Format de l'examen, sélectionner
%\setOuEcrireLesReponses{dans le cahier d'examen standard ÉTS.}
\setOuEcrireLesReponses{sur ce questionnaire.}
%\setOuEcrireLesReponses{sur ce questionnaire pour les questions ## à ## et dans le cahier d'examen standard ÉTS pour les question ## à ##.}
%\setOuEcrireLesReponses{Autre} % spécisez avec la commande \setOuEcrireLesReponsesPrecisions

%% facultatif : ajouter des précisions quant à l'endroit où écrire les réponses
%\setOuEcrireLesReponsesPrecisions{Pour les graphiques, utilisez des crayons de couleur.}


% Nombre de question et nombre de pages. Si l'examen est sur ENAQuiz, il faut
\setNbQuestions{4}
%\setNbPages{5} % optionnel, si non spécifié alors la valeur `\pageref{LastPage}` est utilisée


%% Calculatrice, indiquee si elle est autorisee ou interdite (obligatoire)
%\setCalculatriceAutorisee
\setCalculatriceInterdite

%% Si la calculatrice est autorisée, indiquée le type (une case sera cochée)
%\setTypeCalculatriceTous
%\setTypeCalculatriceProgrammable
%\setTypeCalculatriceNonProgrammable
%\setTypeCalculatriceLogiciel

%% Indiquez le(s) modèle(s) de calculatrice
%\setCalculatriceModelesPermis{``TI-nspire CX CAS'' et ``TI-nspire CX II CAS''.}

%% Documentation, choisissez au moins une options et complétez si nécessaire.
%% La commande `\item` n'est pas optionnelle.
\setDocumentation{
\item Une feuille de note personnelles (format lettre, recto-verso, manuscrite ou imprimée).

  %\item feuille(s) de note(s), précisez le format et le nombre de pages
  %\item toutes documentation papier
  %\item documentation électronique, préciser :
  %\item documentation papier et électronique, précisez :
  %\item limitée, précisez :

  %% Exemples 
  %\item 1 feuille de note, au format lettre (2 pages en tout).
  %\item 3 tables de formules remise par l'enseignant(e) : tables de
  %  trigonométrie (feuille verte), formules de dérivation (feuille jaune),
  %  formules d'intégration (feuille bleue).
}


%% Annexes, choississez une ligne et complétez.
%% La commande `\item` n'est pas optionnelle.
\setAnnexes{
  \item Aucune
  %\item oui, préciser le titre et spécifiez les pages.
}

%% Inscivez vos directives particulière ici. S'il n'y a pas, il faut quand même
%% appeler la commande avec un paramètre vide.
%\setDirectivesParticulieres{}

%% Décommentez si l'examen est en plusieurs parties. Indiquez les directives ici.
%\setExamenEnPlusieursParties{Deux parties : calculatrice est interdite pour la première partie, mais autorisée pour la deuxième. La durée maximale de la première partie : 45 minutes.}


%% Matériel informatique
%\setMaterielInformatiqueAutorise
\setMaterielInformatiqueInterdit

%% Si du matériel informatique est autorisée, il faut obligatoirement préciser de quoi il s'agit
%\setTypeMaterielInformatiqueTous
%\setTypeMaterielInformatiqueOrdinateurPortable
%\setTypeMaterielInformatiqueTablette
%\setTypeMaterielInformatiqueCleUSB
%\setTypeMaterielInformatiqueAutre{Précisions ici}


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%%%%% PAGE TITRE (fin) %%%%%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

```


4. TODO

Bug : la taille du texte de la page titre est affecté par le paramètre de taille de
la commande `\documentclass`.



