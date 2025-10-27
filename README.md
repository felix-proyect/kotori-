### **`➮ Instalación por termux`**
<details>
<summary><b>✰ Instalación Manual</b></summary>

> *Comandos para instalar de forma manual*
```bash
termux-setup-storage
```
```bash
apt update && apt upgrade && pkg install -y git nodejs ffmpeg imagemagick yarn
```
```bash
git clone https://github.com/The-King-Destroy/YukiBot-MD && cd YukiBot-MD
```
```bash
yarn install
```
```bash
npm install
```
```bash
npm start
```
> *Si aparece **(Y/I/N/O/D/Z) [default=N] ?** use la letra **"y"** y luego **"ENTER"** para continuar con la instalación.*
</details>

<details>
  <summary><b>🜸 Comandos para mantener más tiempo activo el Bot</b></summary>

> *Ejecutar estos comandos dentro de la carpeta YukiBot-MD*
```bash
termux-wake-lock && npm i -g pm2 && pm2 start index.js && pm2 save && pm2 logs 
``` 
#### Opciones Disponibles
> *Esto eliminará todo el historial que hayas establecido con PM2:*
```bash 
pm2 delete index
``` 
> *Si tienes cerrado Termux y quiere ver de nuevo la ejecución use:*
```bash 
pm2 logs 
``` 
> *Si desea detener la ejecución de Termux use:*
```bash 
pm2 stop index
``` 
> *Si desea iniciar de nuevo la ejecución de Termux use:*
```bash 
pm2 start index
```
---- 
### En caso de detenerse
> _Si despues que ya instalastes el bot y termux te salta en blanco, se fue tu internet o reiniciaste tu celular, solo realizaras estos pasos:_
```bash
cd && cd YukiBot-MD && npm start
```
----
### Obtener nuevo código QR 
> *Detén el bot, haz click en el símbolo (ctrl) [default=z] usar la letra "z" + "ENTER" hasta que salga algo verdes similar a: `YukiBot-MD $`*
> **Escribe los siguientes comandos uno x uno :**
```bash 
cd && cd YukiBot-MD && rm -rf sessions/Principal && npm run qr
```
----
### Obtener nuevo código de teléfono 
```bash 
cd && cd YukiBot-MD && rm -rf sessions/Principal && npm run code
```
</details>

<details>
<summary><b>❀ Actualizar YukiBot-MD</b></summary>

> **Utiliza esta opción únicamente si deseas actualizar a la última versión de YukiBot. Hemos implementado un método ingenioso mediante comandos para realizar la actualización, pero ten en cuenta que al usarla se eliminarán todos los archivos de la versión actual y se reemplazarán con los de la nueva versión. Solo se conservará la base de datos, por lo que será necesario volver a vincular el Bot.**  

**Comandos para actualizar YukiBot-MD de forma automática**

```bash
grep -q 'bash\|wget' <(dpkg -l) || apt install -y bash wget && wget -O - https://raw.githubusercontent.com/DevAlexJs/SakuraBot-MD/master/termux.sh | bash 
```
**✰ Volverte owner del Bot**

*Si después de instalar el bot e iniciar la sesión (deseas poner tu número es la lista de owner pon este comando:*

```bash
cd && cd YukiBot-MD && nano settings.js
```
#### Para que no pierda su progreso en YukiBot, estos comandos realizarán un respaldo de su `database.json` y se agregará a la versión más reciente.
> *Estos comandos solo funcionan para TERMUX, REPLIT, LINUX*
</details>

---