---
layout: default
---

# Le getter

<div class="mt-3 text-lg">

Un <strong>getter</strong> permet de consulter une information.

</div>

<div class="grid grid-cols-2 gap-8 mt-5 items-center">

<div>

```java
class Point {
    private int x;

    public int getX() {
        return x;
    }
}
```

</div>

<div>

```java
Point p = new Point(3, 5);

int valeur = p.getX();
```

<div class="border border-gray-200 rounded-lg p-4 text-center mt-4">

<code>valeur = 3</code>

</div>

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-4 text-center font-medium">

Le getter fournit un accès en lecture sans exposer directement l'attribut.

</div>

---
layout: default
---

# Getters de `Point`

<div class="grid grid-cols-2 gap-8 mt-5 items-center">

<div>

```java
class Point {
    private int x;
    private int y;

    public int getX() {
        return x;
    }

    public int getY() {
        return y;
    }
}
```

</div>

<div class="space-y-4 text-center">

<div class="border border-gray-200 rounded-lg p-4">

<code>p.getX()</code>

<div class="text-sm text-gray-500 mt-2">

Consulte <code>x</code>

</div>

</div>

<div class="border border-gray-200 rounded-lg p-4">

<code>p.getY()</code>

<div class="text-sm text-gray-500 mt-2">

Consulte <code>y</code>

</div>

</div>

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-4 text-center font-medium">

Les coordonnées restent privées mais peuvent être consultées.

</div>

---
layout: default
---

# Modifier un attribut privé

<div class="mt-3 text-lg">

L'affectation directe reste interdite.

</div>

<div class="grid grid-cols-2 gap-8 mt-6 text-center">

<div class="border border-gray-200 rounded-lg p-4">

### Accès direct

```java
p.x = 8;
```

✗ Interdit

</div>

<div v-click class="border border-gray-200 rounded-lg p-4">

### Accès contrôlé

```java
p.setX(8);
```

✓ Via une méthode

</div>

</div>

<div v-click class="border-t border-gray-200 mt-6 pt-4 text-center font-medium">

Cette méthode est appelée un <strong>mutateur</strong>, ou <strong>setter</strong>.

</div>

---
layout: default
---

# Le setter

<div class="mt-3 text-lg">

Un <strong>setter</strong> permet de modifier un attribut privé.

</div>

<div class="grid grid-cols-2 gap-8 mt-5 items-center">

<div>

```java
class Point {
    private int x;

    public void setX(int x) {
        this.x = x;
    }
}
```

</div>

<div>

```java
Point p = new Point(3, 5);

p.setX(8);
```

<div class="border border-gray-200 rounded-lg p-4 text-center mt-4">

<code>x = 8</code>

</div>

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-4 text-center font-medium">

Le setter fournit un accès en modification.

</div>

---
layout: default
---

# Accesseurs et mutateurs

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="border border-gray-200 rounded-lg p-4">

### Accesseur — Getter

```java
public int getX() {
    return x;
}
```

<div class="text-center mt-3">

<strong>Consulter</strong> une information.

</div>

</div>

<div class="border border-gray-200 rounded-lg p-4">

### Mutateur — Setter

```java
public void setX(int x) {
    this.x = x;
}
```

<div class="text-center mt-3">

<strong>Modifier</strong> une information.

</div>

</div>

</div>

<div class="border-t border-gray-200 mt-6 pt-4 text-center font-medium">

La classe choisit les accès qu'elle souhaite fournir.

</div>

---
layout: default
---

# Contrôler une modification

<div class="mt-3 text-lg">

Passer par une méthode permet d'ajouter des règles.

</div>

<div class="grid grid-cols-2 gap-8 mt-5 items-center">

<div>

```java
public void setX(int x) {
    if (x > = 0) {
        this.x = x;
    }
}
```
<div class="border-t border-gray-200 mt-5 pt-4 text-center font-medium">

La classe garde le contrôle de son état.

</div>
</div>

<div class="space-y-4 text-center">

<div class="border border-gray-200 rounded-lg p-4">

### `setX(8)`

✓ Accepté

<code>x = 8</code>

</div>

<div class="border border-gray-200 rounded-lg p-4">

### `setX(-4)`

✗ Refusé

<code>x</code> reste inchangé

</div>

</div>

</div>



---
layout: default
---

# Faut-il toujours un setter ?

<div class="mt-3 text-lg">

Un attribut <code>private</code> n'a pas forcément besoin d'un setter.

</div>

<div class="grid grid-cols-2 gap-8 mt-6 text-center">

<div class="border border-gray-200 rounded-lg p-4">

