
# Dupliquer un dépôt

v0.0.1

## Théorie

```bash
git clone --bare le-depot-a-cloner
cd le-depot-a-cloner.git
git push --mirror depot-destination
```

## Exemple pratique

- Créer le nouveau dépôt !
- `git clone --bare https://github.com/chris-scientist/git-test-repo.git`
- `cd git-test-repo.git`
- `git push --mirror https://github.com/chris-scientist4learning/git-test-new-repo.git`

### Voir les dépôts GitHub

- [Dépôt d'origine](https://github.com/chris-scientist/git-test-repo)
- [Dépôt dupliqué](https://github.com/chris-scientist4learning/git-test-new-repo)
