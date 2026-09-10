---
layout: default
---

# Du problème à la solution

<div class="mt-6 text-lg">
Pour résoudre un problème, il ne suffit pas d'écrire du code.
</div>

<div class="flex items-center justify-center gap-3 mt-8">

<div class="text-center w-38">
  <div class="text-3xl font-bold text-gray-300">01</div>
  <div class="font-bold mt-2">Analyser</div>
  <div class="text-sm text-gray-500 mt-2">
    Comprendre le problème et identifier les besoins
  </div>
</div>

<div class="text-2xl text-gray-300">→</div>

<div class="text-center w-38">
  <div class="text-3xl font-bold text-gray-300">02</div>
  <div class="font-bold mt-2">Concevoir</div>
  <div class="text-sm text-gray-500 mt-2">
    Imaginer et structurer une solution
  </div>
</div>

<div class="text-2xl text-gray-300">→</div>

<div class="text-center w-38">
  <div class="text-3xl font-bold text-gray-300">03</div>
  <div class="font-bold mt-2">Implémenter</div>
  <div class="text-sm text-gray-500 mt-2">
    Traduire la solution en programme
  </div>
</div>

<div class="text-2xl text-gray-300">→</div>

<div class="text-center w-38">
  <div class="text-3xl font-bold text-gray-300">04</div>
  <div class="font-bold mt-2">Tester</div>
  <div class="text-sm text-gray-500 mt-2">
    Vérifier que la solution répond au besoin
  </div>
</div>

</div>

<div class="border-t border-gray-200 mt-8 pt-4 text-center">

### Une bonne solution doit aussi être :

**Maintenable**
<span class="text-gray-300 mx-3">•</span>
**Évolutive**
<span class="text-gray-300 mx-3">•</span>
**Réutilisable**

</div>

<div class="mt-4 text-center text-gray-500">
Programmer n'est qu'une étape dans la construction d'un logiciel.
</div>

---
layout: default
---

# Le défi de la complexité logicielle

<div class="mt-4 text-lg">
À mesure qu'un logiciel évolue, sa complexité augmente.
</div>

<div class="flex items-start justify-center gap-3 mt-6">

<div class="w-40 text-center">
  <div class="text-2xl font-bold text-gray-300">01</div>
  <div class="font-bold mt-2">Le logiciel grandit</div>
  <div class="text-sm text-gray-500 mt-1">
    De nouvelles fonctionnalités et données sont ajoutées
  </div>
</div>

<div class="text-xl text-gray-300 mt-10">→</div>

<div class="w-40 text-center">
  <div class="text-2xl font-bold text-gray-300">02</div>
  <div class="font-bold mt-2">Les interactions augmentent</div>
  <div class="text-sm text-gray-500 mt-1">
    Les différentes parties deviennent dépendantes
  </div>
</div>

<div class="text-xl text-gray-300 mt-10">→</div>

<div class="w-40 text-center">
  <div class="text-2xl font-bold text-gray-300">03</div>
  <div class="font-bold mt-2">Les changements se propagent</div>
  <div class="text-sm text-gray-500 mt-1">
    Une modification peut affecter plusieurs parties
  </div>
</div>

<div class="text-xl text-gray-300 mt-10">→</div>

<div class="w-40 text-center">
  <div class="text-2xl font-bold">04</div>
  <div class="font-bold mt-2">La complexité augmente</div>
  <div class="text-sm text-gray-500 mt-1">
    Le système devient plus difficile à maîtriser
  </div>
</div>

</div>

<div class="border-t border-gray-200 mt-6 pt-4">

### Conséquences

<div class="grid grid-cols-2 gap-x-10 gap-y-2 mt-3">

<div>🧠 <b>Comprendre</b> : suivre la logique devient plus difficile</div>
<div>🔧 <b>Modifier</b> : anticiper les impacts devient plus difficile</div>
<div>🐛 <b>Corriger</b> : localiser les erreurs prend plus de temps</div>
<div>📈 <b>Faire évoluer</b> : ajouter sans casser devient plus difficile</div>

</div>

</div>

<div class="mt-5 text-center font-medium">
Le défi : <b>organiser le logiciel pour maîtriser cette complexité.</b>
</div>

---
layout: default
---

# Comment organiser un programme ?

<div class="mt-5 text-lg">
Pour maîtriser la complexité, il faut <b>structurer le programme</b>
et répartir clairement les responsabilités.
</div>

