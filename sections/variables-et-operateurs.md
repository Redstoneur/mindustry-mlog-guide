# Les Différents Variables et Opérateurs en `mlog`

Dans cette section, nous allons explorer les différents globales variables et d'opérateurs disponibles dans le langage
`mlog`. Ces éléments sont essentiels pour la création de circuits logiques et de systèmes de contrôle sophistiqués. Nous
allons aussi définir les diférents types de variable disponible dans le langage `mlog`

---

## Type de Variables

Les variables sont des éléments qui peuvent stocker des valeurs numériques, des chaînes de caractères, des booléens et
d'autres types de données. Les variables sont utilisées pour stocker des informations importantes, telles que des
paramètres de configuration ou des états de système. Voici les différents types de variables disponibles dans le
langage `mlog` :

| Type de Variable     | Type          | Image                                          | Description                                                                                                                                                                                     |
|----------------------|---------------|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Numérique            | `number`      | ![number](../screenshots/types/number.PNG)     | Les variables numériques stockent des valeurs numériques, telles que des entiers ou des nombres à virgule flottante.                                                                            |
| Booléen              | `number[0,1]` | ![number](../screenshots/types/number.PNG)     | Les variables booléennes stockent des valeurs booléennes, telles que `true` ou `false`. Même si il sont transformer en number lors du stockage dans une variable (0 pour false et 1 pour true). |
| Chaîne de Caractères | `string`      | ![string](../screenshots/types/string.PNG)     | Les variables de chaîne de caractères stockent des séquences de caractères, telles que des mots ou des phrases.                                                                                 |
| Objet                | `content`     | ![content](../screenshots/types/content.PNG)   | Les variables de type objet stockent des valeurs d'entité, telles que des matériaux ou des ressources.                                                                                          |
| Batiments            | `building`    | ![building](../screenshots/types/building.PNG) | Les variables de type building stockent des valeurs de bâtiments.                                                                                                                               |
| Unitées              | `unit`        | ![unit](../screenshots/types/unit.PNG)         | Les variables de type unit stockent des valeurs d'entité qui sont des unités.                                                                                                                   |
| Null                 | `null`        | ![null](../screenshots/types/null.PNG)         | Les variables de type null stockent des valeurs nulles.                                                                                                                                         |

---

## Variables Globales

Les variables globales sont des éléments qui peuvent être utilisés dans n'importe quelle partie de votre code. Elles
peuvent stocker des valeurs numériques, des chaînes de caractères, des booléens et d'autres types de données. Les
variables globales sont utiles pour stocker des informations importantes, telles que des paramètres de configuration ou
des états de système.

### Variable Générale

Les variables générales sont des variables qui peuvent être utilisées dans n'importe quelle partie de votre code et
disponible pour tous les processeurs.

| Nom  | 	Nom IG | Description                                                                 | Type    | Valeur par défaut (si existant) |
|------|---------|-----------------------------------------------------------------------------|---------|---------------------------------|
| unit | @unit   | La variable unit est une variable les unités selectionné par le processeur. | content | null                            |

### Variable de Matériaux

Les variables de matériaux sont des variables qui peuvent être utilisées dans n'importe quelle partie de votre code et
disponible pour tous les processeurs. Ils sont tous de type `content`.

