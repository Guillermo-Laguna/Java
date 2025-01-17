# Práctica 1.

## 1. INTRODUCCIÓN AL LENGUAJE DE PROGRAMACIÓN

Objetivo: Verificar el dominio teórico y técnico de los principios básicos de java mediante
preguntas de opción múltiple y ejercicios para desarrollar su código.
Indicaciones: Pedir responder cada una de las preguntas de manera correcta, breve y
clara, según sea el caso.

1. Java es un lenguaje compilable, lo que significa que el código que escribimos es
traducido a un lenguaje que la computadora entiende. (Valor 1 punto)

        a. Falso
        b. Cierto
## Answer: b

2. En Java, ¿cuál es el propósito de escribir comentarios en el código? (Valor 1 punto)

        a. Proporcionan notas legibles para humanos que aclaran el pensamiento.
        b. Proporcionan controles que el compilador debe pasar.
        c. Indican cómo se imprimen las palabras en la pantalla.
        d. Sólo están presentes en el código de compilación.
 ## Answer: a

3. El siguiente código se ejecutará sin error. (Valor 1 punto)

        public class LanguagesFacts{

            public static void main(String[] args){

              System.out.println("Las clases Java tienen un método 'main()'.")

              System.out.println("Las declaraciones de Java terminan con un punto y coma.");

             }

        }

        a. Cierto
        b. Falso
## Answer: b 

/* It is necessary to give indentation to the code and in the third line to remove accent and also add semicolon*/

        public class LanguagesFacts{
            public static void main(String[] args) {
                System.out.println("Las clases Java tienen un metodo 'main()'.");
                System.out.println("Las declaraciones de Java terminan con un punto y coma.");
            }
        }

4. ¿Qué imprimirá el siguiente código en la pantalla? (Valor 1 punto)

        public class HelloYou{

             public static void main(String[] args){

               System.out.println("¡Hola amigo!");

             }

        }

        a. ¡Hola amigo!
        b. Este código contiene un error.
        c. "¡Hola amigo!"
## Answer: b (US-ASCII)

        /* You need to remove the first exclamation mark*/

                public class HelloYou {
                    public static void main(String[] args) {   
                        System.out.println("Hola amigo!"); 
                    }
                }

5. ¿Qué le falta a este programa en Java? (Valor 1 punto)

public class HechosLenguaje{

  // Cubre la historia del lenguaje de programación Java.
  
}

          a. Las llaves que marcan el alcance de la clase.
          b. La línea para compilar código: javac HechosLenguaje.java
          c. Un comentario de una sola línea.
          d. El método main().
 ## Answer: d


6. ¿Cuál sería el nombre del archivo si contuviera el siguiente código? (Valor 1 punto)

        public class HolaMundo{

            public static void main(String[] args){

               System.out.println("¡Hola Mundo!");

            }

        }

          a. HolaMundo.java
          b. No hay restricciones en el nombre del archivo en Java.
          c. HolaMundo.class
## Answer: a 

// As in the previous case, you need to remove the first exclamation mark to run the code

7. Completa la clase HolaTu del programa HolaTu.java, para que imprima “¡Hola
Mi_Nombre!” donde “Mi_Nombre” sea tú nombre. (Valor 2 punto)

        public class HolaTu {
          public static void main(String[] args) {
          }
        }

Salida:
¡Hola  ́nombre_del_programador ́!!

## Answer:

        public class HolaTu {
            public static void main(String[] args) {
                 System.out.println("Hola Mi_Nombre!"); 
            }
        }

## Explicación del código Hola Mundo
public static void main(String[] args)
//En detalle:
public: Para que la JVM (Máquina Virtual Java) pueda ejecutar el método desde cualquier lugar.
static: El método principal puede ser llamado sin crear el objeto. (lo veremos más adelante)
//Los modificadores public y static se pueden escribir en cualquier orden.
void: El método main no devuelve nada.
main(): Nombre configurado en la JVM
String[]: El método principal acepta un único argumento:
          una matriz de elementos de tipo String.

8. Dada la clase con método main() LasEscondidas, que pertenece a un programa
que se llama LasEscondidas.java. (Valor 2 puntos)

        public class LasEscondidas {

           public static void main(String[] args) {

               System.out.println("Juguemos a las escondidas.");

            }

        }

          a. Debajo de la declaración de impresión System.out.println("Juguemos a las
          escondidas");, usando System.out.print(), genera las siguientes dos declaraciones:

          "Tres..."
          "Dos..."

          b. Ahora, usando System.out.println(), genera los siguientes dos declaraciones:

          "Uno..."
          "¡Listos o no, aquí voy!"

## Answer:

        public class LasEscondidas {

           public static void main(String[] args) {

              System.out.println("Juguemos a las escondidas.");
              System.out.println("Tres...");
              System.out.println("Dos...");  
              System.out.println("Uno...");
              System.out.println("Listos o no, aqui voy!");
            }
        }

9. Supón que el siguiente código pertenece al programa Timeline.java el cual tiene
texto sin formato. (Valor 2 puntos)

            public class Timeline {
                public static void main(String[] args) {
                   System.out.println("¡Hola Java!");
                   System.out.println("Naciste en 1995.");
                   Sun Microsystems anunció el lanzamiento de Java en 1995
                System.out.println("Fuiste creado por James Gosling.");
                   James Gosling es un ingeniero canadiense que
                   creó Java mientras trabajaba en Sun Microsystems.
                   ¡Su número favorito es la raíz cuadrada de 2!
                System.out.println("¡Eres un lenguaje divertido!");
               }
            }

Usa comentarios para evitar detener la ejecución del programa por el texto sin formato.

a. Usa la sintaxis de comentarios de una sola línea para la primera parte del texto.
Cambia esta línea a comentario:

Sun Microsystems anunció el lanzamiento de Java en 1995

b. Usa la sintaxis de varias líneas para convertir estas líneas en un solo comentario:
James Gosling es un ingeniero canadiense que
creó Java mientras trabajaba en Sun Microsystems.

¡Su número favorito es la raíz cuadrada de 2!
de tal manera que puedas ver impreso el mensaje: ¡Eres un lenguaje divertido!

c. Escribe la salida del programa.

## Answer:

        public class Timeline {
            public static void main(String[] args) {

               System.out.println("Hola Java!");
        //Sun Microsystems anuncio el lanzamiento de Java en 1995               
               System.out.println("Naciste en 1995.");
               System.out.println("Fuiste creado por James Gosling.");
        /*James Gosling es un ingeniero canadiense que creo Java mientras trabajaba en Sun           Microsystems. Su numero favorito es la raiz cuadrada de 2!*/
                System.out.println("Eres un lenguaje divertido!");
              }
         }

10. Escribe el contenido de un programa en java que lleva por nombre
Evaluacion.java con las siguientes características: (Varlor 2 puntos)

a. Define una clase pública (public class) denominada Evaluacion. Usa llaves
de apertura y cierre para determinar el alcance de la clase (class).

b. Define el método main() dentro de las llaves de la clase (class) Evaluacion.

c. Dentro de las llaves para el método main(), escribe

El método main ejecuta las tareas de la clase

como un comentario de una sola línea.

d. Debajo del comentario, escribe una declaración que imprima lo siguiente:


¡Mi primer programa Java desde cero!

e. Escribe la salida del programa.

## Answer: 

        public class Evaluacion {
            public static void main(String[] args) {
              //El metodo main ejecuta las tareas de la clase  
              System.out.println("Mi primer programa Java desde cero!");
            }
        }
