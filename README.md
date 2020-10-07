# Webbutvecklingiii_Moment5

Denna lösning och Git-repository går ut på att skapa en REST-API tjänst genom Objekt orienterad PHP som kan hantera CRUD-funktionalitet.
Detta löste jag genom att bygga på från en föregående laboration i kursen Webbutveckling II när vi gjorde en gästbok och där använde oss av MySQLi för att hantera CRUD-funktionaliteten.

Vid testningen av denna webbtjänst använde jag mig av Advanced REST Client och nedanstående kommandon för att få webbtjänsten att fungera:

Vid GET-anrop utan id i URL-raden visas alla avklarade och pågående kurser upp:
http://studenter.miun.se/~olfa1902/Webbutveckling_III/Moment_5.1/courses.php

Vid GET-anrop med id i URL-raden visas endast den kursen vars id matchar med det id du skickat med från URL-raden:
http://studenter.miun.se/~olfa1902/Webbutveckling_III/Moment_5.1/courses.php?id=x

Vid POST-anrop kommer en kurs att skapas ifall du skickar med sträng-data för coursecode,name,progression och coursesyllabus, lämpligtvis i body-formuläret
http://studenter.miun.se/~olfa1902/Webbutveckling_III/Moment_5.1/courses.php

Vid PUT-anrop kommer en kurs att ändras till den information som du har i ditt body-formulär förutsatt att informationen täcker coursecode,name,progression och coursesyllabus, 
samt att ett id finns i URL:en
http://studenter.miun.se/~olfa1902/Webbutveckling_III/Moment_5.1/courses.php?id=x

Vid DELETE-anrop kommer den kurs vars id matchar med det id du skickat med att tas bort från JSON-listan och databasen.
http://studenter.miun.se/~olfa1902/Webbutveckling_III/Moment_5.1/courses.php?id=x
