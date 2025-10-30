> *Comandos para instalar de forma manual*

termux-setup-storage


apt update && apt upgrade && pkg install -y git nodejs ffmpeg imagemagick yarn

git clone https://github.com/felix-proyect/kotori-  && cd kotori-

yarn install


npm install


npm start

> *Si aparece **(Y/I/N/O/D/Z) [default=N] ?** use la letra **"y"** y luego **"ENTER"** para continuar con la instalación.*


🜸 Comandos para mantener más tiempo activo el Bot

> *Ejecutar estos comandos dentro de la carpeta Session*

termux-wake-lock && npm i -g pm2 && pm2 start index.js && pm2 save && pm2 logs 

#### Opciones Disponibles
> *Esto eliminará todo el historial que hayas establecido con PM2:*

pm2 delete index

> *Si tienes cerrado Termux y quiere ver de nuevo la ejecución use:*

pm2 logs 

> *Si desea detener la ejecución de Termux use:*

pm2 stop index

> *Si desea iniciar de nuevo la ejecución de Termux use:*

pm2 start index

### En caso de detenerse
> _Si despues que ya instalastes el bot y termux te salta en blanco, se fue tu internet o reiniciaste tu celular, solo realizaras estos pasos:_


cd && cd kotori- && npm start

----
### Obtener nuevo código QR

> *Detén el bot, haz click en el símbolo (ctrl) [default=z] usar la letra "z" + "ENTER" hasta que salga algo verdes similar a: `Kotori $`*
> **Escribe los siguientes comandos uno x uno :**

cd && cd kotori- && rm -rf sessions/Principal && npm run qr

----
### Obtener nuevo código de teléfono 

cd && cd kotori- && rm -rf sessions/Principal && npm run code