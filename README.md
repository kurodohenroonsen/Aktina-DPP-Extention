# Aktina-DPP-Extention

**Version**: 1.0  
**Author**: Kurodo Henro Onsen

## Description

**Aktina-DPP-Extention** est une extension de navigateur qui injecte automatiquement des données dans les formulaires à partir d'un fichier JSON au format **GS1voc dérivé de schema.org**, utilisé notamment sur le site [batra.link](https://www.batra.link). L'extension est conçue pour automatiser le remplissage des formulaires sur les sites web à l'aide de données conformes aux normes GS1 et à la directive INCO1169 de l'Union Européenne sur l'étiquetage des produits alimentaires.

L'extension fait une requête GET vers une URL spécifique (par exemple : `https://www.batra.link/01_new/01454000000215/01454000000215.json`) et injecte les données récupérées dans les champs appropriés du formulaire de la page courante.

## Fonctionnalités

- Injecte automatiquement des données structurées au format **GS1voc** dérivé de **schema.org** dans les champs de formulaire.
- Les données sont conformes à la directive **INCO1169** de l'UE, incluant les informations nutritionnelles et les allergènes.
- Fonctionne sur toutes les pages web grâce à un script d'injection de contenu.

## Données conformes à la directive INCO1169

L'extension traite et injecte les données suivantes, en conformité avec la directive INCO1169/2011 de l'UE :

1. **Nom du produit régulé** (ex. : `"Mayonnaise"`)
2. **Déclaration des ingrédients** (ex. : huile de colza, œufs, moutarde, etc.)
3. **Valeur énergétique** (ex. : `3040 kJ / 739 kcal`)
4. **Quantité de matières grasses**, **acides gras saturés**, **glucides**, **sucres**, **protéines**, et **sel**
5. **Allergènes** (ex. : contient des œufs, contient de la moutarde)
6. **Poids net** (ex. : `0.52 kg`)
7. **Instructions de conservation** (ex. : "À conserver au frais après ouverture")
8. **Adresse de l'exploitant** (ex. : GB Foods BELGIUM NV, Rijksweg 16, B-2870 Puurs, Belgique)

## Installation

1. Clonez ce dépôt ou téléchargez les fichiers de l'extension.
   ```bash
   git clone https://github.com/username/form-data-injector-extension.git
