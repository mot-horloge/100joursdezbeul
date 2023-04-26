Lancer le projet localement:

```
npm install

npm run dev -- --open
```

Pour mettre à jour les données uniquement depuis le spreadsheet:
1. on met à jour le spreadsheet à la main
2. on l'export en CSV
3. on lance node ./scripts/csvToJSON/index.js fichier.csv en local
4. on copie export.json dans util/data.json
5. on commit/push

Pour mettre à jour les données ATTAC:
1. on met à jour le spreadsheet à la main
2. on l'export en CSV
3. on lance node ./scripts/csvToJSON/index.js fichier.csv en local
4. on lance npm extractData
5. on copie export.json dans util/data.json
6. on lance node scripts/jsonToCSV/index.js
7. on commit/push
8. on update le spreadsheet avec les données du CSV export.csv

Pour contribuer anonymement:
1. faites un checkout du projet
2. allez dans le repertoire du projet
3. lancez `git config --local user.name "anonymous"` pour changer vos noms dans tous les commits
4. lancez  `git config --local user.email "anonymous@anonymous.com"` pour changer votre emain dans tous les commits
5. lancez  `git config --local commit.gpgsign false` pour ne pas envoyer votre clef gpg si vous en avez une 
6. créez une branche comme habituellement 
7. faites vos modifications
8. créez un patch avec `git format-patch origin/main`
9. envoyez le à un contributeur public du projet via leur page de profile > contact

Immenses remerciements à :

- Attac pour les [données](https://france.attac.org/se-mobiliser/retraites-pour-le-droit-a-une-retraite-digne-et-heureuse/article/on-ne-les-lache-pas-la-carte-des-mobilisations)
- [@Teddyruptif](https://nitter.net/Teddyruptif/) pour le [logo](https://nitter.net/Teddyruptif/status/1649460414676172803)
- Toustes les camarades de Solidaires Informatique qui ont contribué ou encouragé ce projet !
