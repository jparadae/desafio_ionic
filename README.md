# desafio_ionic

Proyecto para alumnos de la clase de programación de app mobiles con ionic y vue

## Objetivos.

1. Generar una notificacion push, puede elegir firebase o aws amplify.
2. Generar una actualización cuando el telefono no tenga la conectividad.

## Criterios a evaluar:

```
- Cumplir con al menos uno de los twelve factors 
- Debe ser compilado en un dispositivo físico y validar lo siguiente:
a) Envio notificación desde emisor firebase/amplify hacia dispositivo con conectividad a internet
b) Envio notificación desde emisor firebase/amplify hacia dispositivo sin conectividad a internet
c) Generar la sincronización de notificaciones
d) Leer notificaciones, (debe generar logs)
```


# Instalar dependencias FCM(Firebase Cloud Messaging)

Documentación oficial https://ionicframework.com/docs/native/fcm

```
npm install cordova-plugin-fcm-with-dependecy-updated

npm install @ionic-native/fcm

npm install @ionic/app-scripts@latest --save-dev

ionic cap sync

npm i @capacitor-community/fcm
```

# Recomendaciones para actualizar node

```
sudo npm cache clean -f
sudo npm install -g n
sudo n stable
```

Iniciar proyecto


```
ionic serve
```


# Compilar en Android

```
ionic build
ionic cap add android
ionic cap copy
ionic cap sync
ionic cap open android
```


