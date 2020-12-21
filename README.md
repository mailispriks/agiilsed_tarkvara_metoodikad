# Agiilsed tarkvara metoodikad

Uue branchi loomine. Tavaliselt kasutatakse branchi nimena:
- Esimene osa on tüüp (story - feature, bug - bugfix)
- Teine osa pileti number
```
git checkout -b feature/ABC-123
```


Olemasolevale branchile minemine
```
git checkout feature/ABC-123
```


Uute muudatuste endale alla tõmbamine
```
git pull
```


Staatuse vaatamine
```
git status
```


Failide lisamine enne commiti. Punktiga lisab kõik failid, milles muudatus tehtud
```
git add filename

git add .
```


Commitimine - muudatuste "salvestamine" koos sõnumiga, mis muudatusi tehti. Lühendiga "-am" tehakse ka automaatselt "git add ." erinevusega, et uusi faile ei lisata commiti, ainult need, milles muudatus tehti.
```
git commit -m 'This is commit message'

git commit -am 'This is commit message'
```


Muudatuste lükkamine giti. Kui branch on juba olemas gitis, siis esimene variant, kui veel ei ole olemas siis teine variant.
```
git push

git push --set-upstream origin feature/ABC-123
```