| Nom                 | Nom IG          | Image                                                            |
|---------------------|-----------------|------------------------------------------------------------------|
| cuivre              | 	@copper        | ![copper](../screenshots/materiaux/cuivre.PNG)                   |
| plomb               | 	@lead          | ![lead](../screenshots/materiaux/plomb.PNG)                      |
| Verre Trempé	       | @metaglass      | ![metaglass](../screenshots/materiaux/verre-trempe.PNG)          |
| graphite            | 	@graphite      | ![graphite](../screenshots/materiaux/graphite.PNG)               |
| sable               | 	@sand          | ![sand](../screenshots/materiaux/sable.PNG)                      |
| Charbon	            | @coal           | ![coal](../screenshots/materiaux/charbon.PNG)                    |
| titane	             | @titanium       | ![titanium](../screenshots/materiaux/titane.PNG)                 |
| thorium	            | @thorium        | ![thorium](../screenshots/materiaux/thorium.PNG)                 |
| féraille            | 	@scrap         | ![scrap](../screenshots/materiaux/feraille.PNG)                  |
| silicium            | 	@silicon       | ![silicon](../screenshots/materiaux/silicium.PNG)                |
| plastanium          | 	@plastanium    | ![plastanium](../screenshots/materiaux/plastanium.PNG)           |
| tissu phasé         | 	@phase-fabric  | ![phase-fabric](../screenshots/materiaux/tissu-phase.PNG)        |
| alliage superchargé | 	@surge-alloy   | ![surge-alloy](../screenshots/materiaux/alliage-supercharge.PNG) |
| spore	              | @spore-pod      | ![spore-pod](../screenshots/materiaux/spore.PNG)                 |
| mélange explosif	   | @blast-compound | ![blast-compound](../screenshots/materiaux/melange-explosif.PNG) |
| pyratite	           | @pyratite       | ![pyratite](../screenshots/materiaux/pyratite.PNG)               |

### Variable de Liquides

Les variables de liquides sont des variables qui peuvent être utilisées dans n'importe quelle partie de votre code et
disponible pour tous les processeurs. Ils sont tous de type `content`.

| Nom       | Nom IG     | Image                                               |
|-----------|------------|-----------------------------------------------------|
| eau       | @water     | ![water](../screenshots/liquides/eau.PNG)           |
| scorie    | @slag      | ![slag](../screenshots/liquides/scorie.PNG)         |
| pétrole   | @oil       | ![oil](../screenshots/liquides/petrole.PNG)         |
| cryofluid | @cryofluid | ![cryofluid](../screenshots/liquides/cryofluid.PNG) |
| néoplasme | @neoplasm  | ![neoplasm](../screenshots/liquides/neoplasme.PNG)  |
| arkydite  | @arkycite  | ![arkycite](../screenshots/liquides/arkycite.PNG)   |
| ozone     | @ozone     | ![ozone](../screenshots/liquides/ozone.PNG)         |
| hydrogène | @hydrogen  | ![hydrogen](../screenshots/liquides/hydrogene.PNG)  |
| azote     | @nitrogen  | ![nitrogen](../screenshots/liquides/azote.PNG)      |
| cyanogène | @cyanogen  | ![cyanogen](../screenshots/liquides/cyanogene.PNG)  |

### Variable d'unités

Les variables d'unités sont des variables qui peuvent être utilisées dans n'importe quelle partie de votre code et
disponible pour tous les processeurs. Ils sont tous de type `content`.

| Nom | Nom IG | image |
|-----|--------|-------|

### Variable de Bâtiments

Les variables de bâtiments sont des variables qui ne peuvent être utilisées pour les batiments lier au processeur. Ils
sont tous de type `building`. Ces variables sont définis à la liaison du processeur avec un batiment.

---

## Opérateurs

Les opérateurs sont des symboles qui effectuent des opérations sur des variables et des valeurs. Ils sont utilisés pour
effectuer des calculs, des comparaisons et d'autres manipulations de données.

### Opérateurs Arithmétiques

Les opérateurs arithmétiques sont utilisés pour effectuer des opérations mathématiques sur des variables numériques.

