sur windows

* desctiver IIS , cela permet d'utiliser le port 80
* demarrer l'image docker pour le proxy : 
    docker-compose -f .\docker-compose.yml up  reverse-proxy
* demarre l'image docker du serveur 
    docker-compose -f .\docker-compose.yml up  whoami
* tester que le serveur reponds :

curl -H Host:whoami.docker.localhost http://127.0.0.1

* generer le l'image pour le serveur nodeJS :
    se placer dans le repertoire nodejsServer 
    
