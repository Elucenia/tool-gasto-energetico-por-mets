<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · fr · no clinical/professional/rights approval -->

# Dépense énergétique selon les MET

[conditions, sources et autorisations](https://elucenia.org/fr/outils/gasto-energetico-por-mets)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Intensité de l’activité (valeur du Compendium)

`met`

METs · intervalle: 1–25

### Poids

`peso`

kg · intervalle: 20–300

### Durée de la séance

`min`

min · intervalle: 1–600

### Séances par semaine

`sessoes`

facultatif · intervalle: 1–14

## Édition de la méthode

MET standard 3,5 mL O₂/kg/min ; kcal/min=MET×3,5×kg/200 ; référence Compendium 2024

## Formule documentée

kcal/min = MET × 3,5 × poids (kg) ÷ 200 (1 MET = 3,5 mL O2/kg/min ; environ 5 kcal par litre d’O2).

MET-min = MET × minutes. Approximation équivalente : kcal ≈ MET × poids (kg) × heures.

## Limites et population

Les MET du Compendium adulte 2024 correspondent aux activités des adultes de 19–59 ans ; les données des personnes ≥60 ans ont été exclues de cette édition. Les valeurs standardisées, y compris les valeurs estimées, ne mesurent pas la dépense individuelle. Enfants, personnes âgées et situations cliniques particulières exigent des sources et méthodes adaptées à ces populations.

## Références

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

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
