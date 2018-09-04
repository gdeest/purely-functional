# Programmation _purement_ fonctionnelle
## Interagir avec le monde réel sans quitter la tour d'ivoire

---

# Fonctions pures

Une fonction dont le résultat ne dépend que de ses arguments.

*Exemple:*

```C
int f(int x, int y) {
  return 2*x+y;
}
```

Les fonctions pures sont _l'essence_ de la programmation fonctionnelle.

--- 

# Fonctions impures

Une fonction dont le résultat est aussi influencé par un état implicite.

*Exemple:*

```C
int z = 0;
int f(int x) {
  z = 2*x + z;
  return ret;
}
```

- Premier appel: `f(1) = 2`
- Deuxième appel: `f(1) = 4`
