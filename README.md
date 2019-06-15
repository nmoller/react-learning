# React

Initiliser projet
```
docker run -it --rm -v ${PWD}:/opt/react \
-u 1000 -w /opt/react node:11.15.0-stretch\
 npm init
```
Installer 
```
docker run -it --rm -v ${PWD}:/opt/react \
 -u 1000 -w /opt/react node:11.15.0-stretch \
 npm install create-react-app
```

Utiliser commande
```
docker run -it --rm -v ${PWD}:/opt/react -u 1000 \
-w /opt/react node:11.15.0-stretch \
node_modules/.bin/create-react-app jsx
```

Nous allons travailler dans le dossier `jsx`:
```
docker run -it --rm -v ${PWD}:/opt/react \
--network host -u 1000 -w /opt/react \
node:11.15.0-stretch yarn start
```