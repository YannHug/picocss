# Mise en place de PicoCss sur Symfony avec WekPack Encore

Après la création du projet symfony :

``composer require symfony/webpack-encore-bundle``

Puis 

``npm install``

Dans "asset" modifier le fichier "app.js" pour avoir du scss et modifier le fichier "app.css" en "app.scss"

Dans "app.scss" impoter picocss ``@import '~@picocss/pico/scss/pico.scss';``

Dans "webpack.config.js" décommanter ``.enableSassLoader()``

Installer un "SassLoader" ``npm install sass-loader sass --save-dev``

Puis lancer le build avec ``npm build watch``


Source : 

- YohanDev : https://www.youtube.com/watch?v=8siyYpMv_KY&t=261s

- PicoCSS : https://picocss.com/docs