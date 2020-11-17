https://medium.com/@onexlab.io/docker-compose-mariadb-multiple-database-c24f75f4c3c8


C'è l'intento di deployare attraverso un file yaml un database mariadb, creando diversi users e databases, di modo da poter associarvi dei secrets e configmaps usate da utenti diversi. Nel mio caso, mi piacerebbe ci sia Dev1, che ha accesso a db1, Dev2 che ha accesso a db2(o db1?) e un utente root che può far di tutto.
Creerò 3 diverse istanze di db: 
-PROD
-DEV
-TEST
inizialmente userò docker compose

https://www.mariadbtutorial.com/getting-started/connect-to-mariadb/ : comandi fondamentali per poter usare mariadb!

docker exec -it nome_container /bin/bash per accedere dentro un container(rulof)