### Modifier directement

```java
p.setX(8);
p.setY(6);
```

Le code choisit les nouvelles coordonnées.

</div>

<div class="border border-gray-200 rounded-lg p-4">

### Demander une opération

```java
p.deplacer(5, 1);
```

Le point contrôle son déplacement.

</div>

</div>

<div v-click class="border-t border-gray-200 mt-6 pt-4 text-center font-medium">

Encapsuler ne signifie pas ajouter systématiquement un setter à chaque attribut.

</div>

---
layout: default
---

# Une interface adaptée

<div class="grid grid-cols-2 gap-8 mt-5 items-center">

<div>

```java
class Point {
    private int x;
    private int y;

    public int getX() {
        return x;
    }

    public int getY() {
        return y;
    }

    public void deplacer(int dx, int dy) {
        x += dx;
        y += dy;
    }
}
```

</div>

<div class="space-y-4 text-center">

<div class="border border-gray-200 rounded-lg p-4">

### Consulter

<code>getX()</code>

<code>getY()</code>

</div>

<div class="border border-gray-200 rounded-lg p-4">

### Modifier

<code>deplacer()</code>

</div>

<div class="text-sm text-gray-500">

La classe expose uniquement les opérations utiles.

</div>

</div>

</div>

<div class="border-t border-gray-200 mt-5 pt-4 text-center font-medium">

L'interface publique décrit ce que l'objet permet de faire.

</div>

---
layout: default
---

# À retenir : encapsulation

<div class="grid grid-cols-2 gap-6 mt-7">

<div class="border border-gray-200 rounded-lg p-4">

### 🔒 `private`

Protège l'état interne.

</div>

<div class="border border-gray-200 rounded-lg p-4">

### 🌐 `public`

Expose les opérations accessibles.

</div>

<div class="border border-gray-200 rounded-lg p-4">

### 📤 Accesseur

Permet la consultation.

</div>

<div class="border border-gray-200 rounded-lg p-4">

### 📥 Mutateur

Permet une modification contrôlée.

</div>

</div>

<div class="border-t border-gray-200 mt-6 pt-4 text-center font-medium">

L'encapsulation permet à l'objet de contrôler l'accès et l'évolution de son état.

</div>

---
layout: default
---

# Exercice : encapsuler `CompteBancaire`

<div class="mt-3 text-lg">

Nous souhaitons représenter un compte bancaire en respectant le principe d'encapsulation.

</div>

<div class="grid grid-cols-2 gap-8 mt-5">

<div class="border border-gray-200 rounded-lg p-5">

### Le compte possède

- un <strong>titulaire</strong>
- un <strong>solde</strong>

<div class="mt-4 text-sm text-gray-500">

Le solde initial est fourni lors de la création du compte.

</div>

</div>

<div class="border border-gray-200 rounded-lg p-5">

### Le compte permet

- de consulter le solde
- de déposer une somme
- de retirer une somme

<div class="mt-4 text-sm text-gray-500">

Le solde ne doit pas pouvoir être fixé directement depuis l'extérieur.

</div>

</div>

</div>

<div class="mt-5 text-center font-medium">

Proposez la classe <code>CompteBancaire</code> correspondante.

</div>

<div v-click class="border-t border-gray-200 mt-5 pt-4 text-center">

Quels membres doivent être <code>private</code> ? Quels membres doivent être <code>public</code> ?

<br>

<strong>Faut-il fournir un setter pour le solde ?</strong>

</div>

---
layout: default
---

# Correction : `CompteBancaire`

<div class="grid grid-cols-2 gap-8 mt-3">

<div>

```java
public class CompteBancaire {

    private String titulaire;
    private double solde;

    public CompteBancaire(String titulaire, double solde) {
        this.titulaire = titulaire;
        this.solde = solde;
    }

    public double getSolde() {
        return solde;
    }

    public void deposer(double montant) {
        solde += montant;
    }

    public void retirer(double montant) {
        solde -= montant;
    }
}
```

</div>

<div class="border-l border-gray-200 pl-8">

### Choix d'encapsulation

<div class="mt-5">

**🔒 État interne**

`titulaire` et `solde` sont `private`.

</div>

<div class="mt-5">

**👁 Consultation**

`getSolde()` permet de consulter le solde.

</div>

<div class="mt-5">

**⚙️ Modification**

Le solde évolue avec `deposer()` et `retirer()`.

</div>

<div class="mt-5">

**🚫 Pas de `setSolde()`**

Le solde ne peut pas être fixé arbitrairement.

</div>

</div>

</div>