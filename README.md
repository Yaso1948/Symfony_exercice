# Symfony_exercice
a test example for using the Symfony project, including matters such as CRUD,DQL,QueryBuiler,etc.(subject to change for whenever i have time to clarify more, this is all the superficial information you'll need to execute a foreign symfony project) .

the content of the test consists of the following:
  _Two entities: joueur/partie, join one to many from player to part, RCD for joueur,RCU to partie in addition a feature with the utility corresponding to the display of parties whose dates are between two statitically given dates._

In order to run the project, you need the following requirements(exluding most instalments such as scoop,symfony CLI,etc, could be added at a later date):
* XAMPP(at least apache and MySQL services available to run).

* manipulate the .env file, particularlythe DATABASE_URL variable in order to configure doctrine ORM to know which database it deals with.

**make sure MySQL service is running from here.**
* type into the command prompt(in the project directory) php bin/console d:d:c(this creates the database in your DBMS(SGBD in french) of choice depending on your configuration of the .env file.

* again, in the command prompt, php bin/console doctrine:migrations:migrate in order to define for your DBMS the structure of the database considering the tables,columns and relations(in case you made a migration before migrating,doctrine:migrations:version to choose which migration to execute, doctrine:migrations:latest executes the latest migration). 

**Once that's over, finally in the command prompt, Symfony serve, it should give you the URL in a green highlighted part.**
