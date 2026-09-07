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
src: ./pages/class.md
---
---
src: ./pages/getset.md
---
---
layout: default
---

# À retenir : les classes

<div class="mt-4 text-lg text-center">

Une <strong>classe</strong> permet de regrouper les données et les opérations qui concernent un même concept.

</div>

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="border border-gray-200 rounded-lg p-5 text-center">

<div class="text-xl font-medium">
📦 Attributs
</div>

<div class="mt-3 text-gray-600">

Décrivent les <strong>données</strong> de la classe.

</div>

<div class="mt-3">
<code>x</code> · <code>y</code>
</div>

</div>

<div class="border border-gray-200 rounded-lg p-5 text-center">

<div class="text-xl font-medium">
⚙️ Méthodes
</div>

<div class="mt-3 text-gray-600">

Décrivent les <strong>opérations</strong> disponibles.

</div>

<div class="mt-3">
<code>deplacer()</code>
</div>

</div>

<div class="border border-gray-200 rounded-lg p-5 text-center">

<div class="text-xl font-medium">
🔒 Encapsulation
</div>

<div class="mt-3 text-gray-600">

Permet de <strong>protéger les données</strong> et de contrôler leur accès.

</div>

<div class="mt-3">
<code>private</code> · <code>public</code>
</div>

</div>

</div>

<div class="border-t border-gray-200 mt-7 pt-5 text-center text-lg font-medium">

Une classe définit une <strong>structure</strong> et des <strong>comportements</strong>.

</div>

<div class="mt-4 text-center text-gray-500">

Mais comment utiliser concrètement cette classe dans un programme ? → <strong>Les objets</strong>

</div>
---
src: ./pages/objet.md
---
---
src: ./pages/reference.md
---
---
src: ./pages/constructeur.md
---