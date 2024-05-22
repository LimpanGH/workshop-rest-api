
# Backendutveckling och API:er workshop: Skapa REST API

👋 Ta inspiration/struktur från lektion 22 maj och d[etta repo](https://github.com/chasacademy-sandra-larsson/nodejs-mysql-rest-socialmedia) ✅ 

### Din uppgift:

Du ska skapa ett REST API för 2 till 3 olika resurser. Detta ska göras med Node.js, Express och MySQL.

1. Börja identifiera de resurser du ska ha för [inlämningsuppgiften i kursen](https://chasacademy.instructure.com/courses/289/assignments/1706?module_item_id=8427)

2. Definiera dina tabeller för varje resurs i phpMyaAdmin eller SQL-syntax. Ange datatypen för varje fält, tabellens primärnyckel (primary key) och eventuell/a främmande nycklar (foreign keys)

3. Använd dig av mysql2 för uppkoppling och förfrågning mot mysql-databasen (samma som i förra workshopen). Denna gång ska du lägga din databasuppgifter i en .env fil.

2. Använd dig av en mappstruktur eller liknande enligt bild nedan, så att du får en bra struktur och modulär kod som är enkel att skala upp

3. Du behöver installera ```npm install express mysql2 bcrypt body-parser cors dotenv``` ```npm i nodemon --save-dev```

4. Definera dina endpoints (routes) för varje resurs

5. Skriva dina handler enligt CRUD för varje route

6. Testa ditt REST API med ThunderClient eller Postman. Skapa en "collection" för tester av varje resurs så att du enkelt kan testa dina routes


Förslag på mappstruktur:

```
nodejs-mysql-rest-socialmedia
├── .env
├── .gitignore
├── README.md
├── app.js
├── package-lock.json
├── package.json
└── src
    ├── db
    │   └── connect.js
    ├── middleware
    └── resources
        ├── posts
        │   ├── posts.controllers.js
        │   └── posts.routes.js
        └── users
            ├── users.controllers.js
            └── users.routes.js

```

### *Tanken är att du bygger vidare på denna kod nästa vecka och till inlämningsuppgiften!*


# 👩🏽‍💻 Övrigt

Ta hjälp av dokumentation på [https://expressjs.com/](https://expressjs.com/)

Se även över HTTP-statuskoder! [https://developer.mozilla.org/en-US/docs/Web/HTTP/Status](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)


# 💬 Diskutera/Bra att kunna

* Vad är ett REST API?
* Vad är CRUD?
* Ha koll på klient-server modellen, request/response-cykeln
* Ha koll på HTTP-statuskoder


