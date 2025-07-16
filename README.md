# Checkpoint-python-fonctions
# 🧮 Projet Python – Calculatrice Interactive

## 🎯 Objectif

Créer une application Python capable d’effectuer des **opérations arithmétiques de base** : addition, soustraction, multiplication et division.

---

## 📌 Description

L’application demande à l’utilisateur :
1. Deux **nombres**
2. Un **opérateur** parmi `+`, `-`, `*`, `/`

Elle applique l’opération choisie aux deux nombres et renvoie le **résultat**. Elle doit aussi :
- Gérer les **opérateurs non valides**
- Prévenir la **division par zéro**

---

## ✏️ Instructions

- Créer une fonction nommée `calculatrice(num1, num2)`
- À l’intérieur de la fonction :
  - Demander à l’utilisateur de saisir un opérateur
  - Utiliser des conditionnelles pour exécuter l’opération
  - Retourner le résultat
  - Afficher un message en cas d’erreur (division par zéro ou opérateur invalide)
- Appeler cette fonction avec deux valeurs et afficher le résultat
- Bonus : Ajouter une boucle ou des messages personnalisés pour améliorer l’expérience utilisateur

---

## 💻 Code Python réalisé

```python
def calculator(num1, num2):
    while True:
        opération = input("entrer un opérateur (+, -, *, /)")

        if opération == "+":
            return num1 + num2
        elif opération == "-":
            return num1 - num2
        elif opération == "*":
            return num1 * num2
        elif opération == "/":
            if num2 != 0:
                return num1 / num2
            else:
                return "erreur : ne peut pas être divisé par 0"
        else:
            print("entrer un opérateur valide")
