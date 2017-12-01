# Remix
Remix (també conegut com Browser-Solidity) és un compilador Solidity basat en navegador i IDE.
Visiteu https://remix.ethereum.org per utilitzar; sempre lliurarà la versió més recent.

# Ús fora de línia
La branca de les pàgines de gh sempre té l'última versió estable del remix. També conté un fitxer ZIP amb tota la compilació. Baixeu-lo per utilitzar fora de línia.
Nota: conté l'última versió de Solidity disponible al moment de l'embalatge. No s'admeten versions de cap altre compilador.  

# **Instalación**
Instale npm y node.js (consulte https://docs.npmjs.com/getting-started/installing-node), luego haga:
+ git clone https://github.com/ethereum/browser-solidity
+ cd navegador-solidez


# DESENVOLUPAMENT:
Executeu npm i obriu http://127.0.0.1:8080 al vostre navegador.
A continuació, obriu l'editor de text i comenci a desenvolupar. El navegador s'actualitzarà automàticament quan es guardin els fitxers
## Resolució de problemes de construcció
Aquí teniu algunes coses a tenir en compte si teniu problemes per crear el paquet.
• Assegureu-vos que teniu la versió correcta del node, npm i nvm. Podeu trobar la versió que es prova en Travis CI buscant.
node --version
npm --versió

# Prova Unitària
Registreu fitxers de prova d'unitats nous a prova / index.js. Les proves s'escriuen amb cinta adhesiva.
Executeu les proves de la unitat a través de: prova de npm
Per a les proves locals sense navegador sense cap executar, executeu el navegador de prova (requereix que s'instal·li el seleni), es pot fer amb npm executar selenium-install)
La realització de proves unitàries a través de la prova npm requereix, com a mínim, el node v7.0.0

# **Pruebas del navegador**
Para ejecutar las pruebas de Selenium a través de Nightwatch, sirve la aplicación a través de un servidor web local:
npm run serve # inicia el servidor web en localhost: 8080
Entonces necesitarás:
1. Tener un servidor Selenium ejecutándose localmente en el puerto 4444.
  + Ejecutar: npm ejecutar test-browser
2. O bien, instale y ejecute SauceConnect.
  + Ejecutar: sc -u <NOMBRE DE USUARIO> -k <ACCESS_KEY> (ver .travis.yml para conocer los valores)
