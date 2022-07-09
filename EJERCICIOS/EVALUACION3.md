# Práctica 3.

## 3. OPERADORES

Objetivo: Verificar el dominio teórico y técnico del concepto de operador en el lenguaje
de java mediante preguntas de opción múltiple y ejercicios para desarrollar su código.
Indicaciones: Pedir responder cada una de las preguntas de manera acertada, breve y
clara, según sea el caso.

1. La expresión 5 != 6 , ¿qué valor arrojará? (Valor 1 punto)

          a. 6
          b. false
          c. true 
          d. 5
## Answer: c
              
2. ¿Qué hace el siguiente código? (Valor 1 punto)
System.out.println(8 <= 8);

          a. Imprime false.
          b. Imprime true.
          c. Imprime 8.
          d. Imprime 0.
## Answer: b

3. ¿Cómo podríamos obtener un resultado de 10, dada la siguiente variable? (Valor 1
punto)

double a = 2;

          a. a/2
          b. a*5 
          c. a - 12
          d. a % 10
## Answer: b
          
4. ¿Cuál es la mejor manera de saber si las siguientes dos cadenas son iguales?
(Valor 1 punto)

String username1 = "teracoder";

String username2 = "gigacoder";

          a. username1 == username2
          b. System.out.println(username1)
          c. username1.isEqualto(username2)
          d. username1.equals(username2)
## Answer: a    
          
5. ¿Qué operador se puede usar para concatenar dos strings? (Valor 1 punto)

          a. *
          b. .equals()
          c. +
          d. -
## Answer: c

6. ¿Hay algún error en la siguiente declaración en Java? (Valor 1 punto)

int status = 7 < 8;

          a. Sí, int debería se char.
          b. Sí, int debería ser boolean.
          c. Sí, no debería de haber un punto y como.
          d. No hay error.
 ## Answer: b

7. ¿Cuál es el resultado de la siguiente concatenación de cadenas? (Valor 1 punto)

"Son las " + 5 + "pm"

          a. "Son las pm"
          b. Error
          c. "Son las 5pm" ---
          d. 11
## Answer: c

8. Después de ejecutar el siguiente código, ¿cuál será el valor de la variable
endpoint? (Valor 1 punto)

int endpoint = 11 % 3;

          a. 1
          b. 11
          c. 2.66 
          d. 2
          e. 11
## Answer: d

9. Supón que intentamos construir algunas de las funciones de una cuenta bancaria.
Considera el siguiente código (Valor 2 puntos)

            public class CuentaBancaria {
              public static void main(String[] args){
                double saldo = 1000.75;
                double cantidadARetirar= 250;
              }
            }

a. Crea una nueva variable double llamada saldoActualizado y
almacene saldo con cantidadARetirar restada de él.

b. Ahora, imagina que has decidido dividir tu saldo en 3 partes iguales
para dárselo a tus tres mejores amigos. Crea una variable double
llamada cantidadParaCadaAmigo que contenga saldoActualizado
dividido por 3.

c. Si cada uno de tus amigos quiere comprar un boleto para un
concierto con el dinero que les diste. Y las entradas cuestan 250. Crea
una variable de tipo boolean llamado puedeComprarTicket y
configúralo de tal manera que arroje si cantidadParaCadaAmigo
tiene lo suficiente para comprar una entrada para el concierto.
Entonces, usa System.out.println() para imprimir
puedeComprarTicket.

d. Usa + y System.out.println() para imprimir:

          Le di a cada amigo <cantidadParaCadaAmigo>...
          con el valor de cantidadParaCadaAmigo en lugar de <cantidadParaCadaAmigo>.

Salida:

          true
          Le di a cada amigo 250.25...
          
## Answer:

          import java.util.Scanner;
	  
	  public class CuentaBancaria {
              public static void main(String[] args){
                double saldo = 1000.75;
                double cantidadARetirar= 250;
                
                Scanner input = new Scanner(System.in);
                System.out.println("Salida:");
		
		// Consultamos el saldo
                double saldo = 1000.75;
                double cantidadARetirar= 250;
                double saldoActualizado = saldo - cantidadARetirar;
                System.out.println(saldoActualizado);
                    
                double cantidadParaCadaAmigo = saldoActualizado / 3;
                System.out.println(cantidadParaCadaAmigo);
                boolean puedeComprarTicket = true;
                    
                    if (cantidadParaCadaAmigo >= 250) {
            		puedeComprarTicket = true;
        		} else {
            		cantidadParaCadaAmigo < 250;
        		}
        		return puedeComprarTicket;
    			}
        	    System.out.println("Le di a cada amigo" + cantidadParaCadaAmigo);
    			}
          	   // closing the scanner object
                   input.close();
		
              }
	  }
           
              
## Otro ejemplo de banco 2
 
 if (puedoSacar(cantidad))
saldo = saldo – cantidad;
 
//método ingreso
    public boolean ingreso(double n) {
        boolean ingresoCorrecto = true;
        if (n < 0) {
            ingresoCorrecto = false;
        } else {
            saldo = saldo + n;
        }
        return ingresoCorrecto;
    }

    //método reintegro
    public boolean reintegro(double n) {
        boolean reintegroCorrecto = true;                                                                         
        if (n < 0) {
            reintegroCorrecto = false;
        } else if (saldo >= n) {
            saldo -= n;
        } else {
            reintegroCorrecto = false;
        }
        return reintegroCorrecto;
    }

    //método transferencia
    public boolean transferencia(Cuenta c, double n) {
        boolean correcto = true;
        if (n < 0) {
            correcto = false;
        } else if (saldo >= n) {
            reintegro(n);
            c.ingreso(n);
        } else {
            correcto = false;
        }
        return correcto;
    }
}


 ## Otro ejemplo de banco 3
 
	 public class Banco {
	    public static void main(String[] args) {

		double totalCuenta;

		// Creamos la cuenta
		Cuenta Cuenta1;
		Cuenta1 = new Cuenta(11111, 2500.70);

		// Consultamos el saldo
		totalCuenta = Cuenta1.saldo();
		System.out.println("Total actual en la cuenta: " + totalCuenta + " €");

		// Hacemos un ingreso en la cuenta
		double ingreso = 350.25;
		System.out.println("Se ingresan en la cuenta: " + ingreso + " €");
		Cuenta1.depositar(ingreso);

		System.out.println("---");

		// Consultamos el saldo de nuevo
		totalCuenta = Cuenta1.saldo();
		System.out.println("Total actual en la cuenta: " + totalCuenta + " €");        

	    }

	}

