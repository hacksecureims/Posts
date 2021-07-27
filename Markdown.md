# Écrire en Markdown

# Sommaire

- 
- 
- 

# Introduction

Le Markdown est un langage de balisage léger. Il a été créé dans le but d'offrir une syntaxe facile pour pouvoir écrire du code HTML plus rapidement. Toutes les balises Markdown ont un équivalent en HTML.

Presque toutes les applications Markdown prennent en charge la syntaxe de base. Mais il existe des variations et des divergences mineures entre les processeurs Markdown.

Le Markdown est principalement utilisé pour rédiger des commentaires et des documentations techniques, comme le fichier README dans les dépôts Github. 

# Syntaxe basique

## Les titres

Pour créer un titre, ajoutez un dièse (#) devant un mot ou une phrase. Le nombre de dièse que vous utilisez doit correspondre au niveau de l'en-tête. Par exemple, pour créer un titre de niveau trois (`<h3>` en HTML), utilisez trois dièses (par exemple `### Mon titre`).

|Markdown|HTML|Rendu|
|---|---|---|
|# Titre niveau 1|`<h1>Titre niveau 1</h1>`|<h1>Titre niveau 1</h1>|
|# Titre niveau 2|`<h2>Titre niveau 2</h2>`|<h2>Titre niveau 2</h2>|
|# Titre niveau 3|`<h3>Titre niveau 3</h3>`|<h3>Titre niveau 3</h3>|
|# Titre niveau 4|`<h4>Titre niveau 4</h4>`|<h4>Titre niveau 4</h4>|
|# Titre niveau 5|`<h5>Titre niveau 5</h5>`|<h5>Titre niveau 5</h5>|
|# Titre niveau 6|`<h6>Titre niveau 6</h6>`|<h6>Titre niveau 6</h6>|

### Syntaxe alternative

|Markdown|HTML|Rendu|
|---|---|---|
|Titre niveau 1<br>==========|`<h1>Titre niveau 1</h1>`|<h1>Titre niveau 1</h1>|
|Titre niveau 2<br>-----------------|`<h2>Titre niveau 2</h2>`|<h2>Titre niveau 2</h2>|

### Meilleures pratiques à propos des titres

Les interpréteurs Markdowns ne sont pas d'accords sur la façon de prendre en charge les espaces manquants entre les dièses et les titres ou autres. Pour une meilleur compatibilité, mettez toujours un espace entre les caractères dièses et les titres.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|# Voici un titre|#Voici un titre|

De la même façon qu'il est mieux d'ajouter des lignes vides avant et après les titres pour une meilleure compatibilité.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|Une ligne vide avant...<br><br># Voici un titre<br><br>...et une après.|Sans les lignes vides<br>#Voici un titre<br>ça pourrait ne pas sembler bon.|

## Les paragraphes

Pour créer des paragraphes, séparez votre texte par des lignes vides.

### Meilleures pratiques à propos des paragraphes

Contrairement aux paragraphes dans les listes, il ne faut pas indenter les paragraphes avec des espaces/tabulations.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|<p>Ne mettez pas de tabulations ou d'espaces.</p><p>Gardez les lignes alignées à gauche comme ça.</p>|<p>&nbsp;&nbsp;&nbsp;&nbsp;Cela peut entraîner des problèmes de formatage inattendus.</p><p>&nbsp;&nbsp;&nbsp;&nbsp;N'ajoutez pas de tabulations ou d'espaces devant les paragraphes.</p>|

## Les sauts de ligne

Pour créer un saut de ligne (`<br>`), terminez une ligne par deux espaces ou plus, puis tapez retour.

|Markdown|HTML|Rendu|
|---|---|---|
|Je suis la première ligne.<br>Je suis la deuxième ligne. |`<p>Je suis la première ligne<br><p>Je suis la deuxième ligne</p>`|<p>Je suis la première ligne<br><p>Je suis la deuxième ligne</p>|

### Meilleures pratiques à propos des sauts de lignes

Vous pouvez donc utiliser deux espaces ou plus (appelés "espaces blancs de fin de ligne") pour les sauts de ligne dans presque toutes les applications Markdown mais cette pratique est controversée. Il est difficile de voir les espaces en fin de ligne dans un éditeur et de nombreuses personnes mettent accidentellement ou intentionnellement deux espaces après chaque phrase. Il est donc préférable d'utiliser autre chose. Si l'application Markdown prend en charge l'HTML, vous pouvez utiliser le balise HTML `<br>`.<br><br>
Pour des raisons de compatibilité, il vaut mieux utiliser cette balise à la fin de la ligne.<br><br>
Il y a d'autres options mais non recommandées :<br>Certains langages dérivés permettent de taper une barre oblique inversée à la fin de la ligne (`\`) et d'autres permettent de taper `return` pour un créer un saut de ligne, mais encore une fois, il ne vaut mieux pas les utiliser pour des raisons de compatibilités.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|First line with the HTML tag after.<br>And the next line.|First line with a backslash after. \ And the next line.|

## L'accentuation

Vous pouvez ajouter de l'emphase (accentuation) pour mettre votre texte en gras ou en italique.

### Texte en gras

Pour mettre votre texte en gras, ajouter deux astérisques (`**`) ou deux tirets bas (`__`) avant et après votre mot ou votre phrase. Pour mettre en gras seulement le milieu d'un mot, ajoutez deux astérisques sans espaces autour des lettres.

|Markdown|HTML|Rendu|
|---|---|---|
|`Texte en **gras**`|`Texte en <strong>gras</strong>`|Texte en **gras**|
|`Texte en __gras__`|`Texte en <strong>gras</strong>`|Texte en __gras__|
|`Texte**en**gras`|`Texte<strong>en</strong>gras`|Texte**en**gras|

### Meilleures pratiques à propos des caractères gras

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`Texte**en**gras`|`Texte__en__gras`|

### Texte en italique

Pour mettre votre texte en italique, ajouter un astérisque(`*`) ou un tiret bas (`_`) avant et après votre mot ou votre phrase. Pour mettre en italique seulement le milieu d'un mot, ajoutez un astérisque sans espaces autour des lettres.

|Markdown|HTML|Rendu|
|---|---|---|
|`Texte en *italique*`|`Texte en <em>italique</em>`|Texte en *italique*|
|`Texte en _italique_`|`Texte en <em>italique</em>`|Texte en _italique_|
|`Texte*en*gras`|`Texte<em>en</em>italique`|Texte*en*italique|

### Meilleures pratiques à propos des caractères gras

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`Texte*en*gras`|`Texte_en_gras`|

### Texte en gras ET en italique

Pour mettre votre texte en gras et en italique, ajouter trois astérisques (`***`) ou trois tirets bas (`___`) avant et après votre mot ou votre phrase. Pour mettre en gras et en italique seulement le milieu d'un mot, ajoutez trois astérisques sans espaces autour des lettres.

|Markdown|HTML|Rendu|
|---|---|---|
|`Texte très ***important***`|`Texte très <strong><em>important</em></strong>`|Texte très ***important***|
|`Texte très ___important___`|`Texte très <strong><em>important</em></strong>`|Texte très ___important___|
|`Texte très __*important*__`|`Texte très <strong><em>important</em></strong>`|Texte très __*important*__|
|`Texte très **_important_**`|`Texte très <strong><em>important</em></strong>`|Texte très **_important_**|
|`Texte***très***important`|`Texte<strong><em>très</em></strong>important`|Texte***très***important|

### Meilleures pratiques à propos des caractères gras

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`Texte***très***important`|`Texte___très___important`|

## Les citations

Pour créer une citation, il suffit d'ajouter `>` devant le paragraphe.

`> Le principe de l'évolution est beaucoup plus rapide en informatique que chez le bipède.`

donnera : 

> Le principe de l'évolution est beaucoup plus rapide en informatique que chez le bipède.

### Citation avec plusieurs paragraphes

Les blocs de citations peuvent contenir plusieurs paragraphes. Il faut ajouter un chevron (`>`) entre chaque paragraphe.

```
> Le principe de l'évolution est beaucoup plus rapide en informatique que chez le bipède.
>
> Quelle prétention de prétendre que l'informatique est récente : Adam et Eve avaient déjà un Apple !
```

donnera : 

> Le principe de l'évolution est beaucoup plus rapide en informatique que chez le bipède.
>
> Quelle prétention de prétendre que l'informatique est récente : Adam et Eve avaient déjà un Apple !

### Citation imbriquée

Les blocs de citations peuvent être imbriqués. Ajouter deux chevrons (`>>`) devant la citation que vous voulez imbriquer.

```
> Le principe de l'évolution est beaucoup plus rapide en informatique que chez le bipède.
>
>> Quelle prétention de prétendre que l'informatique est récente : Adam et Eve avaient déjà un Apple !
```

donnera : 

> Le principe de l'évolution est beaucoup plus rapide en informatique que chez le bipède.
>
>> Quelle prétention de prétendre que l'informatique est récente : Adam et Eve avaient déjà un Apple !

### Citation avec d'autres éléments

La plupart des éléments Markdown peuvent contenir d'autres éléments Markdown, mais pas tous. Il faut tester différentes combinaisons.

```
> ### Liste de course
> 
> - Clé USB
> - **Adhésion SAFIR**
> - Fruits (*peut être*)
>> par John Doe
```

donnera : 

> ### Liste de course
> 
> - Clé USB
> - **Adhésion SAFIR**
>   - Fruits (*peut être*)

### Meilleures pratiques à propos des citations

Par soucis de compatibilité, ajoutez toujours des lignes vides avant et après les citations.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`bla bla avant`<br><br>`> Ceci est une citation`<br><br>`bla bla après`|`bla bla avant`<br>`> Ceci est une citation`<br>`bla bla après`|

## Les listes

Vous pouvez organiser les éléments en listes ordonnées et non ordonnées.

### Liste ordonnée

Les listes ordonnées commencent par des nombres suivis d'un point. Les nombres n'ont pas besoin d'être dans l'ordre numérique. Certaines applications ont besoin que la liste commence par 1.

|Markdown|HTML|Rendu|
|---|---|---|
|`1. Un`<br>`2. Deux`<br>`3. Trois`<br>`4. Quatre`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ol>`|<ol><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ol>|
|`1. Un`<br>`1. Deux`<br>`1. Trois`<br>`1. Quatre`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ol>`|<ol><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ol>|
|`1. Un`<br>`8. Deux`<br>`3. Trois`<br>`5. Quatre`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ol>`|<ol><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ol>|
|`1. Un`<br>`2. Deux`<br>&nbsp;&nbsp;&nbsp;&nbsp;`1. UnUn`<br>&nbsp;&nbsp;&nbsp;&nbsp;`2. DeuxDeux`<br>`3. Trois`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<ol>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li>UnUn</li>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li>DeuxDeux</li>`<br>`</ol>`<br>`<li>Trois</li>`<br>`</ol>`|<ol><li>Un</li><li>Deux</li><ol><li>UnUn</li><li>DeuxDeux</li></ol><li>Trois</li></ol>|

### Meilleures pratiques à propos des listes ordonnées

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`1. First item`<br>`2. Second item`|`1) First item`<br>`2) Second item`|

### Liste non ordonnée

Les listes non ordonnées commencent soit par des tirets (`-`), soit par des astérisques (`*`), soit par des plus (`+`) devant les lignes. Vous pouvez indenter un ou plusieurs items pour créer une liste imbriquée.

|Markdown|HTML|Rendu|
|---|---|---|
|`- Un`<br>`- Deux`<br>`- Trois`<br>`- Quatre`|`<ul>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ul>`|<ul><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ul>|
|`* Un`<br>`* Deux`<br>`* Trois`<br>`* Quatre`|`<ul>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ul>`|<ul><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ul>|
|`+ Un`<br>`+ Deux`<br>`+ Trois`<br>`+ Quatre`|`<ul>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ul>`|<ul><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ul>|
|`- Un`<br>`- Deux`<br>&nbsp;&nbsp;&nbsp;&nbsp;`- UnUn`<br>&nbsp;&nbsp;&nbsp;&nbsp;`- DeuxDeux`<br>`- Trois`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<ol>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li>UnUn</li>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li>DeuxDeux</li>`<br>`</ol>`<br>`<li>Trois</li>`<br>`</ol>`|<ul><li>Un</li><li>Deux</li><ul><li>UnUn</li><li>DeuxDeux</li></ul><li>Trois</li></ul>|

### Meilleures pratiques à propos des listes non ordonnées

Encore une fois, les applications Markdown ne gèrent pas toutes de la même façon les différents délimiteurs dans la même liste. Pour une meilleure compatibilité, ne mélangez pas les délimiteurs dans la même liste. Choisissez en un et gardez le.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`- Un`<br>`- Deux`<br>`- Trois`<br>`- Quatre`|`+ Un`<br>`* Deux`<br>`- Trois`<br>`+ Quatre`|

[ SUITE A VENIR ]