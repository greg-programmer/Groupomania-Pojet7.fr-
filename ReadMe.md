***************************LES ETAPES POUR DEMARER LE PROJET***********************************************

-----Etape 1 la préparation des dossiers---------- 

Récupérer le dossier frontend via github :
Créer un dossier nommé Groupomania
Ensuite, dans le dossier Groupamania, il faut copier le dossier frontend via github avec le terminal node 
"git clone ??? frontend"
Ensuite il faut aller sur le dossier frontend
"npm install"
Enfin, il faut copier le dossier backend dans le dossier Groupomania.


-----Etape 2 Faire fonctionner le backend---------- 

npm install express
 //Ce package installe express, de ce fait, il facilite grandement la création du server// 
npm install -g nodemon
 //Ce package permet de visualiser en temps réél le changement côtés server.
npm install mongoose
 //Ce package permet de gérer la base de donné mongoDb
npm install mongoose-unique-validator
//Ce package permet de rendre l'adresse email unique
npm install bcrypt
 //Ce package permet de crypter le mot de passe de chaque utilisateur
npm install jsonwebtoken
//Ce package permet de créer un jeton d'authentification pour l'utilisateur qui se connecte
npm install multer
//Ce package permet de capturer les fichiers envoyés avec une requête http//
ensuite lancer 'nodemon server' via le dossier backend et vous pourrez vous connecter au server backend

**--------------ROUTE API backend (utilisateur)---------------**
------
"POST"
- http://localhost:4080/api/auth/signup/ ==> Inscription de l'utilisateur 
- http://localhost:4080/api/auth/login/ ==> Connexion de l'utilisateur
- http://localhost:4080/api/auth/user/upload/:id ==> Modifier l'image de l'utlisateur
------
"GET"
- http://localhost:4080/api/auth/login/token/ ==> Récupération du token pour identifier l'utilisateur
- http://localhost:4080/api/auth/logout/ ==> Déconnexion de l'utilisateur et suppression du cookies (token) 
- http://localhost:4080/api/auth/login/getusers ==> Récupération du nom, prénom ,service et la photo de l'utilisateur. 

-----Etape 3 Faire fonctionner le frontend---------- 

**--Faire fonctionner le server Frontend**:
Il faut lancer 'npm run start' via le dossier frontend.
Maintenant vous pouvez vous connecter sur http://localhost:4080/profil
