# js-fake-dinner
Projet fil conducteur sur environ 3 mois en step by step 

### Référence :
[https://dinnr.herokuapp.com/]

### Step1 : copy design du site existant 3jours

Pause de 3 semaines

#### Step2 : Fake JS Data
[https://github.com/simplonco/js-fake-dinne/data.js]
Pause de 3 semaines

### Step3 :  Server  : router pour tes pages

1. une route pour servir les elements statiques via le middleware static de express (ex. app.use(express.static('public'));
2. une route pour servir le json (ex. GET /api/dinners) qui se trouve dans ce repo
3. un route qui sert l'index.html de l'app react

   ex. 
   ``` 
   app.get('/*', (req, res) => {
     res.sendFile(path.join(__dirname, '../client/build/index.html'));
   });

   ```

### Step4 :  Server  : router pour ton API (se baser sur le contrat de données de data.js et item.js)
2 routes à faire :
  - GET all events (…/api/event)
  - GET 1 event by ID (…/api/event/ID)

### Step5 : Server : mettre en place la base de données

### Step6 : tu fais ta couche métier server (Insert / remove / list / patch (put évolué) => Possibilité d'utiliser un ORM
(ADD, REMOVE, UPDATE, DELETE)

### Step7 : Back office pour gérer les évènements 
(ADD, REMOVE, UPDATE, DELETE)
