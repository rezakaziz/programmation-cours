---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# some information about your slides (markdown enabled)
title: Encapsulation et packages

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

Chapitre 3

</div>

# Encapsulation et packages

<div class="mt-4 text-xl text-gray-500">

Protéger les données et organiser les classes d'une application

</div>

<div class="mt-8 flex flex-nowrap items-center justify-center text-sm text-gray-500 whitespace-nowrap">

<span>Encapsulation</span>

<span class="text-gray-300 mx-2">•</span>

<span>Visibilité</span>

<span class="text-gray-300 mx-2">•</span>

<span>Accesseurs</span>

<span class="text-gray-300 mx-2">•</span>

<span>Mutateurs</span>

<span class="text-gray-300 mx-2">•</span>

<span>Packages</span>

</div>

</div>
---
layout: default
---

# Plan du chapitre

<div class="grid grid-cols-2 gap-4 mt-5">

<div class="border border-gray-200 rounded-lg p-3">

<div class="text-sm text-gray-400">
01
</div>

<div class="font-medium text-lg mt-1">
Encapsulation
</div>

<div class="text-sm text-gray-500 mt-1">
Contrôler l'accès à l'état interne d'un objet.
</div>

</div>

<div class="border border-gray-200 rounded-lg p-3">

<div class="text-sm text-gray-400">
02
</div>

<div class="font-medium text-lg mt-1">
Interface et implémentation
</div>

<div class="text-sm text-gray-500 mt-1">
Séparer ce qui est exposé de ce qui reste interne.
</div>

</div>

<div class="border border-gray-200 rounded-lg p-3">

<div class="text-sm text-gray-400">
03
</div>

<div class="font-medium text-lg mt-1">
Accesseurs et mutateurs
</div>

<div class="text-sm text-gray-500 mt-1">
Lire et modifier les données de manière contrôlée.
</div>

</div>

<div class="border border-gray-200 rounded-lg p-3">

<div class="text-sm text-gray-400">
04
</div>

<div class="font-medium text-lg mt-1">
Packages
</div>

<div class="text-sm text-gray-500 mt-1">
Organiser les classes selon leur rôle.
</div>

</div>

<div class="border border-gray-200 rounded-lg p-3">

<div class="text-sm text-gray-400">
05
</div>

<div class="font-medium text-lg mt-1">
Imports
</div>

<div class="text-sm text-gray-500 mt-1">
Utiliser des classes appartenant à d'autres packages.
</div>

</div>

<div class="border border-gray-200 rounded-lg p-3">

<div class="text-sm text-gray-400">
06
</div>

<div class="font-medium text-lg mt-1">
Visibilité et packages
</div>

<div class="text-sm text-gray-500 mt-1">
Comprendre les règles d'accès entre les classes.
</div>

</div>

</div>

---
src: ./pages/encapsulation.md
---
---
src: ./pages/getset.md
---
---
src: ./pages/packages.md
---
---
src: ./pages/imports.md
---
---
src: ./pages/visibilite.md
---
---
src: ./pages/synthese.md
---

