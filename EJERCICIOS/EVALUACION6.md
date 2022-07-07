# Práctica 6.

### ARREGLOS

Objetivo: Verificar el dominio teórico y técnico del concepto de arreglos en el lenguaje de
java mediante ejercicios para desarrollar su código y preguntas de respuesta múltiple.
Indicaciones: Pedir responder cada una de las preguntas de manera acertada, breve y
clara, según sea el caso.

1. ¿Qué es un arreglo? (Valor 1 punto)

        a. Datos o valores en un arreglo
        b. Son colecciones de variables de un mismo tipo que se referencian utilizando
        un nombre común.
        c. Conjunto de variables del mismo tipo cuyo acceso se realiza por índice
 ## Answer: a
        
2. De la siguiente ilustración de un arreglo, coloca los elementos según corresponda.
(Valor 1 punto)

![image](https://user-images.githubusercontent.com/91554777/176980202-f705e695-3175-47eb-8e54-5c2cfd5ae148.png)

3. Tomando el siguiente arreglo, contesta las siguientes preguntas: (Valor 2 puntos)

![image](https://user-images.githubusercontent.com/91554777/176980222-c9ac9e57-a50d-4329-9db6-b2b1c02aeae4.png)

      a. ¿Qué tipo de dato tiene el arreglo?
      b. ¿Qué valor se encuentra en la posición con el índice 4?
      c. ¿Cuál es el rango de índices del arreglo?
## Answers a: double, b: 8.3, c: 10 (length=longitud)

      
 4. ¿Qué tipo de ciclo se adapta fácilmente para el manejo de un arreglo? (Valor 1
punto)

      a. Do - While
      b. For
      c. While
## Answer: 
      
 5. ¿Cómo se le conoce a los arreglos unidimensionales? (Valor 1 punto)
 
        a. Matriz
        b. Contador
        c. Vector    
## Answer: c
   
6. Un arreglo bidimensional es aquel que consta de: (Valor 1 punto)

        a. Una columna
        b. n columnas
        c. m filas y n columnas
## Answer: c
        
7. Sea un arreglo vector[] conformado por 10 elementos, ¿Qué muestra si se escribe
en el código vector[10]? (Valor 1 punto)

      a. Nada.
      b. Todo el contenido.
      c. Lo que tengo en la posición 10 de mi arreglo.
## Answer: c    
      
8. Si se ejecuta el siguiente código, ¿Qué imprime la línea 5 y la línea 7? (Valor 2
puntos)

![image](https://user-images.githubusercontent.com/91554777/176980300-634ec85b-39d3-4b54-8101-962128d7252f.png)

      a. Lista de productos
      Paleta 2.50
      Papas 14.00
      Galletas de chocolate 15.50
      Refresco 34.70

      b. Lista de productos
      Paleta 2.50
      Lista de productos
      Papas 14.00
      Lista de productos
      Galletas de chocolate 15.50
      Lista de productos
      Refresco 34.70

      c. Lista de productos
      Paleta
      Papas
      Galletas de chocolate
      Refresco
      2.50
      14.00
      15.50
      34.70

      d. Paleta 2.50
      Papas 14.00
      Galletas de chocolate 15.50
      Refresco 34.70
      Lista de productos
      
## Answer: a

        public class Main {

                   public static void main(String[] args) {

                       String productos [] = {"Paleta", "Papas", "Galletas de chocolate", "Refresco"};
                       double precios [] = {2.50, 14.00, 15.50, 34.70};
                       System.out.println("Lista de Productos");  
                       for(int i=0; i < productos.length; i++){
                           System.out.println(productos[i] + " " + precios[i]);
                        }
                    }
        }
    
 9. Crea un programa en java considerando las siguientes instrucciones: (Valor 2
puntos)

      a. Crea un arreglo llamado números el cual tenga los siguientes elementos 12,
      10, 4, 24, 5 y 9.
      b. Realiza un ciclo que recorra todo el arreglo y en cada pasada, imprima El
      arreglo en la posición “número de posición” tiene el número “imprimir el
      número que se encuentre en esa posición”.
      i. Ejemplo. El arreglo en la posición 2 tiene el número 4.
      
## Answer:

public class Main {
        public static void main(String[] args) {

            // crear un arreglo
            int[] numeros = {12, 10, 4, 24, 5, 9};

            //  realizar un ciclo que recorra todo el arreglo 
            //  usar el bucle for 

            for(int i = 0; i < numeros.length; i++) {
                System.out.println(numeros[i]);
                }   
                System.out.println("El arreglo en la posicion 1 tiene el numero: " + numeros[0]);
                System.out.println("El arreglo en la posicion 2 tiene el numero: " + numeros[1]);
                System.out.println("El arreglo en la posicion 3 tiene el numero: " + numeros[2]);
                System.out.println("El arreglo en la posicion 4 tiene el numero: " + numeros[3]);
                System.out.println("El arreglo en la posicion 5 tiene el numero: " + numeros[4]);
                System.out.println("El arreglo en la posicion 6 tiene el numero: " + numeros[5]);
        }
    }

    
## Otro ejemplo:

public class Main {
    public static void main(String[] args) {

        // crear un arreglo
        int[] numeros = {12, 10, 4, 24, 5, 9};

        //  realizar un ciclo que recorra todo el arreglo 
        //  usar el bucle for 
        System.out.println("Usando el bucle for:");
        for(int i = 0; i < numeros.length; i++) {
            System.out.println(numeros[i]);
            }
     }
}

