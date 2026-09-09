---
layout: default
---

# Exercice de synthèse

<div class="mt-3 text-lg">

Notre application bancaire contient maintenant plusieurs classes.

</div>

<div class="grid grid-cols-2 gap-8 mt-5">

<div>

### Organisation du projet

```text
projet/
├── banque/
│   ├── CompteBancaire.java
│   └── Client.java
│
└── application/
    └── Main.java
```

<div class="text-sm text-gray-500 mt-3">

`CompteBancaire` possède un `solde` privé et propose `getSolde()`, `deposer()` et `retirer()`.

</div>

</div>

<div class="border-l border-gray-200 pl-8">

### À vous de jouer

1. Quel `package` déclarer dans chaque classe ?

2. Quel `import` est nécessaire dans `Main` ?

3. Le `solde` doit-il être `private`, package-private ou `public` ?

4. Depuis `Main`, quels accès sont autorisés ?

```java
compte.solde
compte.getSolde()
compte.deposer(100)
```

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-4 text-center font-medium">

Justifiez chaque réponse à partir des règles étudiées dans le chapitre.

</div>
---
layout: default
---

# Correction : exercice de synthèse

<div class="grid grid-cols-2 gap-8 mt-4">

<div>

### `CompteBancaire.java`

```java
package banque;

public class CompteBancaire {

    private double solde;

    public double getSolde() {
        return solde;
    }

    public void deposer(double montant) {
        solde += montant;
    }
}
```

### `Main.java`

```java
package application;

import banque.CompteBancaire;
```

</div>

<div class="border-l border-gray-200 pl-8">

### Depuis `Main`

<div class="mt-4">

❌ `compte.solde`

<div class="text-sm text-gray-500">
`solde` est `private`.
</div>

</div>

<div class="mt-5">

✓ `compte.getSolde()`

<div class="text-sm text-gray-500">
La méthode est `public`.
</div>

</div>

<div class="mt-5">

✓ `compte.deposer(100)`

<div class="text-sm text-gray-500">
L'opération est `public`.
</div>

</div>

</div>

</div>

<div class="border-t border-gray-200 mt-4 pt-3 text-center font-medium">

`Main` connaît la classe grâce à l'`import`, mais accède uniquement à son interface publique.

</div>

---
layout: default
---

# A retenir : Bonnes pratiques

<div class="mt-3 text-lg">

Quelques règles simples pour concevoir des classes bien encapsulées et organiser son programme.

</div>

<div class="grid grid-cols-4 gap-4 mt-6">

<div class="border border-gray-200 rounded-lg p-4">

### 🔒 Attributs

<strong>Tous les attributs doivent être <code>private</code>.</strong>

<div class="text-sm text-gray-500 mt-2">

L'état reste sous le contrôle de l'objet.

</div>

</div>

<div class="border border-gray-200 rounded-lg p-4">

### 🎯 Méthodes

Rendre <code>public</code> uniquement les méthodes nécessaires.

<div class="text-sm text-gray-500 mt-2">

Limiter l'interface exposée.

</div>

</div>

<div class="border border-gray-200 rounded-lg p-4">

### 🔧 Getters / setters

Ne pas les créer systématiquement pour chaque attribut.

<div class="text-sm text-gray-500 mt-2">

Les ajouter seulement si nécessaire.

</div>

</div>

<div class="border border-gray-200 rounded-lg p-4">

### 📦 Packages

Regrouper les classes ayant des responsabilités proches.

<div class="text-sm text-gray-500 mt-2">

Garder une organisation cohérente.

</div>

</div>

</div>

<div v-click class="border-t border-gray-200 mt-6 pt-4 text-center font-medium">

<strong>Protéger l'état · Limiter l'interface · Organiser les responsabilités</strong>

</div>
