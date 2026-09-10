---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# some information about your slides (markdown enabled)
title: Classes et Objets

# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
# duration of the presentation
duration: 35min

src: ./pages/page-garde.md
---
layout: default
---

<div class="absolute inset-0 flex flex-col items-center justify-center text-center">

<div class="text-sm uppercase tracking-widest text-gray-400 mb-5">
Chapitre 2
</div>

# Classes et objets

<div class="mt-4 text-xl text-gray-500">
Passer du modèle à la création et à la manipulation d'objets
</div>

<div class="mt-8 text-sm text-gray-500">
Classes
<span class="text-gray-300 mx-3">•</span>
Objets
<span class="text-gray-300 mx-3">•</span>
Références
<span class="text-gray-300 mx-3">•</span>
Tableaux d'objets
</div>

</div>
---
layout: default
---

# Plan du chapitre

<div class="mt-3 text-lg">


</div>

<div class="grid grid-cols-2 gap-5 mt-6">

<div class="border border-gray-200 rounded-lg p-4">

<div class="text-sm text-gray-400">
01
</div>

<div class="font-medium text-lg mt-2">
Notion de classe
</div>

<div class="text-sm text-gray-500 mt-2">
Définir la structure et le comportement d'un type d'objet.
</div>

</div>

<div class="border border-gray-200 rounded-lg p-4">

<div class="text-sm text-gray-400">
02
</div>

<div class="font-medium text-lg mt-2">
Notion d'objet
</div>

<div class="text-sm text-gray-500 mt-2">
Créer des instances et manipuler leur état.
</div>

</div>

<div class="border border-gray-200 rounded-lg p-4">

<div class="text-sm text-gray-400">
03
</div>

<div class="font-medium text-lg mt-2">
Notion de référence
</div>

<div class="text-sm text-gray-500 mt-2">
Comprendre comment une variable permet d'accéder à un objet.
</div>

</div>

<div class="border border-gray-200 rounded-lg p-4">

<div class="text-sm text-gray-400">
04
</div>

<div class="font-medium text-lg mt-2">
Notion de constructeur
</div>

<div class="text-sm text-gray-500 mt-2">
Initialiser un objet au moment de sa création.
</div>

</div>

</div>

<div class="border border-gray-200 rounded-lg p-4 mt-5 text-center">

<div class="text-sm text-gray-400">
05
</div>

<div class="font-medium text-lg mt-2">
Membres et méthodes <code>static</code>
</div>

<div class="text-sm text-gray-500 mt-2">
Distinguer ce qui appartient à un objet de ce qui appartient à la classe.
</div>

</div>


---
src: ./pages/class.md
---
---
src: ./pages/objet.md
---
---
src: ./pages/reference.md
---
---
src: ./pages/constructeur.md
---
---
src: ./pages/static.md
---
---
layout: default
---

# ⚠️ Une limite de notre classe actuelle

<div class="mt-3 text-lg">

Pour l'instant, les attributs de nos objets peuvent être modifiés directement depuis l'extérieur de la classe.

</div>

```java
Point p = new Point(3, 5);

p.x = 100;
p.y = -50;
```

<div class="mt-5 text-center text-gray-500">

Le code extérieur peut donc modifier directement l'état de l'objet.

</div>

<div class="mt-5 px-5 py-4 bg-gray-50 rounded-lg text-center">

Cette possibilité nous a permis de découvrir simplement les classes et les objets,

mais ce n'est généralement <strong>pas une bonne pratique</strong>.

</div>

<div class="border-t border-gray-200 mt-6 pt-4 text-center font-medium">

Dans le prochain cours, nous verrons comment <strong>protéger les attributs</strong> et contrôler leur accès grâce à l'<strong>encapsulation</strong>.

</div>