<!-- ELUCENIA technical documentation · sistema-de-bethesda-tireoide · fr · no clinical/professional/rights approval -->

# Système Bethesda pour la cytologie thyroïdienne

[conditions, sources et autorisations](https://elucenia.org/fr/outils/sistema-de-bethesda-tireoide)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Catégorie du compte rendu

`cat`

- `1` — I · Non diagnostique
- `2` — II · Bénigne
- `3` — III · Atypie de signification indéterminée (AUS)
- `4` — IV · Néoplasie folliculaire
- `5` — V · Suspecte de malignité
- `6` — VI · Maligne

## Édition de la méthode

Bethesda thyroïde 2023, 3e édition : 6 catégories, ROM et AUS nucléaire/autres ; vérification documentaire limitée au code de la catégorie sélectionnée

## Formule documentée

Six catégories diagnostiques, ROM moyen et plage attendue, troisième édition 2023 : nom unique par catégorie, AUS en atypie nucléaire et autres.

## Limites et population

La catégorie Bethesda doit provenir d’un compte rendu cytopathologique de ponction thyroïdienne à l’aiguille fine et ne pas être attribuée par le calculateur. Le risque moyen et l’intervalle sont des estimations de l’édition, pas un diagnostic individuel. L’édition 2023 traite de risques et de prises en charge pédiatriques spécifiques ; les valeurs adultes ne doivent pas être automatiquement extrapolées aux enfants. Dans cette vérification, l’accès direct à l’article de 2023 n’a fourni que le résumé de l’éditeur ; le tableau des ROM a été consulté dans une reproduction de l’article original par un tiers, avec une image de faible résolution. Le Tableau 2 reproduit indique une plage d’AUS de 13–30 %, tandis que le texte du même article indique 20–32 %. Ces plages n’ont pas été départagées. Le test vérifie uniquement le code de la catégorie sélectionnée ; les ROM adultes, les ROM pédiatriques et la prise en charge n’ont pas été validés dans cette vérification.

## Références

- [Ali SZ et al. The 2023 Bethesda System for Reporting Thyroid Cytopathology. Thyroid, 2023.](https://doi.org/10.1089/thy.2023.0141)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