| Opérateur | Description                         | Nom       | Image                                                 |
|-----------|-------------------------------------|-----------|-------------------------------------------------------|
| +         | Addition                            | add       | ![add](../screenshots/operateurs/add.PNG)             |
| -         | Soustraction                        | sub       | ![sub](../screenshots/operateurs/sub.PNG)             |
| *         | Multiplication                      | mul       | ![mul](../screenshots/operateurs/mul.PNG)             |
| /         | Division                            | div       | ![div](../screenshots/operateurs/div.PNG)             |
| //        | Division entière                    | idiv      | ![idiv](../screenshots/operateurs/idiv.PNG)           |
| %         | Modulo                              | mod       | ![mod](../screenshots/operateurs/mod.PNG)             |
| **        | Puissance                           | pow       | ![pow](../screenshots/operateurs/pow.PNG)             |
| <<        | Décalage binaire à gauche           | shl       | ![shl](../screenshots/operateurs/shl.PNG)             |
| \>\>      | Décalage binaire à droite           | shr       | ![shr](../screenshots/operateurs/shr.PNG)             |
| max       | Maximum de deux valeurs             | max       | ![max](../screenshots/operateurs/max.PNG)             |
| min       | Minimum de deux valeurs             | min       | ![min](../screenshots/operateurs/min.PNG)             |
| angle     | Calcul de l'angle entre deux points | angle     | ![angle](../screenshots/operateurs/angle.PNG)         |
| angleDiff | Différence entre deux angles        | angleDiff | ![angleDiff](../screenshots/operateurs/angleDiff.PNG) |
| len       | Longueur d'un vecteur               | len       | ![len](../screenshots/operateurs/len.PNG)             |
| noise     | Génération de bruit aléatoire       | noise     | ![noise](../screenshots/operateurs/noise.PNG)         |
| abs       | Valeur absolue                      | abs       | ![abs](../screenshots/operateurs/abs.PNG)             |
| log       | Logarithme naturel                  | log       | ![log](../screenshots/operateurs/log.PNG)             |
| log10     | Logarithme en base 10               | log10     | ![log10](../screenshots/operateurs/log10.PNG)         |
| floor     | Arrondi à l'entier inférieur        | floor     | ![floor](../screenshots/operateurs/floor.PNG)         |
| ceil      | Arrondi à l'entier supérieur        | ceil      | ![ceil](../screenshots/operateurs/ceil.PNG)           |
| sqrt      | Racine carrée                       | sqrt      | ![sqrt](../screenshots/operateurs/sqrt.PNG)           |
| rand      | Génération d'un nombre aléatoire    | rand      | ![rand](../screenshots/operateurs/rand.PNG)           |
| sin       | Sinus                               | sin       | ![sin](../screenshots/operateurs/sin.PNG)             |
| cos       | Cosinus                             | cos       | ![cos](../screenshots/operateurs/cos.PNG)             |
| tan       | Tangente                            | tan       | ![tan](../screenshots/operateurs/tan.PNG)             |
| asin      | Arc sinus                           | asin      | ![asin](../screenshots/operateurs/asin.PNG)           |
| acos      | Arc cosinus                         | acos      | ![acos](../screenshots/operateurs/acos.PNG)           |
| atan      | Arc tangente                        | atan      | ![atan](../screenshots/operateurs/atan.PNG)           |

### Opérateurs de Comparaison

Les opérateurs de comparaison sont utilisés pour comparer des variables et des valeurs.

| Opérateur | Description         | Nom           | Image                                                         |
|-----------|---------------------|---------------|---------------------------------------------------------------|
| ==        | Égal à              | equal         | ![equal](../screenshots/operateurs/equal.PNG)                 |
| !=        | Différent de        | notEqual      | ![notEqual](../screenshots/operateurs/notEqual.PNG)           |
| &&        | ET logique          | land          | ![land](../screenshots/operateurs/land.PNG)                   |
| <         | Inférieur à         | lessThan      | ![lessThan](../screenshots/operateurs/lessThan.PNG)           |
| <=        | Inférieur ou égal à | lessThanEq    | ![lessThanEq](../screenshots/operateurs/lessThanEq.PNG)       |
| \>        | Supérieur à         | greaterThan   | ![greaterThan](../screenshots/operateurs/greaterThan.PNG)     |
| \>=       | Supérieur ou égal à | greaterThanEq | ![greaterThanEq](../screenshots/operateurs/greaterThanEq.PNG) |
| ===       | Strictement égal à  | strictEqual   | ![strictEqual](../screenshots/operateurs/strictEqual.PNG)     |
| \|\|      | OU logique          | or            | ![or](../screenshots/operateurs/or.PNG)                       |
| &         | ET binaire          | and           | ![and](../screenshots/operateurs/and.PNG)                     |
| ^         | OU exclusif binaire | xor           | ![xor](../screenshots/operateurs/xor.PNG)                     |
| !         | Négation logique    | not           | ![not](../screenshots/operateurs/not.PNG)                     |

---

[Précédent](composants.md) | [🏠](../README.md) | [Suivant](commandes.md)