<div class="mt-6">

<div class="flex gap-5 items-start">
<div class="text-2xl font-bold text-gray-300">01</div>
<div>

### Décomposer

Diviser un problème complexe en **parties plus petites et plus simples à traiter**.

</div>
</div>

<div class="border-t border-gray-200 my-3"></div>

<div class="flex gap-5 items-start">
<div class="text-2xl font-bold text-gray-300">02</div>
<div>

### Répartir les responsabilités

Déterminer **le rôle de chaque partie** et éviter de concentrer toute la logique au même endroit.

</div>
</div>

<div class="border-t border-gray-200 my-3"></div>

<div class="flex gap-5 items-start">
<div class="text-2xl font-bold text-gray-300">03</div>
<div>

### Limiter les dépendances

Faire en sorte qu'une modification **affecte le moins possible le reste du programme**.

</div>
</div>

</div>

<div class="mt-5 text-center font-medium">
Ces choix dépendent notamment du <b>paradigme de programmation</b> utilisé.
</div>

---
layout: default
---

# Les paradigmes de programmation

<div class="mt-3 text-lg">
Un <b>paradigme de programmation</b> est une manière de
<b>penser et structurer</b> la résolution d'un problème.
</div>

<div class="grid grid-cols-2 gap-x-10 gap-y-5 mt-6">

<div>
<div class="flex items-start gap-4">
<div class="text-2xl font-bold text-gray-300">01</div>
<div>

### Programmation procédurale

Organise le programme autour de **procédures et de fonctions** qui manipulent des données.

<div class="text-sm text-gray-500 mt-2">
Fortran · C · Pascal
</div>

</div>
</div>
</div>

<div>
<div class="flex items-start gap-4">
<div class="text-2xl font-bold text-gray-300">02</div>
<div>

### Programmation fonctionnelle

Organise le calcul autour de **fonctions** et de transformations de données.

<div class="text-sm text-gray-500 mt-2">
Lisp · Scheme · Haskell
</div>

</div>
</div>
</div>

<div class="border-t border-gray-200 pt-4">
<div class="flex items-start gap-4">
<div class="text-2xl font-bold text-gray-300">03</div>
<div>

### Programmation logique

Décrit le problème à l'aide de **faits et de règles logiques**.

<div class="text-sm text-gray-500 mt-2">
Prolog · GHC
</div>

</div>
</div>
</div>

<div class="border-t border-gray-200 pt-4">
<div class="flex items-start gap-4">
<div class="text-2xl font-bold text-gray-300">04</div>
<div>

### Programmation orientée objet

Organise le programme autour d'**objets qui possèdent un état et des comportements**.

<div class="text-sm text-gray-500 mt-2">
Simula · Smalltalk · C++ · Java · C#
</div>

</div>
</div>
</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-3 text-center font-medium">
Un même problème peut être abordé selon <b>plusieurs paradigmes</b>.
</div>


---
layout: default
---

# Procédural vs Orienté Objet

<div class="mt-3 text-lg">
Deux façons différentes d'<b>organiser un programme</b>.
</div>

<div class="grid grid-cols-2 gap-10 mt-6">

<div>

### Programmation procédurale

<div class="flex items-center justify-center gap-6 mt-7">

<div class="border-2 border-gray-300 rounded-lg px-7 py-10 text-center font-bold">
Données
</div>

<div class="flex flex-col gap-3">

<div class="border border-gray-300 rounded px-5 py-2 text-center">
Fonction 1
</div>

<div class="border border-gray-300 rounded px-5 py-2 text-center">
Fonction 2
</div>

<div class="border border-gray-300 rounded px-5 py-2 text-center">
Fonction 3
</div>

</div>

</div>

<div class="mt-6 text-center text-sm text-gray-500">
Les <b>fonctions</b> manipulent des données<br>
organisées séparément.
</div>

</div>

<div class="border-l border-gray-200 pl-10">

### Programmation orientée objet

<div class="flex justify-center gap-3 mt-7">

<div class="border-2 border-gray-300 rounded-lg p-4 text-center">

<b>Objet 1</b>

<div class="border-t border-gray-200 my-2"></div>

Données

<div class="border-t border-gray-200 my-2"></div>

Comportements

</div>

<div class="flex items-center text-2xl text-gray-300">
↔
</div>

<div class="border-2 border-gray-300 rounded-lg p-4 text-center">

