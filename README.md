# actividad3
Mi Proyecto: Verificador de Paréntesis y Llaves
¡Hola! Este es un programa que hice en Java para resolver el típico problema de cuando programas y te falta cerrar un paréntesis o una llave. El código revisa una cadena de texto y te dice si todo está en orden o en qué parte metiste la pata.

🧐 ¿Cómo funciona?
Para que el programa sea ordenado, no usé las herramientas que ya trae Java, sino que armé mi propia Pila (Stack) desde cero usando Nodos.

La lógica es como una pila de platos:

Cuando el código lee un símbolo que abre ((, [, {), lo empuja a la pila.

Lo padre es que guardo no solo el símbolo, sino también en qué columna está, para que sea fácil encontrar el error.

Cuando encuentra uno que cierra (), ], }), saca el último que entró y checa si hacen "match".

Si intentas cerrar algo que nunca abriste, o si cierras con el símbolo equivocado, el programa te avisa de volada.

🛠️ Cómo correrlo
Si quieres probarlo en tu compu, solo haz esto:

Copia el código en un archivo que se llame verificador.java.

Abre la terminal en esa carpeta.

Compila con: javac verificador.java.

Corre el programa con: java verificador.

Nota: Si quieres probar otros textos, cambia la línea que dice String codigo = "([])"; en el Main.

📸 Pruebas (Evidencias)
Aquí dejo las capturas de pantalla de cuando estuve testeando el código:

✅ Todo salió bien
Aquí probé con ([]). El programa recorrió todo sin problemas porque cada cosa que se abrió, se cerró correctamente.
