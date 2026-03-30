# actividad3
Mi Proyecto: Verificador de Paréntesis y Llaves

este es un programa que hice en Java para resolver el problema de cuando programas y te falta cerrar un paréntesis o una llave. El código revisa una cadena de texto y te dice si todo está en orden o en qué parte cometiste un error.

Cómo funciona? Para que el programa funcione de manera ordenada, no utilicé las herramientas que ya trae Java, sino que creé mi propia pila desde cero usando nodos.

La lógica es similar a una pila de platos: cuando el código lee un símbolo que abre, como paréntesis, corchetes o llaves, lo agrega a la pila. Lo interesante es que guardo no solo el símbolo, sino también la columna en la que se encuentra, para que sea fácil identificar el error.

Cuando encuentra un símbolo que cierra, saca el último que se agregó a la pila y verifica si coinciden. Si intentas cerrar algo que nunca abriste, o si cierras con el símbolo incorrecto, el programa te avisa de inmediato.

Cómo correr el programa

Si deseas probar el programa en tu computadora, sigue estos pasos:

* Copia el código en un archivo llamado verificador.java.

* Abre la terminal en la carpeta donde se encuentra el archivo.

* Compila el código con el comando javac verificador.java.

* Ejecuta el programa con el comando java verificador.

Nota: si deseas probar con otros textos, cambia la línea que dice String codigo = “([])"; en el Main.

Pruebas

Aquí te dejo las capturas de pantalla de cuando estuve probando el código:

* Todo salió bien: probé con ([]). El programa recorrió todo sin problemas porque cada cosa que se abrió se cerró correctamente.
