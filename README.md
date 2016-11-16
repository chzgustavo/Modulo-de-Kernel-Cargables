# Sistemas Operativos 2016
# Modulo de Kernel Cargable
## Trabajo Práctico N° 3: Desarrollo de módulos para el kernel de Linux
				
			
			 		

***Descripción:*** El objetivo de este TP es el desarrollo de dos simples módulos para insertar en el kernel de linux. Uno de los dispositivos realizara la encriptacion simple de los caracteres que se escriben en el. El otro de los módulos realizara la desencriptacion de los caracteres que se escriben en el. Esta encriptacion y desencriptacon consta de la conversión de cada carácter a numero y luego sumar y restar un valor constante a cada carácter. En este caso la constante es uno. Con respecto a los caracteres solo se tiene en cuenta las letras de abecedario en minúscula.

***Pasos que se deben realizar para poder ejecutar los módulos y compilar el programa:***

1. Ejecute el comando: make
2. Asegúrese de cargar los módulos en el kernel para ello debe realizar lo siguiente:
	* En modo usuario : sudo insmod mkmodulo.ko (usado para encriptar)
	* En modo usuario : sudo insmod mkmodulo2.ko (usado para desencriptar)
3. Verifique de que los módulos están cargados utilizando el comando: lsmod |head
4. Para ejecutar el programa en conjunto utilice: sudo ./lkm
5. Una vez que allá corroborado el funcionamiento del programa y quiera borrar todo los archivos creados utilice: make clean
6. Si quiere borrar los modulos del kernel utilice:
	* sudo rmmod mkmodulo
	* sudo rmmod mkmodulo2
