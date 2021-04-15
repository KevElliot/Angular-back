# Projet Angular / Node MDBS Madagascar 2021

#Développeurs:
	- RAVOAHANGY Mahefarivo Sombiniaina N°54
	- RAKOTOMANANA Kevin Elliot N°26

#Données:

#Lien Github:
	- Backend: https://github.com/KevElliot/Angular-back
	- Frontend: https://github.com/KevElliot/Angular-front
	
#Lien Heroku:
	- Backend: https://mbdsangularback.herokuapp.com/
	- Frontend: https://mbdsangularfront.herokuapp.com/

#Fonctionnalités:
	- Gestion de login/password avec JWT et gestion de roles
	- Inscription étudiant/ prof
	- Ajout de nouvelles collections et propriétés: 
		=> Collections: Assignments, Matières, Users
		=> Propriétés: Auteur, Matière, image de la matière, photo du prof, note, remarques
	- Assignment sous forme d'une Material Card
	- Liste - pagination - infinite scroll - detail assignment
	- Formulaire de type Stepper : Modification(snackbar material) + note
    - Navigation (navbar)
	- Drag and drop Rendu et Non rendu
	- Messages de notification a la suppression d'un assignment
	- Collection d'élèves et de profs (Users)
	- Hébergement sur Heroku.com

#Utilisation en locale:
	- Backend:
		=> Télécharger le zip du projet git
		=> Extraire le fichier zip dans un dossier
		=> Executer la commande dans le dossier du projet : npm install
		=> Pour lancer, executer la commande : npm start
	- Frontend:
		=> Télécharger le zip du projet git
		=> extraire le fichier zip dans un dossier
		=> executer la commande dans le dossier du projet : npm install
		=> pour lancer, executer la commande : ng serve

#Vidéo démo:
	.
		
#Accès:
	- Etudiant:
		=> ex: 
			.Email: toto@gmail.com
			.Mot de passe: motdepasse
		=> non accès liste rendu/ non rendu, pas accès a noté assignment
		
	- Prof:
		=> ex: 
			.Email: jojo@gmail.com
			.Mot de passe: motdepasse
		=> accès à toutes les fonctionnalités

#Collections:
	- Assignments: _id - nom - prof - imageProf - matiere - imageMatiere - note - remarque - dateRendu - rendu
	- Matieres : _id - designation - image - prof - imageProf
	- Users: _id - name - email - password - role(Prof / Etudiant)

#Architecture:
[API]
	- Technologie: nodeJs 
	
	- Routes disponibles:
		=> GET /api/assignments
		=> POST /api/assignments
		=> PUT /api/assignments/:_id
		=> DELETE /api/assignments/:_id
        => GET /api/assignmentsRenduTrue/:rendu
        => GET /api/assignmentsRenduFalse/:rendu
		=> GET /api/assignments/:_id
        => POST /api/auth/register
		=> POST /api/auth/login
        => POST /api/auth/logout
		=> GET /api/assignments/student/:_id
        => GET /api/matiere
		
[ANGULAR]
	- Technologie: Angular (typescript)
	
	- Pages disponibles:
		=> login & register
		=> liste des assignments: rendu - non rendu - paginnation - delete assignment(notification)
        => liste des devoirs drag and drop - infinite scrolling
		=> assignment detail - suppression - modification - note(stepper) assignment
		=> ajout assignment
		
#Sources:
	- JWT : 
        => https://www.freecodecamp.org/news/securing-node-js-restful-apis-with-json-web-tokens-9f811a92bb52/
		=> https://dev-academy.com/angular-jwt/

    - Stepper : 
        => https://www.freakyjolly.com/angular-material-stepper-tutorial-with-examples/

    - Drag and drop : 
        => https://stackblitz.com/angular/akmmvnrgqor?file=src%2Fapp%2Fcdk-drag-drop-connected-sorting-example.html

	- Card, pagination, Stepper, notification, snackbar : 
		=> https://material.angular.io/

	- CRUD :
		=> https://github.com/micbuffa/MBDS_Madagascar2021_frontend

	- Données de test: 
		=> https://mockaroo.com/

	- Design et idées css:
		=> https://material.angular.io/
		=> https://getbootstrap.com/

    - Code copier :
        => data.service.ts (code vue groupe 08 "ANDRIAMANALINA Ranto Herizo")

		