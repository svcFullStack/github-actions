# github-actions

Ce dépôt contient les workflows réutilisable de l'équipe fullstack. 

Répertoire temporaire en attendant l'arrivé de github enterprise.

Documentation: https://docs.github.com/en/actions/using-workflows/reusing-workflows

---
exemple d'utilisation:
```
name: CI

on: [push, pull_request]

jobs:
  run:
    uses: svcFullStack/github-actions/.github/workflows/ci.yaml@main
    with:
      node-version: 16.14.0
```
### Attention le code doit être rétrocompatible car les répertoires LaCapitale/Beneva utilise la branche @main
