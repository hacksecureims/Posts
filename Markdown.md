# Écrire en Markdown

## Sommaire

- 
- 
- 

## Introduction

Le Markdown est un langage de balisage léger. Il a été créé dans le but d'offrir une syntaxe facile pour pouvoir écrire du code HTML plus rapidement. Toutes les balises Markdown ont un équivalent en HTML.

Presque toutes les applications Markdown prennent en charge la syntaxe de base. Mais il existe des variations et des divergences mineures entre les processeurs Markdown.

Le Markdown est principalement utilisé pour rédiger des commentaires et des documentations techniques, comme le fichier README dans les dépôts Github. 

## Syntaxe basique

### Titres

Pour créer un titre, ajoutez un dièse (#) devant un mot ou une phrase. Le nombre de dièse que vous utilisez doit correspondre au niveau de l'en-tête. Par exemple, pour créer un titre de niveau trois (`<h3>` en HTML), utilisez trois dièses (par exemple `### Mon titre`).

|Markdown|HTML|Rendu|
|---|---|---|
|# Titre niveau 1|`<h1>Titre niveau 1</h1>`|<h1>Titre niveau 1</h1>|
|# Titre niveau 2|`<h2>Titre niveau 2</h2>`|<h2>Titre niveau 2</h2>|
|# Titre niveau 3|`<h3>Titre niveau 3</h3>`|<h3>Titre niveau 3</h3>|
|# Titre niveau 4|`<h4>Titre niveau 4</h4>`|<h4>Titre niveau 4</h4>|
|# Titre niveau 5|`<h5>Titre niveau 5</h5>`|<h5>Titre niveau 5</h5>|
|# Titre niveau 6|`<h6>Titre niveau 6</h6>`|<h6>Titre niveau 6</h6>|

#### Syntaxe alternative

|Markdown|HTML|Rendu|
|---|---|---|
|Titre niveau 1<br>==========|`<h1>Titre niveau 1</h1>`|<h1>Titre niveau 1</h1>|
|# Titre niveau 2<br>-----------------|`<h2>Titre niveau 2</h2>`|<h2>Titre niveau 2</h2>|

#### Meilleures pratiques à propos des titres

Les interpréteurs Markdowns ne sont pas d'accords sur la façon de prendre en charge les espaces manquants entre les dièses et les titres ou autres. Pour une meilleur compatibilité, mettez toujours un espace entre les caractères dièses et les titres.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|# Voici un titre|#Voici un titre|

De la même façon qu'il est mieux d'ajouter des lignes vides avant et après les titres pour une meilleure compatibilité.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|Une ligne vide avant...<br><br># Voici un titre<br><br>...et une après.|Sans les lignes vides<br>#Voici un titre<br>ça pourrait ne pas sembler bon.|

### Paragraphes

Pour créer des paragraphes, séparez votre texte par des lignes vides.

#### Meilleures pratiques à propos des paragraphes

Contrairement aux paragraphes dans les listes, il ne faut pas indenter les paragraphes avec des espaces/tabulations.

|✔️ À faire|❌ À ne pas faire|
|---|---|
|<p>Ne mettez pas de tabulations ou d'espaces.</p><p>Gardez les lignes alignées à gauche comme ça.</p>|<p>&nbsp;&nbsp;&nbsp;&nbsp;Cela peut entraîner des problèmes de formatage inattendus.</p><p>&nbsp;&nbsp;&nbsp;&nbsp;N'ajoutez pas de tabulations ou d'espaces devant les paragraphes.</p>|

### Sauts de ligne

Pour créer un saut de ligne (`<br>`), terminez une ligne par deux espaces ou plus, puis tapez retour.

|Markdown|HTML|Rendu|
|---|---|---|
|Je suis la première ligne.<br>Je suis la deuxième ligne. |`<p>Je suis la première ligne<br><p>Je suis la deuxième ligne</p>`|<p>Je suis la première ligne<br><p>Je suis la deuxième ligne</p>|

#### Meilleures pratiques à propos des sauts de lignes

Vous pouvez donc utiliser deux espaces ou plus (appelés "espaces blancs de fin de ligne") pour les sauts de ligne dans presque toutes les applications Markdown mais cette pratique est controversée. Il est difficile de voir les espaces en fin de ligne dans un éditeur et de nombreuses personnes mettent accidentellement ou intentionnellement deux espaces après chaque phrase. Il est donc préférable d'utiliser autre chose. Si l'application Markdown prend en charge l'HTML, vous pouvez utiliser le balise HTML `<br>`.<br><br>
Pour des raisons de compatibilité, il vaut mieux utiliser cette balise à la fin de la ligne.<br><br>
Il y a d'autres options mais non recommandées :<br>Certains langages dérivés permettent de taper une barre oblique inversée à la fin de la ligne (`\`) et d'autres permettent de taper `return` pour un créer un saut de ligne.

# My first HackMD note (change me!)

###### tags: `Tag(change me!)`

> This note is yours, feel free to play around.  :video_game: 
> Type on the left :arrow_left: and see the rendered result on the right. :arrow_right: 

## :memo: Where do I start?

### Step 1: Change the title and add a tag

- [x] Create my first HackMD note (this one!)
- [ ] Change its title
- [ ] Add a tag

:rocket: 

### Step 2: Write something in Markdown

Let's try it out!
Apply different styling to this paragraph:
**HackMD gets everyone on the same page with Markdown.** ==Real-time collaborate on any documentation in markdown.== Capture fleeting ideas and formalize tribal knowledge.

- [x] **Bold**
- [ ] *Italic*
- [ ] Super^script^
- [ ] Sub~script~
- [ ] ~~Crossed~~
- [x] ==Highlight==

:::info
:bulb: **Hint:** You can also apply styling from the toolbar at the top :arrow_upper_left: of the editing area.

![](https://i.imgur.com/Cnle9f9.png)
:::

> Drag-n-drop image from your file system to the editor to paste it!

### Step 3: Invite your team to collaborate!

Click on the <i class="fa fa-share-alt"></i> **Sharing** menu :arrow_upper_right: and invite your team to collaborate on this note!

![permalink setting demo](https://i.imgur.com/PjUhQBB.gif)

- [ ] Register and sign-in to HackMD (to use advanced features :tada: ) 
- [ ] Set Permalink for this note
- [ ] Copy and share the link with your team

:::info
:pushpin: Want to learn more? ➜ [HackMD Tutorials](https://hackmd.io/c/tutorials) 
:::

---

## BONUS: More cool ways to HackMD!

- Table

| Features          | Tutorials               |
| ----------------- |:----------------------- |
| GitHub Sync       | [:link:][GitHub-Sync]   |
| Browser Extension | [:link:][HackMD-it]     |
| Book Mode         | [:link:][Book-mode]     |
| Slide Mode        | [:link:][Slide-mode]    | 
| Share & Publish   | [:link:][Share-Publish] |

[GitHub-Sync]: https://hackmd.io/c/tutorials/%2Fs%2Flink-with-github
[HackMD-it]: https://hackmd.io/c/tutorials/%2Fs%2Fhackmd-it
[Book-mode]: https://hackmd.io/c/tutorials/%2Fs%2Fhow-to-create-book
[Slide-mode]: https://hackmd.io/c/tutorials/%2Fs%2Fhow-to-create-slide-deck
[Share-Publish]: https://hackmd.io/c/tutorials/%2Fs%2Fhow-to-publish-note

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
- Auto-generated Table of Content
[ToC]

> Leave in-line comments! [color=#3b75c6]

- Embed YouTube Videos

{%youtube PJuNmlE74BQ %}

> Put your cursor right behind an empty bracket {} :arrow_left: and see all your choices.

- And MORE ➜ [HackMD Tutorials](https://hackmd.io/c/tutorials)
