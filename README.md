- 👋 Hi, I’m @MarcosDiaz10
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
MarcosDiaz10/MarcosDiaz10 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
--Hora futura
package quiz.fabian.sanchez;
import java.util.Scanner;

public class QUIZFABIANSANCHEZ {

    public static void main(String[] args) {
        Scanner leer = new Scanner(System.in);
        System.out.println("Ingrese la hora actual: ");
        int hora_actual=leer.nextInt();
        System.out.println("Ingrese las horas: ");
        int horas =leer.nextInt();
        
        int hora= hora_actual+horas;
        
        if (hora>24){
            int hora_nueva=(hora%24);
            System.out.println("Sera la "+ hora_nueva);
        }
        else{
            System.out.println("Sera la " +hora);
        }
    }
    
}


-- Valor de hipotenusa

package javaapplication2;
import java.util.Scanner;

public class JavaApplication2 {

    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer=new Scanner(System.in);
        double C,A,B;
        System.out.println("Ingrese el cateto A: ");
        A=leer.nextDouble();
        System.out.println("Ingrese el cateto B: ");
        B=leer.nextDouble();
        A=Math.pow(A,2);
        B=B*B;
        C=A+B;
        C=Math.sqrt(C);
        System.out.println("la hipotenusa vale "+C);
    }
    
}
 -- Calcular comision
 
 
package ciclo_for;
import java.util.Scanner;
public class Ciclo_for {

    public static void main(String[] args) {
        // TODO code application logic here
        Scanner leer=new Scanner(System.in);
        System.out.println("Ingrese el numero de vendedores: ");
        int ven=leer.nextInt();
        
        for (int i=0; i<ven; i++){
            System.out.println("Ingrese el Documento del vendedor: ");
            String doc=leer.next();
            System.out.println("Tipo de vendedor: 1= Puerta a Puerta o 2= Ejecutivo");
            int tipo=leer.nextInt();
            System.out.println("Ingrese el valor de ventas en el mes: ");
            double mes=leer.nextDouble();
            if(tipo==1){
                mes=(double)0.20* mes;
                System.out.println("Comsion ganada en el mes es de: "+mes);
            }
            else{
               mes=(double)0.30* mes;
               System.out.println("Comsion ganada en el mes es de: "+mes); 
            }
        }
    }
    
}
--trabajando con While


package ejercicio.pkgwhile;
import java.util.Scanner;
public class EjercicioWHILE {

   
    public static void main(String[] args) {
        Scanner leer =new Scanner(System.in);
        String doc="-1", nombre;
        int tipo_vende;
        double ventas_mes, comiciones ;
        
        System.out.println("Ingrese el numero de Cedula ");
        doc=leer.next();
        while(!doc.equals("999")){
            System.out.println("Ingrese el nombre ");
            nombre=leer.next();
            System.out.println("Ingrese el tipo de vendedor. 1=Puerta o 2=Ejecutivo ");
            tipo_vende=leer.nextInt();
            System.out.println("Ingrese las ventas del mes ");
            ventas_mes=leer.nextDouble();
            
            if (tipo_vende==1){
                comiciones=ventas_mes*0.20;
            }
            else{
                comiciones=ventas_mes*0.30;
            }
            System.out.println("La comicion es $"+comiciones);
            System.out.println("---------------------------");
            System.out.println("Ingrese el numero de Cedula ");
            doc=leer.next();
            
        }
        System.out.println("Fin de programa.");
        
        
    }
    
}

-- Saber cuantos son pares y cuantos son impares y cual es la suma de cada uno

package javaapplication5;
import java.util.Scanner;
public class JavaApplication5 {

    public static void main(String[] args) {
       Scanner leer=new Scanner(System.in);
       int contador_par=0,contador_impar=0,suma_par = 0,suma_impar = 0;
       
       for (int i=1; i<7; i++){
           System.out.println("Ingrese el numero "+i);
           int numero=leer.nextInt();
           if (numero%2==0){
               contador_par+=1;
               suma_par=suma_par+numero;
           }
           else{
               contador_impar+=1;
               suma_impar=suma_impar+numero;
           }
           
       }
        System.out.println("Cantidad de pares es: "+contador_par);
        System.out.println("Cantidad de pares es: "+contador_impar);

        System.out.println("la suma de los pares es: "+suma_par);
        System.out.println("la suma de los pares es: "+suma_impar);
        
        
    }
    
}

