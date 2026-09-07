---
layout: default
---

# Qu'est-ce qu'un objet ?

<div class="mt-4 text-lg">
Un <b>objet</b> représente une entité identifiable du problème que l'on souhaite modéliser.
</div>

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="text-center">
<div class="text-3xl font-bold text-gray-300">01</div>

### Identité

Permet de distinguer un objet des autres.

<span class="text-sm text-gray-500">
Compte d'Alice ≠ Compte de Bob
</span>
</div>

<div class="text-center">
<div class="text-3xl font-bold text-gray-300">02</div>

### État

Ensemble des données qui décrivent l'objet.

`titulaire = "Alice"`  
`solde = 1000`
</div>

<div class="text-center">
<div class="text-3xl font-bold text-gray-300">03</div>

### Comportements

Actions que l'objet peut réaliser.

`deposer()`  
`retirer()`
</div>

</div>

<div class="border-t border-gray-200 mt-8 pt-5 text-center">

### Un objet : Identité + État + Comportements

</div>
---
layout: default
---

# Exemples d'objets



<div class="grid grid-cols-3 gap-5 mt-6">

<div class="border border-gray-200 rounded-lg p-4">

### 🏦 compteAlice

<b>Identité :</b>  
`compteAlice`

<b>État :</b>  
`solde = 1000`  
`titulaire = "Alice"`

<b>Comportements :</b>  
`deposer()` · `retirer()`

</div>

<div class="border border-gray-200 rounded-lg p-4">

### 🏦 compteAlice

<b>Identité :</b>  
`compteBob`

<b>État :</b>  
`solde = 500`  
`titulaire = "Bob"`

<b>Comportements :</b>  
`deposer()` · `retirer()`

</div>

<div class="border border-gray-200 rounded-lg p-4">

### 🚗 voiturePaul

<b>Identité :</b>  
`voiturePaul`

<b>État :</b>  
`vitesse = 50`  
`carburant = 70%`

<b>Comportements :</b>  
`accelerer()` · `freiner()`

</div>



</div>



<div class="border-t border-gray-200 mt-5 pt-4 text-center">

`compteAlice` et `compteBob` ont un <b>état différent</b>,
mais partagent les mêmes <b>attributs</b> et <b>comportements</b>.

<div class="mt-3 text-lg font-medium">
Ils peuvent donc être décrits par un <b>même modèle : la classe</b>.
</div>
</div>

---
layout: default
---

# Qu'est-ce qu'une classe ?

<div class="mt-4 text-lg">
Une <b>classe</b> est un modèle qui décrit les caractéristiques
communes à un ensemble d'objets.
</div>

<div class="mt-6 flex justify-center">

```mermaid {theme: 'neutral', scale: 0.75}
classDiagram
    class NomClasse {
        attribut1
        attribut2
        operation1()
        operation2()
    }
```

</div>

<div class="grid grid-cols-2 gap-10 mt-5 text-center">

<div>

### Attributs

Décrivent les <b>données</b>  
qui constituent l'état d'un objet (son état) .

</div>

<div class="border-l border-gray-200">

### Opérations

Décrivent les <b>comportements</b>  
que les objets peuvent réaliser.

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-4 text-center font-medium">

### Classe : modèle commun pour créer des objets

</div>

---
layout: default
---

# Exemple : une classe, plusieurs objets

<div class="mt-2 text-lg">
Une même <b>classe</b> peut être instanciée plusieurs fois.
Chaque objet possède alors son <b>propre état</b>.
</div>

<div class="mt-3 flex justify-center">

```mermaid {theme: 'neutral', scale: 0.48}
classDiagram
    class CompteBancaire {
        titulaire : String
        solde : double
        deposer(montant)
        retirer(montant)
    }
```

</div>

<div class="text-center text-gray-300 text-2xl -mt-1">
↓ &nbsp;&nbsp;&nbsp; instanciation &nbsp;&nbsp;&nbsp; ↓
</div>

<div class="grid grid-cols-3 gap-5 mt-2">

<div class="border border-gray-300 rounded-lg p-3 text-center">

### compteAlice

<div class="text-sm text-gray-500">
Instance de <b>CompteBancaire</b>
</div>

<div class="border-t border-gray-200 my-2"></div>

`titulaire = "Alice"`  
`solde = 1500`

</div>

<div class="border border-gray-300 rounded-lg p-3 text-center">

### compteBob

<div class="text-sm text-gray-500">
Instance de <b>CompteBancaire</b>
</div>

<div class="border-t border-gray-200 my-2"></div>

`titulaire = "Bob"`  
`solde = 800`

</div>

<div class="border border-gray-300 rounded-lg p-3 text-center">

### compteCharlie

<div class="text-sm text-gray-500">
Instance de <b>CompteBancaire</b>
</div>

<div class="border-t border-gray-200 my-2"></div>

`titulaire = "Charlie"`  
`solde = 2300`

</div>

</div>

<div class="border-t border-gray-200 mt-4 pt-3 text-center font-medium">

<b>1 classe</b>
<span class="text-gray-300 mx-3">→</span>
<b>3 instances</b>
<span class="text-gray-300 mx-3">→</span>
même structure, <b>états différents</b>

</div>