<b>Objet 2</b>

<div class="border-t border-gray-200 my-2"></div>

Données

<div class="border-t border-gray-200 my-2"></div>

Comportements

</div>

</div>

<div class="mt-6 text-center text-sm text-gray-500">
Les <b>objets</b> regroupent données et comportements<br>
et collaborent entre eux.
</div>

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-3 text-center font-medium">
<b>Procédural :</b> organiser autour des traitements
<span class="text-gray-300 mx-4">|</span>
<b>Objet :</b> organiser autour des objets
</div>
---
layout: default
---

# Un problème, plusieurs approches

<div class="h-[75%] flex flex-col justify-center">

<div class="text-center">

### Problème

<div class="mt-6 text-2xl font-light">
Concevoir un système de <b>gestion de comptes bancaires</b>
</div>

<div class="mt-5 text-lg text-gray-500">
Le système doit permettre d'effectuer des
<b>dépôts</b> et des <b>retraits</b> d'argent.
</div>

</div>

<div class="border-t border-gray-200 mt-10 pt-6 text-center">

### Comment organiser notre programme pour résoudre ce problème ?

<div class="mt-2 text-gray-500">
Nous allons comparer deux approches.
</div>

</div>

</div>


---
layout: default
---

# Première approche : organisation procédurale

<div class="mt-4 text-lg">
On commence par <b>séparer les données des traitements</b>.
</div>

<div class="grid grid-cols-2 gap-10 mt-6">

<div>

### 1 : Représenter les données

```text
structure Compte
    numero
    titulaire
    solde
fin
```

<div class="mt-3 text-sm text-gray-500">
Chaque compte est représenté par une structure contenant ses données.
</div>

</div>

<div class="border-l border-gray-200 pl-10">

### 2 : Définir les traitements

```text
créerCompte(numero, titulaire, solde)

deposer(compte, montant)

retirer(compte, montant)
```

<div class="mt-3 text-sm text-gray-500">
Les fonctions reçoivent le compte à manipuler et modifient ses données.
</div>

</div>

</div>

<div class="border-t border-gray-200 mt-7 pt-4 text-center">

### Organisation procédurale

<b>Structure de données</b>
<span class="text-gray-300 mx-3">+</span>
<b>Fonctions séparées</b>

</div>

---
layout: default
---

# Quand le système grandit...

<div class="mt-3 text-lg">
De nouveaux types de comptes apparaissent, chacun avec ses <b>propres règles métier</b>.
</div>

<div class="grid grid-cols-2 gap-10 mt-5">

<div>

### Les structures se spécialisent

```text
structure Compte
    numero
    solde
    type
    decouvert
    tauxInteret
fin
```

<div class="mt-3 text-sm text-gray-500">
Une même structure doit maintenant représenter
plusieurs types de comptes.
</div>

</div>

<div class="border-l border-gray-200 pl-10">

### Les traitements se complexifient

```text
deposer(compte, montant)

retirer(compte, montant)

calculerInterets(compte)

verifierDecouvert(compte)
```

<div class="mt-3 text-sm text-gray-500">
Chaque fonction doit tenir compte du
<b>type de compte</b> qu'elle manipule.
</div>

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-4 text-center">

<b>CompteCourant</b>
<span class="text-gray-300 mx-2">↔</span>
<b>Fonctions</b>
<span class="text-gray-300 mx-2">↔</span>
<b>CompteEpargne</b>

</div>

<div class="mt-4 text-center font-medium">
Plus les types se multiplient, plus les fonctions doivent intégrer
<b>des règles spécifiques à chaque type</b>.
</div>

---
layout: default
---

# La logique se complexifie...

<div class="mt-3 text-lg">
Une même fonction doit maintenant connaître les <b>règles de chaque type de compte</b>.
</div>

<div class="grid grid-cols-2 gap-10 mt-5">

<div>

### Exemple : retirer de l'argent

```text
fonction retirer(compte, montant)

    si compte.type = "courant"
        si solde + decouvert >= montant
            compte.solde -= montant
        fin

    sinon si compte.type = "epargne"
        si solde >= montant
            compte.solde -= montant
        fin
    fin
fin
```

</div>

<div class="border-l border-gray-200 pl-10">

### Le problème

<div class="mt-2">

<b>01 : La fonction connaît les types</b>

<div class="text-sm text-gray-500 mt-1">
Elle doit savoir si le compte est courant ou épargne.
</div>

