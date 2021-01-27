# Agiilsed tarkvara metoodikad

## Feature branchid
### Uue branchi loomine. Tavaliselt kasutatakse branchi nimena:

- Esimene osa on tüüp (story - feature, bug - bugfix)
- Teine osa pileti number
```
git checkout -b feature/ABC-123
```

### Olemasolevale branchile minemine

```
git checkout feature/ABC-123
```

### Uute muudatuste endale alla tõmbamine

```
git pull
```

### Staatuse vaatamine

```
git status
```

### Failide lisamine enne commiti. Punktiga lisab kõik failid, milles muudatus tehtud

```
git add filename

git add .
```

### Commitimine - muudatuste "salvestamine" koos sõnumiga, mis muudatusi tehti. Lühendiga "-am" tehakse ka automaatselt "git add ." erinevusega, et uusi faile ei lisata commiti, ainult need, milles muudatus tehti.

```
git commit -m 'This is commit message'

git commit -am 'This is commit message'

git commit -am 'This is commit message' && git push
```

### Muudatuste lükkamine giti. Kui branch on juba olemas gitis, siis esimene variant, kui veel ei ole olemas siis teine variant.

```
git push

git push --set-upstream origin feature/ABC-123
```


## Merge conflicti lahendamine

### Olles oma branchil ilma uute muudatusteta, aga kõige uuem kood all, tuleks tõmmata sisse main või master (olenevalt nimetusest) branch.

Seda saab teha kas terminalis

```
git pull origin main

git pull origin master
```

või VSCode Source conrol vaates valides kolm punkti -> Pull, Push -> Pull from... -> siis valite origin -> origin/main

![VSCode source control](assets/source_control_1.png)
