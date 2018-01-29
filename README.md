# Ruby on rails Explication
  Salut a toi nous allons voir ce qu'est Ruby on Rails dans ce README
  ![Rails](https://i.imgur.com/eo8Asuu.png?2)
## Sommaire :
 
 1. Qu'est ce que Ruby on rails
 1. La différence entre un site statique et un site dynamique
 2. Le MVC
 3. Les routes
 4. Les Bases de Données
 5. GET / POST
 6. Le concept de migration
 7. Les relations entre les models des BDD
 8. Les fonctions du CRUD

###  1. Qu'est ce que Ruby on rails (RoR)
   
   **Ruby on rails** (RoR, ou même juste Rails) est un framework Web écrit en Ruby ,
     elle permet de développer des site ou application web en suivant le principe **MVC**
     qui sera expliquer un peu pus tard.

### 1. La différence entre un site statique et un site dynamique
       
   Une page *statique* est une page dont le contenue est identique pour tous quelque soit la demande ou
   les informations fournie.
       
   Par conséquant un site dynamique est un site dont le contenu varie en fonction de la demande de l'user et
   de ses informations.
       
### 2.Le MVC
   
   Le  **MVC** (Models , View , Controller), qui est utilisé par plusieurs framework , le principe est plutôt simple. Cela va nous permettre d'avoir une interface utilisateur si je puis dire , avoir une interaction avec l'utilisateur qui nous envoi des _requêtes_ (Une demande quelconque) et pouvoir répondre a sa demande .
     * Le **Model** Qui va se charger de gérer les données
     * La **Vue** (view) Qui va se charger de l'interface graphique
     * Le **Controller** Qui va gérer les requêtes de l'utlisateur
                
                
               
Le principe de MVC est très simples a comprendre cette image résume bien la chose:









![MVC_Schema](https://i.imgur.com/cxlwPC8.png?1)

### 3.Les routes

   Les routes sont l'equivalent des actions demandable par l'user, mais interpreter d'une maniere precise
   pour orienter le controlleur.
   La configuration du route se trouve dans le fichier config/routes.rb . ex : 

```
get "users", to: "users#index"
post "users", to: "users#create"
```

  C'est comme si lorsque vous envoyer une requête (ex: vous appuyer sur un boutton), le controlleur orientais
  la requêtes pour executer une action.
  Il existe sept routes très fréquemment utilisées : index, create, show, update, destroy, new, edit.

### 4.Les bases de données (BDD)

  Pour que le **Model** puisse gérer les données il faut qu'il puisse y accéder à partir d'un certain "espace"
  qui est la **Base** **de** **donnée**.
  Les données y sont stockée et ordonées. On peux prendre comme exemple la liste des villes et des adresses E-mail
  que vous avez fait sur spreadsheets c'est en quelque sorte une base de données.
    
### 5. GET/POST

  Tout est dans les noms ou presque :
   * **GET** : Permet de recupérer des données dans la base de données
   * **POST**: Permet de crée des données dans une base de données
    
### 6.Le concept de migration 

      Le concept de Migration est là pour te permettre de structurer et d'organiser ta base de donnée.
      Mais aussi, et c'est important, d'enregistrer tes actions (historique) ou
      celles d'autres developpers sur la base de données.
      
### 7.Les relations entre les models et les BDD

   Comme dis plutôt le model recupère les données dans la bases de données qui est ordonées . 
   Mais certaines données peu etre a l'intérieur d'un base de données qui est elle même dans une base de données etc...
   Pour récupérer cela le model utilise des associations (methode) Pour traiter ces les données.
    
   Voila les commandes utiliser :
   
        belongs_to
        has_one
        has_many
        has_many :through
        has_one :through
        has_and_belongs_to_many
    
    
  Vous pouvez vous référer a la [doc Ruby](http://guides.rubyonrails.org/association_basics.html#the-types-of-associations)
    
### 8.Les fonctions du CRUD

   * **C** reate, qui permet de créer un nouvel enregistrement (POST:/{resources});
    * **R** ead, pour afficher un ou plusieurs enregistrements, (GET:/{resources} et GET:/{resources}/:id)
    * **U** pdate, pour mettre à jour un enregistrement (PUT:/{resources}/:id)
    * **D** elete, pour supprimer un enregistrement (DELETE:/{resources}/:id)


Voila pour vous Bonnes journée et bon courage a vous!!!
      
