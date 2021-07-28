# Écrire en Markdown

# Sommaire

- 
- 
- 

# Introduction

Le Markdown est un langage de balisage léger. Il a été créé dans le but d'offrir une syntaxe facile pour pouvoir écrire du code HTML plus rapidement. Toutes les balises Markdown ont un équivalent en HTML.

Presque toutes les applications Markdown prennent en charge la syntaxe de base. Mais il existe des variations et des divergences mineures entre les processeurs Markdown.

Le Markdown est principalement utilisé pour rédiger des commentaires et des documentations techniques, comme le fichier README dans les dépôts Github. 

# Les titres

Pour créer un titre, ajoutes un dièse (#) devant un mot ou une phrase. Le nombre de dièse que tu utilises doit correspondre au niveau de l'en-tête. Par exemple, pour créer un titre de niveau trois (`<h3>` en HTML), utilises trois dièses (par exemple `### Mon titre`).

|Markdown|HTML|Rendu|
|---|---|---|
|# Titre niveau 1|`<h1>Titre niveau 1</h1>`|<h1>Titre niveau 1</h1>|
|# Titre niveau 2|`<h2>Titre niveau 2</h2>`|<h2>Titre niveau 2</h2>|
|# Titre niveau 3|`<h3>Titre niveau 3</h3>`|<h3>Titre niveau 3</h3>|
|# Titre niveau 4|`<h4>Titre niveau 4</h4>`|<h4>Titre niveau 4</h4>|
|# Titre niveau 5|`<h5>Titre niveau 5</h5>`|<h5>Titre niveau 5</h5>|
|# Titre niveau 6|`<h6>Titre niveau 6</h6>`|<h6>Titre niveau 6</h6>|

## Syntaxe alternative

|Markdown|HTML|Rendu|
|---|---|---|
|Titre niveau 1<br>==========|`<h1>Titre niveau 1</h1>`|<h1>Titre niveau 1</h1>|
|Titre niveau 2<br>-----------------|`<h2>Titre niveau 2</h2>`|<h2>Titre niveau 2</h2>|

## Meilleures pratiques à propos des titres

Les interpréteurs Markdowns ne sont pas d'accords sur la façon de prendre en charge les espaces manquants entre les dièses et les titres ou autres. Pour une meilleur compatibilité, mets toujours un espace entre les caractères dièses et les titres.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|# Voici un titre|#Voici un titre|

De la même façon qu'il est mieux d'ajouter des lignes vides avant et après les titres pour une meilleure compatibilité.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|Une ligne vide avant...<br><br># Voici un titre<br><br>...et une après.|Sans les lignes vides<br>#Voici un titre<br>ça pourrait ne pas sembler bon.|

# Les paragraphes

Pour créer des paragraphes, séparez votre texte par des lignes vides.

## Meilleures pratiques à propos des paragraphes

Contrairement aux paragraphes dans les listes, il ne faut pas indenter les paragraphes avec des espaces/tabulations.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|<p>Ne mettez pas de tabulations ou d'espaces.</p><p>Gardez les lignes alignées à gauche comme ça.</p>|<p>&nbsp;&nbsp;&nbsp;&nbsp;Cela peut entraîner des problèmes de formatage inattendus.</p><p>&nbsp;&nbsp;&nbsp;&nbsp;N'ajoutez pas de tabulations ou d'espaces devant les paragraphes.</p>|

# Les sauts de ligne

Pour créer un saut de ligne (`<br>`), terminez une ligne par deux espaces ou plus, puis tapez retour.

|Markdown|HTML|Rendu|
|---|---|---|
|Je suis la première ligne.<br>Je suis la deuxième ligne. |`<p>Je suis la première ligne<br><p>Je suis la deuxième ligne</p>`|<p>Je suis la première ligne<br><p>Je suis la deuxième ligne</p>|

## Meilleures pratiques à propos des sauts de lignes

Vous pouvez donc utiliser deux espaces ou plus (appelés "espaces blancs de fin de ligne") pour les sauts de ligne dans presque toutes les applications Markdown mais cette pratique est controversée. Il est difficile de voir les espaces en fin de ligne dans un éditeur et de nombreuses personnes mettent accidentellement ou intentionnellement deux espaces après chaque phrase. Il est donc préférable d'utiliser autre chose. Si l'application Markdown prend en charge l'HTML, vous pouvez utiliser le balise HTML `<br>`.<br><br>
Pour des raisons de compatibilité, il vaut mieux utiliser cette balise à la fin de la ligne.<br><br>
Il y a d'autres options mais non recommandées :<br>Certains langages dérivés permettent de taper une barre oblique inversée à la fin de la ligne (`\`) et d'autres permettent de taper `return` pour un créer un saut de ligne, mais encore une fois, il ne vaut mieux pas les utiliser pour des raisons de compatibilités.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|First line with the HTML tag after.<br>And the next line.|First line with a backslash after. \ And the next line.|

# L'accentuation

Vous pouvez ajouter de l'emphase (accentuation) pour mettre votre texte en gras ou en italique.

## Texte en gras

Pour mettre votre texte en gras, ajouter deux astérisques (`**`) ou deux tirets bas (`__`) avant et après votre mot ou votre phrase. Pour mettre en gras seulement le milieu d'un mot, ajoutez deux astérisques sans espaces autour des lettres.

|Markdown|HTML|Rendu|
|---|---|---|
|`Texte en **gras**`|`Texte en <strong>gras</strong>`|Texte en **gras**|
|`Texte en __gras__`|`Texte en <strong>gras</strong>`|Texte en __gras__|
|`Texte**en**gras`|`Texte<strong>en</strong>gras`|Texte**en**gras|

## Meilleures pratiques à propos des caractères gras

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`Texte**en**gras`|`Texte__en__gras`|

## Texte en italique

Pour mettre votre texte en italique, ajouter un astérisque(`*`) ou un tiret bas (`_`) avant et après votre mot ou votre phrase. Pour mettre en italique seulement le milieu d'un mot, ajoutez un astérisque sans espaces autour des lettres.

|Markdown|HTML|Rendu|
|---|---|---|
|`Texte en *italique*`|`Texte en <em>italique</em>`|Texte en *italique*|
|`Texte en _italique_`|`Texte en <em>italique</em>`|Texte en _italique_|
|`Texte*en*gras`|`Texte<em>en</em>italique`|Texte*en*italique|

## Meilleures pratiques à propos des caractères gras

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`Texte*en*gras`|`Texte_en_gras`|

## Texte en gras ET en italique

Pour mettre votre texte en gras et en italique, ajouter trois astérisques (`***`) ou trois tirets bas (`___`) avant et après votre mot ou votre phrase. Pour mettre en gras et en italique seulement le milieu d'un mot, ajoutez trois astérisques sans espaces autour des lettres.

|Markdown|HTML|Rendu|
|---|---|---|
|`Texte très ***important***`|`Texte très <strong><em>important</em></strong>`|Texte très ***important***|
|`Texte très ___important___`|`Texte très <strong><em>important</em></strong>`|Texte très ___important___|
|`Texte très __*important*__`|`Texte très <strong><em>important</em></strong>`|Texte très __*important*__|
|`Texte très **_important_**`|`Texte très <strong><em>important</em></strong>`|Texte très **_important_**|
|`Texte***très***important`|`Texte<strong><em>très</em></strong>important`|Texte***très***important|

## Meilleures pratiques à propos des caractères gras

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`Texte***très***important`|`Texte___très___important`|

# Les citations

Pour créer une citation, il suffit d'ajouter `>` devant le paragraphe.

`> Le principe de l'évolution est beaucoup plus rapide en informatique que chez le bipède.`

donnera : 

> Le principe de l'évolution est beaucoup plus rapide en informatique que chez le bipède.

## Citation avec plusieurs paragraphes

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

## Citation imbriquée

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

## Citation avec d'autres éléments

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

> ## Liste de course
> 
> - Clé USB
> - **Adhésion SAFIR**
>   - Fruits (*peut être*)

## Meilleures pratiques à propos des citations

Par soucis de compatibilité, ajoutez toujours des lignes vides avant et après les citations.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`bla bla avant`<br><br>`> Ceci est une citation`<br><br>`bla bla après`|`bla bla avant`<br>`> Ceci est une citation`<br>`bla bla après`|

# Les listes

Vous pouvez organiser les éléments en listes ordonnées et non ordonnées.

## Liste ordonnée

Les listes ordonnées commencent par des nombres suivis d'un point. Les nombres n'ont pas besoin d'être dans l'ordre numérique. Certaines applications ont besoin que la liste commence par 1.

|Markdown|HTML|Rendu|
|---|---|---|
|`1. Un`<br>`2. Deux`<br>`3. Trois`<br>`4. Quatre`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ol>`|<ol><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ol>|
|`1. Un`<br>`1. Deux`<br>`1. Trois`<br>`1. Quatre`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ol>`|<ol><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ol>|
|`1. Un`<br>`8. Deux`<br>`3. Trois`<br>`5. Quatre`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ol>`|<ol><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ol>|
|`1. Un`<br>`2. Deux`<br>&nbsp;&nbsp;&nbsp;&nbsp;`1. UnUn`<br>&nbsp;&nbsp;&nbsp;&nbsp;`2. DeuxDeux`<br>`3. Trois`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<ol>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li>UnUn</li>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li>DeuxDeux</li>`<br>`</ol>`<br>`<li>Trois</li>`<br>`</ol>`|<ol><li>Un</li><li>Deux</li><ol><li>UnUn</li><li>DeuxDeux</li></ol><li>Trois</li></ol>|

## Meilleures pratiques à propos des listes ordonnées

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`1. First item`<br>`2. Second item`|`1) First item`<br>`2) Second item`|

## Liste non ordonnée

Les listes non ordonnées commencent soit par des tirets (`-`), soit par des astérisques (`*`), soit par des plus (`+`) devant les lignes. Vous pouvez indenter un ou plusieurs items pour créer une liste imbriquée.

|Markdown|HTML|Rendu|
|---|---|---|
|`- Un`<br>`- Deux`<br>`- Trois`<br>`- Quatre`|`<ul>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ul>`|<ul><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ul>|
|`* Un`<br>`* Deux`<br>`* Trois`<br>`* Quatre`|`<ul>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ul>`|<ul><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ul>|
|`+ Un`<br>`+ Deux`<br>`+ Trois`<br>`+ Quatre`|`<ul>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<li>Trois</li>`<br>`<li>Quatre</li>`<br>`</ul>`|<ul><li>Un</li><li>Deux</li><li>Trois</li><li>Quatre</li></ul>|
|`- Un`<br>`- Deux`<br>&nbsp;&nbsp;&nbsp;&nbsp;`- UnUn`<br>&nbsp;&nbsp;&nbsp;&nbsp;`- DeuxDeux`<br>`- Trois`|`<ol>`<br>`<li>Un</li>`<br>`<li>Deux</li>`<br>`<ol>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li>UnUn</li>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li>DeuxDeux</li>`<br>`</ol>`<br>`<li>Trois</li>`<br>`</ol>`|<ul><li>Un</li><li>Deux</li><ul><li>UnUn</li><li>DeuxDeux</li></ul><li>Trois</li></ul>|

## Meilleures pratiques à propos des listes non ordonnées

Encore une fois, les applications Markdown ne gèrent pas toutes de la même façon les différents délimiteurs dans la même liste. Pour une meilleure compatibilité, ne mélangez pas les délimiteurs dans la même liste. Choisissez en un et gardez le.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`- Un`<br>`- Deux`<br>`- Trois`<br>`- Quatre`|`+ Un`<br>`* Deux`<br>`- Trois`<br>`+ Quatre`|

# Ajouter un élément à une liste 

Pour ajouter un élément à une liste tout en préservant la continuité de la liste, indentes l'élément de 4 espaces ou d'une tabulation.

## Ajouter un paragraphe

```MD
* Première ligne
* Deuxième ligne

    Ajouter un paragraphe

* Troisième ligne
```

Le rendu ressemble à ceci :
***

* Première ligne
* Deuxième ligne

    Ajouter un paragraphe

* Troisième ligne
***

## Ajouter une citation

```MD
* Première ligne
* Deuxième ligne

    > Ajouter un paragraphe

* Troisième ligne
```

Le rendu ressemble à ceci :
***

* Première ligne
* Deuxième ligne

    > Ajouter un paragraphe

* Troisième ligne
***

## Ajouter un bloc de code

```MD
1. Première ligne
2. Deuxième ligne

        <html>
            <head>
                <title>Test</title>
            </head>

3. Troisième ligne
```

Le rendu ressemble à ceci :
***

1. Ouvres le fichier .html.
2. Trouves ce bloc de code à la ligne 21: 

        <html>
            <head>
                <title>Test</title>
            </head>

3. Modifies en fonction de ton titre.

***

## Ajouter une image

```MD
1. Trouver un logo
2. Voici le logo

    ![Le logo SAFIR](./img/logo_safir.png)

3. Utiliser le logo
```

Le rendu ressemble à ceci :

***

1. Trouver un logo
2. Voici le logo

    ![Le logo SAFIR](./img/logo_safir.ico)

3. Utiliser le logo

***

## Ajouter une liste

```MD
1. Trouver un logo
2. Voici le logo

    - ligne indentée
    - ligne indentée

3. Utiliser le logo
```

Le rendu ressemble à ceci :

***

1. Trouver un logo
2. Voici le logo

    - ligne indentée
    - ligne indentée

3. Utiliser le logo

***

# Code

Pour signaler qu'un mot ou qu'une phrase est du code, entoures la d'accents graves ou backticks (`` ` ``).

|Markdown|HTML|Rendu|
|---|---|---|
|``Dans le cmd, tapez `nano` ``|`Dans le cmd, tapez <code>nano</code>`|Dans le cmd, tapez `nano`|

## Échapper les backticks

Si le mot ou la phrase que tu veux désigner comme code comprend un ou plusieurs backticks, tu peux l'échapper en entourant le mot ou la phrase de doubles backticks (``).

|Markdown|HTML|Rendu|
|---|---|---|
|``` ``Utilisez `code` dans les fichiers md``  ```|``<code>Utilisez `code` dans les fichiers md</code>``| ``Utilisez `code` dans les fichiers md``  |

# Bloc de code

Pour créer un bloc de code, il y a deux façons de faire. Soit tu indentes chaque ligne d'au moins 4 espaces ou d'une tabulation, soit tu utilises 3 backticks comme ci-dessous.

```
    <html>
        <head>
        </head>
    </html>
```
```
    ```HTML
    <html>
        <head>
        </head>
    </html>
    ```
```

Le rendu ressemble à ceci :

***

    <html>
        <head>
        </head>
    </html>

```HTML
<html>
    <head>
    </head>
</html>
```

***

Comme tu l'as vu, tu peux ajouter le langage souhaité après les 3 premiers backticks pour avoir une coloration syntaxique. Cela fonctionne uniquement dans les blocs de code compris entre les 3 backticks.

```
    ```CSS
    .btn {
        background-color: #ffffff;
    }
    ```
```

```
    ```PY
    import requests

    def main():
        print("HelloWorld")
    ```
```

```
    ```TS
    export class AccountService {

        constructor(private http: HttpClient) { }

        httpOptions = {
            headers: new HttpHeaders({ 'Content-Type': 'application/json'})
        };

        registerAccount(newUser: User) {
            const url = environment.api_base_url + "/auth/local/register";
            return this.http.post(url, newUser, this.httpOptions);
        }
    }
    ```
```

Le rendu ressemble à ceci :

***

```CSS
.btn {
    background-color: #ffffff;
}
```

```PY
import requests

def main():
    print("HelloWorld")
```

```TS
export class AccountService {

    constructor(private http: HttpClient) { }

    httpOptions = {
        headers: new HttpHeaders({ 'Content-Type': 'application/json'})
    };

    registerAccount(newUser: User) {
        return this.http.post(url, newUser, this.httpOptions);
    }
}
```

***

Tu peux trouver dans la documentation de Markdown les langages supportés.

# Séparation horizontale

Pour créer une séparation horizontale, utilises soit 3 astérisques (`***`), 3 tirets ou plusieurs tirets (`---`) du bas sur toute une ligne (`_______`)

```
***

---

_____________

Le rendu ressemble à ceci :

```

***
---
_______________________

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`Mettez une ligne vide avant ...`<br><br>`---`<br><br>`... et une après.`|`Sans les lignes vides, l'élément deviendrait un titre.`<br>`---`<br>`Donc ne faites pas ça!`|

# Les liens

Pour créer un lien, entoures le titre du lien dans des crochets (ex: [Google]) et ajoutes directement après le lien entre parenthèses (`[Google](https://google.com)`)

`Mon site préféré est [SAFIR](http://safir.univ-reims.fr)`

Le rendu ressemble à ceci :
> Mon site préféré est [SAFIR](http://safir.univ-reims.fr)

Tu peux aussi lier un élément de la même page à un lien. 
Tu dois d'abord créer un identifiant personnalisé sur tes titres. Certaines applications Markdown les ajoute automatiquement.

Pour en ajouter, tu dois simplement ajouter l'identifiant personnalisé après le titre ` ### First {#first} ` puis y faire référence `[link to first](#first)`

Le rendu ressemble à ceci :

> ### First
>
> Bla bla bla
>
> - [link to first](#first)

## Ajouter des info-bulles

Tu peux aussi ajouter des info-bulles qui apparaîtront en passant sur le lien. Pour se faire, rajoutes le texte du tooltip après le lien qui se trouve entre les parenthèses

`[SAFIR](http://safir.univ-reims.fr "Le site officiel SAFIR")`

Le rendu ressemble à ceci :

> [SAFIR](http://safir.univ-reims.fr "Le site officiel SAFIR")

## URLs et adresses mail

Pour créer un lien à partir d'une URL ou d'une adresse mail, entoures là de chevrons.

***La majorité des applications Markdown le font nativement, donc pas forcément besoins des chevrons.***

```
<http://safir.univ-reims.fr>
<contact@safir.univ-reims.fr>

http://safir.without-chevrons.fr>
contact@safir.without-chevrons.fr
```

Le rendu ressemble à ceci : 

> <http://safir.univ-reims.fr> <br>
> <contact@safir.univ-reims.fr> <br><br>
> http://safir.without-chevrons.fr <br>
> contact@safir.without-chevrons.fr

## Formatage des liens

Le formatage habituel fonctionne aussi sur les liens.

```
Le site du **[Master RT](https://master-reseaux-telecom-reims.fr/)**.
Tu peux retrouver ces astuces sur le *[guide Markdown](https://www.markdownguide.org)*.
Et même faire du [`code`](#code)
```

> Le site du **[Master RT](https://master-reseaux-telecom-reims.fr/)**. <br>
> Tu peux retrouver ces astuces sur le *[guide Markdown](https://www.markdownguide.org)*. <br>
> Et même faire du [`code`](#code) clickable.

# Liens par référence
Les liens par référence sont un style de lien particulier qui simplifie l'affichage et la lecture des liens dans le Markdown. Ils sont construits en deux parties : la partie que tu gardes en ligne avec ton texte et la partie que tu stockes ailleurs dans le fichier pour que le texte reste facile à lire. 

## Formatage de la première partie du lien

La première partie du lien se décompose en deux ensembles de crochets. Le premier ensemble contient le texte qui doit être lié. Le second contient le label utilisé pour pointer vers le lien stocké ailleurs dans le document.

Il peut y avoir un espace entre ces deux parties. Le deuxième ensemble est insensible à la casse et peut contenir des lettres, des chiffres, des espaces ou des signes de ponctuation. 

```
[tutoriel][1]
[tutoriel] [1]
```

## Formatage de la seoncde partie du lien

La seconde partie du lieu est formaté avec les attributs suivants : 

1. Le label
    - Entre crochets, suivi directement de deux points et d'au moins un espace (ex: `[label]: `).
2. L'URL
    - Le lien qui peut être entouré de chevrons.
3. Le titre optionnel pour le lien
    - Peut être entouré de simple ou doubles guillemets ou de parenthèses.

Les formats suivants sont donc équivalents : 

```
[1]: https://fr.wikipedia.org/wiki/Informatique#Histoire
[1]: https://fr.wikipedia.org/wiki/Informatique#Histoire "Histoire de l'informatique"
[1]: https://fr.wikipedia.org/wiki/Informatique#Histoire 'Histoire de l'informatique'
[1]: https://fr.wikipedia.org/wiki/Informatique#Histoire (Histoire de l'informatique)
[1]: <https://fr.wikipedia.org/wiki/Informatique#Histoire> "Histoire de l'informatique"
[1]: <https://fr.wikipedia.org/wiki/Informatique#Histoire> 'Histoire de l'informatique'
[1]: <https://fr.wikipedia.org/wiki/Informatique#Histoire> (Histoire de l'informatique)
```

Tu peux placer ces lignes n'importe où dans ton document Markdown. Certains le préfère directement après le paragraphe où il est appelé, d'autres le préfèrent à la toute fin du document.

## Les deux parties ensemble

Disons que vous voulez mettre une URL avec la méthode basique dans un paragraphe : 

```
Les dieux de ce panthéon existent du fait du grand dieu non évoqué, qu'on peut assimiler au Destin. Le panthéon nordique se divise d'abord en deux groupes de divinités : les Ases et les [Vanes](https://fr.wikipedia.org/wiki/Vanes "Page Wikipedia sur les Vanes"). La guerre entre les Ases et les Vanes se termine par l'union des deux groupes de dieux.
```

Bien qu'en tant que lecteur on puisse clicker sur le lien comme d'habitude, le texte brut est un peu compliqué à lire étant donné les différentes parties. Mais si on utilise les liens par référence, voici ce que cela donnerait : 

```
Les dieux de ce panthéon existent du fait du grand dieu non évoqué, qu'on peut assimiler au Destin. Le panthéon nordique se divise d'abord en deux groupes de divinités : les Ases et les [Vanes][1]. La guerre entre les Ases et les Vanes se termine par l'union des deux groupes de dieux.

[1]: <https://fr.wikipedia.org/wiki/Vanes> "Vanes"
```

Dans les deux exemples ci dessus, le rendu est le même : 
> Les dieux de ce panthéon existent du fait du grand dieu non évoqué, qu'on peut assimiler au Destin. Le panthéon nordique se divise d'abord en deux groupes de divinités : les Ases et les [Vanes][1]. La guerre entre les Ases et les Vanes se termine par l'union des deux groupes de dieux.
>
> [1]: <https://fr.wikipedia.org/wiki/Vanes> "Vanes"

et l'HTML généré serait également le même :

`<a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles">hobbit-hole</a>`

## Meilleures pratiques à propos des liens

Par soucis de compatibilité, il vaut mieux encoder les caractères spéciaux dans les URLs, comme les espaces qui se transforment en `%20`.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|`[link](https://www.exemple.fr/un%20exemple/)`|`[link](https://www.exemple.fr/un exemple/`|

# Images

Pour ajouter une image, il faut ajouter un point d'exclamation (`!`) suivi du texte alternatif entre crochets et du chemin ou du lien vers l'image entre parenthèses. On peut également ajouter un titre optionnel entre guillemets après le lien, toujours dans les parenthèses.

`![Magnifique vue d'une forêt de sapins enneigés](./img/spruce_snow.jpg "Forêt de sapins enneigés)`

Ce qui ressemble à ceci :

***

![Forêt de sapins enneigés](./img/spruce_snow.jpg "Forêt de sapins enneigés")

***

# Image avec lien

Pour ajouter un lien dans une image, entoures la balise pour l'image dans des crochets et ajoutes ensuite le lien entre parenthèses. 

`[!Une plaine](./img/plain.jpg "Click me!")](https://discord.gg/T2vM2Tu)`

Ce qui ressenble à 

***

[![Une plaine](./img/plain.jpg "Click me!")](https://discord.gg/T2vM2Tu)

***

# Échappement de caractères

Comme dans beaucoup de situations, tu peux échapper certains caractères pour qu'ils n'aient pas d'influence dans le Markdown. Pour se faire, ajoutes un backslash (`\`) devant le caractère.

`\* Sans le backslash, cette phrase serait le début d'une liste`

ce qui donne 

> \* Sans le backslash, cette phrase serait le début d'une liste

Voici une liste des caractères que tu peux échapper :

``\\ \` \* \_ \{ \} \[ \] \< \> \( \) \# \+ \- \. \! \|``

# HTML
Certaines applications Markdown permettent l'utilisation des balises HTML. C'est utile pour certaines personnes qui préfèrent la syntaxe HTML pour les images. Les balises HTML sont aussi utiles pour changer la couleur du texte ou changer la taille d'une image. 

Par contre, pour des raisons de sécurité, toutes les applications Markdown ne le supportent pas. Si vous souhaitez tout de même utiliser les balises HTML, il faut séparer les blocs comme `<div>` ou `<table>` du contenu autour par des lignes vides. Il vaut mieux ne pas indenter ces balises car elles pourraient interférer avec le formatage Markdown. 

De plus, il n'est pas possible d'utiliser du Markdown à l'intérieur des balises HTML<br>
`Par exemple, <p>italique et **gras**</p> ne fonctionnera pas`.

# Syntaxe étendue

Les prochaines sections peuvent ne pas fonctionner sur toutes les applications Markdown. 

## Section dépliable

Pour se faire, utilises la balise HTML `<details>` et `<summary>`.

```
> ### Exemple
> <details>
>   <summary>Clic pour déplier</summary>
>   
>   #### Un sous titre
>   1. Une liste
>   2. **La suite**
>       - avec une
>       - sous liste
> </details>
```

Ce qui donnera : 

> ### Exemple
> <details>
>   <summary>Clic pour déplier</summary>
>   
>   #### Un sous titre
>   1. Une liste
>   2. **La suite**
>       - avec une
>       - sous liste
> </details>

## Notes de bas de page

```
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
```

Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.

## LaTeX

- LaTeX for formulas

$$
x = {-b \pm \sqrt{b^2-4ac} \over 2a}
$$

- Code block with color and line numbers：
```javascript=16
var s = "JavaScript syntax highlighting";
alert(s);
```

- UML diagrams
```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
Note left of Alice: Alice responds
Alice->Bob: Where have you been?
```