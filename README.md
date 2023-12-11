# EJEMPLO DE MICRO FRONTS

El siguiente ejemplo muestra un enrutador de single-spa, así como el menú creado con react y dos proyectos en angular.
Cada uno de estos ambientes creados desde single-spa.

## Requisitos previos

- Angular (versión 15.2.10)
- React (versión 17.0.19)
- Node (a partir de la versión 18.18.0)

## Iniciar
1. Navega al orquestador del proyecto: 'cd root'
2. Iniciar el parcel root de primera instancia: 'npm start'
3. En diferentes terminales, navegar a cada carpeta de los parcel e inicializarlos
    -cd header
        - npm start
    - cd body
        - cd angular1
        - angular1/ npm start
    - cd content
        - cd angular2
        - angular2/ npm start


## NOTA: 
Para montar dos o más parcel de Angular, se debe utilizar diferentes puertos y esta configuración se puede realizar de las siguientes maneras:

## Desde package.json
1. En el script de start, poner el puerto que se quiere utilizar, en el ejemplo se puso el siguiente:
 "ng serve --port 4202"
2. Se guardan los cambios y se inicia el parcel

## Desde terminal
1. En la terminal del segundo parcel y antes de iniciar el parcel, se ingresa el siguiente comando con el puerto a elección como en el siguiente ejemplo:
    ng s --port 4202

2. Si marca error al ejecutar el comando, se debe ejecutar la siguiente instrucción:
    Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

3. Se vuelve a ingresar el comando del punto 1 y deberá iniciarse sin problema

