
les titres et dates de sortie des films du plus récent au plus ancien V

 ``` SQL
SELECT `Nom_Films`, `Date_Films` FROM `Films`
ORDER BY `Nom_Films`, `Date_Films` ASC
 ```


les noms, prénoms et âges des acteurs ou actrices de plus de 30 ans dans l'ordre alphabétique  V

 ``` SQL
SELECT `Nom_Acteur`, `Prenom_Acteur`, `Age_Acteur` FROM `Acteur` ORDER BY `Nom_Acteur`, `Prenom_Acteur`, `Age_Acteur` DESC
 ```


la liste des actrices ou acteurs principaux pour un film donné V

 ``` SQL
SELECT `Principaux_Acteurs` FROM `Acteur`
 ```
 

 la liste des films pour une actrice ou un acteur donné V

 ``` SQL
SELECT `Films_Acteur` FROM `Acteur`; 
 ```

ajouter un film V

``` SQL
INSERT INTO `Films` (`ID_Films`, `Nom_Films`, `Acteurs_Films`, `Realisateur_Films`, `Date_Films`) VALUES (NULL, '...', '...', '...');
 ```


ajouter une actrice ou un acteur V

 ``` SQL
INSERT INTO `Acteur` (`ID_Acteur`, `Prenom_Acteur`, `Nom_Acteur`, `Films_Acteur`, `Age_Acteur`) VALUES (NULL, '...', '...', '...');
 ```


modifier un film V

 ``` SQL
UPDATE `Films`
SET `Nom_Films` = '...'
 ```


 supprimer une actrice ou un acteur V

 ``` SQL
DROP TABLE `Acteur`
 ```
 

 afficher les 3 derniers acteurs/actrices ajouté(e)s V

 ``` SQL
SELECT `ID_Acteur` FROM `Acteur` ORDER BY `ID_Acteur` DESC LIMIT 3
 ```
