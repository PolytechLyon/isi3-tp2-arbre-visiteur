**Nom/Prénom Etudiant 1 :**

**Nom/Prénom Etudiant 2 :**

# Rapport TP2

## Question 1
*Insérer un schéma du patron de conception mis en place*

## Question 2
Nous avons dans cette question implémenté le pattern visitor définit par le diagramme UML de la question 1. 
Pour ce faire nous avons dû créer deux interface : `Vistable` et `Visitor`. En effet ces deux interfaces vont nous permettre de dire tel ou tel classe est visitable par tel visiteur.  Ainsi les classes `Addition`, `Multiplication`, `Negation` et `Constante` doivent être visitables. On remarque que toutes nos classes précédemment citées sont filles de l'élément Node. En rendant alors `Node` de type visitable par un héritage de l'interface `Visitable` nous rendons toutes ses classes filles visitables.
Nos opérations étant maintenant visitables elle doivent toutes implémenter une fonction `accept` afin d'accepter la visite d'un visiteur. Exemple d'une fonction accept : 
```java
    public int accept(Visitor visitor) {
        return visitor.visit(this);
    }
```
Comme on peut le voir cette fonction se contente de renvoyer l'instance de la classe où elle se trouve à la fonction `visit`.
Ainsi par la suite nous pourrons créer des classes de type visiteur ayant des fonctions `visit` pour chaque classe visitable.
Ces fonctions `visit` nous permettrons de réaliser le traitement voulu en fonction du type de l'instance. 

## Question 3
*Expliquer le code ajouté*

## Question 4
*Expliquer le code ajouté*

## Question 5
*Expliquer le code ajouté*

## Question 6
*Expliquer le code ajouté*