<div class="border-t border-gray-200 my-3"></div>

<b>02 : Les règles sont mélangées</b>

<div class="text-sm text-gray-500 mt-1">
Les règles des différents comptes se retrouvent dans la même fonction.
</div>

<div class="border-t border-gray-200 my-3"></div>

<b>03 : Ajouter un type implique de modifier la fonction</b>

<div class="text-sm text-gray-500 mt-1">
Chaque nouveau type ajoute de nouvelles conditions.
</div>

</div>

</div>

</div>

<div class="border-t border-gray-200 mt-4 pt-3 text-center font-medium">
Plus de types
<span class="text-gray-300 mx-2">→</span>
plus de <code>if / else</code>
<span class="text-gray-300 mx-2">→</span>
<b>plus de complexité</b>
</div>

---
layout: default
---

# L'approche orientée objet

<div class="mt-3 text-lg">
L'idée : chaque type de compte <b>porte ses propres données et ses propres règles</b>.
</div>

<div class="grid grid-cols-2 gap-10 mt-5">

<div>

### CompteCourant

```text
CompteCourant
    numero
    solde
    decouvert

    deposer(montant)
    retirer(montant)
    verifierDecouvert()
```

<div class="mt-3 text-sm text-gray-500">
Le compte courant connaît ses propres règles de retrait.
</div>

</div>

<div class="border-l border-gray-200 pl-10">

### CompteEpargne

```text
CompteEpargne
    numero
    solde
    tauxInteret

    deposer(montant)
    retirer(montant)
    calculerInterets()
```

<div class="mt-3 text-sm text-gray-500">
Le compte épargne connaît ses propres règles.
</div>

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-4 text-center">

<b>Données</b>
<span class="text-gray-300 mx-2">+</span>
<b>Règles métier</b>
<span class="text-gray-300 mx-2">=</span>
<b>Objet responsable de son comportement</b>

</div>

<div class="mt-4 text-center font-medium">
On ne demande plus à une fonction de gérer tous les types :
<b>chaque objet sait comment se comporter.</b>
</div>
---
layout: default
---

# Pourquoi organiser en objets ?

<div class="mt-4 text-lg">
L'objectif n'est pas d'écrire moins de code, mais de
<b>mieux maîtriser sa structure</b>.
</div>

<div class="mt-6">

<div class="flex gap-5 items-start">
<div class="text-2xl font-bold text-gray-300">01</div>
<div>

### Localiser les responsabilités

Les données d'un compte et les opérations qui les concernent sont
<b>regroupées dans Compte</b>.

</div>
</div>

<div class="border-t border-gray-200 my-3"></div>

<div class="flex gap-5 items-start">
<div class="text-2xl font-bold text-gray-300">02</div>
<div>

### Limiter les dépendances

Les autres parties du programme n'ont pas besoin de connaître
<b>tous les détails internes du compte</b>.

</div>
</div>

<div class="border-t border-gray-200 my-3"></div>

<div class="flex gap-5 items-start">
<div class="text-2xl font-bold text-gray-300">03</div>
<div>

### Faciliter l'évolution

Une modification concernant le compte peut être
<b>principalement localisée dans Compte</b>.

</div>
</div>

</div>

<div class="mt-5 text-center font-medium">
POO : <b>regrouper les responsabilités pour mieux maîtriser la complexité.</b>
</div>

---
layout: default
---

# ⚠️ Un point important

<div class="mt-8 text-center">

<div class="text-2xl font-medium">
La complexification observée dans notre exemple ne signifie pas que
<b>la programmation procédurale est une mauvaise approche</b>.
</div>

<div class="mt-10 text-lg text-gray-600">

Nous avons simplement atteint une situation dans laquelle
<b>l'organisation choisie devient moins adaptée</b>
à l'évolution de notre problème.

</div>

</div>

<div  class="mt-10 flex justify-center">

<div class="border border-gray-200 rounded-lg px-8 py-5 text-center">

<b>Un paradigme est une manière d'organiser une solution.</b>

<div class="mt-2 text-gray-500">
Son intérêt dépend du problème, de sa complexité
et de la manière dont il doit évoluer.
</div>

</div>

</div>

<div  class="border-t border-gray-200 mt-8 pt-4 text-center font-medium">

L'objectif n'est donc pas de remplacer le procédural,
mais de découvrir <b>une autre manière d'organiser notre programme</b>.

</div>