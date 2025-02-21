# docker-build

> Construis une image à partir d'un Dockerfile.
> Plus d'informations : <https://docs.docker.com/engine/reference/commandline/build/>.

- Construis une image Docker en utilisant le Dockerfile du répertoire courant :

`docker build .`

- Construis une image Docker à partir d'un Dockerfile situé à une URL précisée :

`docker build {{github.com/creack/docker-firefox}}`

- Construis une image Docker et l'étiquette :

`docker build --tag {{nom:etiquette}} .`

- N'utilise pas le cache lors de la construction de l'image :

`docker build --no-cache --tag {{nom:etiquette}} .`

- Construis une image Docker utilisant un Dockerfile spécifique :

`docker build --file {{Dockerfile}} .`

- Construis avec des variables personnalisées définies à la volée :

`docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .`
