#Práctica 5.

###INSTRUCCIONES

Objetivo: Verificar el dominio teórico y técnico del concepto de la sentencia switch
en el lenguaje de java mediante, preguntas abiertas, de opción múltiple y ejercicios para
desarrollar su código.

Indicaciones: Pedir responder y/o desarrollar cada una de las preguntas de manera
breve y clara.

1. ¿Cuál es la sintaxis de la estructura switch - case en Java? (Valor 2)

## Answer:

      //La sentencia switch nos permite ejecutar un bloque de codigo entre muchas alternativas.
      // La sintaxis de la estructura switch es la siguiente:

            switch (expresion) {
            case valor1:
               // codigo
              break;
       // La expresion se evalua una vez y se compara con los valores de cada caso.
       // Si la expresion coincide con el valor1, el codigo de case valor1 se executa.
            case valor2:
               // codigo
              break;
       // Del mismo modo el codigo de case valor2 se executa si la expresion coincide con valor2.
       // Si no hay coincidencia, se ejecuta el codigo del caso predeterminado.
            ...
            ...
            default:
                // declaraciones predeterminadas
            }

2. ¿Cual de las siguientes oraciones es correcta acerca del default dentro de la
estructura switch - case? (Valor 1)

      a. Se ejecuta si el resultado de la expresión no coincide con ningún caso.
      b. El default es opcional.
      c. Todas las anteriores.
      
## Answer: a 
      
3. ¿Cuál es una afirmación incorrecta de la estructura switch – case? (Valor 1)

        a. La instrucción switch no nos permite reemplazar varias construcciones
        if-else.
        b. Los tipos de datos que puede evaluar un switch - case son short, int, byte o
        char.
        c. El valor para un case debe ser del mismo tipo de datos que la variable en el
        switch.
 
 ## Answer: a
        
4. ¿Qué líneas del siguiente código tienen algún error? (Valor 2)

![image](https://user-images.githubusercontent.com/91554777/176980099-2bf4ede3-0c22-49af-9bc5-0d2f09f81976.png)

      a) Líneas 1, 3, 5, 10
      b) Línea 1, 5, 10, 15
      c) Línea 1, 9 10, 14
      
## Answer: c
      
 5. En la estructura switch - case, ¿cuál instrucción se usa para terminar la secuencia
de un caso? (Valor 1)

      a. default
      b. case
      c. break
      d. switch
      
## Answer: c
      
6. Crea el código en java bajo las siguientes instrucciones: (Valor 3)

        a. Importa la clase Scanner para la lectura de datos.
        b. Crea un objeto semana de la clase Scanner.
        c. Crea una variable dia de tipo entero.
        d. Imprime el texto Introduce un número del 1 al 7 para conocer el día de la
        semana, para hacer la lectura de el dato desde teclado y almacenarlo en la
        variable dia.
        e. Crea una estructura switch-case, donde la variable a comparar con todos los
        casos es dia.
        f. En cada caso, coloca e imprime cada día de la semana (comenzando el Lunes).
        g. Si se ingresa un número de día no válido, imprime el mensaje Número no
        válido.
        
## Answer:

//a. Importa la clase Scanner para la lectura de datos.
import java.util.Scanner;

public class diadelaSemana {
  public static void main(String[] args) {
  
//c. Crea una variable dia de tipo entero.
    int dia;
    
    // b. Crea un objeto semana de la clase Scanner.
    Scanner ingresa = new Scanner(System.in);

    // ask users to enter operator
    System.out.println("Dame un numero");
    operator = input.next().charAt(0);

    // ask users to enter numbers
    System.out.println("El numero 1 corresponde al dia lunes");
    number1 = input.nextDouble();

    System.out.println("El numero 2 corresponde al dia martes");
    number2 = input.nextDouble();
    
    System.out.println("El numero 3 corresponde al dia miercoles");
    number2 = input.nextDouble();
    
    System.out.println("El numero 4 corresponde al dia jueves");
    number2 = input.nextDouble();

    switch (operator) {

      // performs addition between numbers
      case '+':
        result = number1 + number2;
        System.out.println(number1 + " + " + number2 + " = " + result);
        break;

      // performs subtraction between numbers
      case '-':
        result = number1 - number2;
        System.out.println(number1 + " - " + number2 + " = " + result);
        break;

      // performs multiplication between numbers
      case '*':
        result = number1 * number2;
        System.out.println(number1 + " * " + number2 + " = " + result);
        break;

      // performs division between numbers
      case '/':
        result = number1 / number2;
        System.out.println(number1 + " / " + number2 + " = " + result);
        break;

      default:
        System.out.println("Invalid operator!");
        break;
    }

    input.close();
  }
}

