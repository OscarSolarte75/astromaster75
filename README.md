- 👋 Hi, I’m @astromaster75
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
astromaster75/astromaster75 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import java.util.Scanner;
class menu
{//inicio clase
    static Scanner digite = new Scanner(System.in);
       public static void main (String pito [])
       {//inicio funcion
        int opcion = 0;
        opcion = menu();
        switch (opcion)
        {//inicio casos
         case 1:
         int numero1 ,numero2;
         System.out.println("digite un numero: ");
         numero1 = digite.nextInt();
         System.out.println("digite otro numero: ");
         numero2 = digite.nextInt();
         suma(numero1 , numero2);
         despedida();
         break;
         case 2:
         System.out.println("digite un numero: ");
         numero1= digite.nextInt();
         System.out.println("digite un numero: ");
         numero2= digite.nextInt(); 
         double total_resta = resta (numero1 , numero2);
         System.out.println("el resultado de la resta es: "+ total_resta);
         despedida();
         break;

         case 3:
         System.out.println("digite un numero: ");
         numero1= digite.nextInt();
         System.out.println("digite un numero: ");
         numero2= digite.nextInt(); 
         double resultado = division (numero1 , numero2);
         System.out.println("el resultado de la suma es: "+ resultado);
         despedida();
         break;
         case 4:
         System.out.println("digite un numero: ");
         numero1= digite.nextInt();
         System.out.println("digite un numero: ");
         numero2= digite.nextInt(); 
         int rta = multiplicacion(numero1 , numero2);
         System.out.println("el resultado de la multiplicacion es: "+ rta);
         despedida();
         break;
         case 5:
         int edad;
         System.out.println("dame tu edad");
         edad= digite.nextInt();
         if (edad <= 18)
         System.out.println("dame unas papas con mani menor ");
         else
         System.out.println("ya buscate la chamba viejon ");
         despedida();
         break;
         case 6:
         int year;
         System.out.println("dame el year: ");
         year = digite.nextInt();
         if (year % 4 == 0 || year % 400 == 0)
         System.out.println("el year es bisiesto");
         else if 
         (year % 100 == 0)
         System.out.println("el year no es bisiesto");
         else
         System.out.println("el year no es bisiesto");
         despedida();
         break;
         case 7:
         despedida();
         break;
         }//fin casos
       }//fin funcion
       public static int menu()
       {//inicio menu
       int opcion=0;
       System.out.println(" MENU ");
       System.out.println("1 ... SUMA ");
       System.out.println("2 ... RESTA ");       
       System.out.println("3 ... DIVISION ");
       System.out.println("4 ... MULTIPLICACION ");
       System.out.println("5 ... MAYOR DE EDAD ");
       System.out.println("6 ... BISIESTO ");
       System.out.println("7 ... DESPEDIDA ");
       
       opcion = digite.nextInt();
       return opcion;
       }//fin menu
       public static void suma (int numero1,int numero2)
       {//inicio funcion suma
       int resultado;
       resultado = numero1 + numero2;
       System.out.println("el resultado de la suma es "+ resultado);
       }//fin funcion suma
       public static int division (int numero1,int numero2)
       {//inicio funcion division
       return numero1/numero2;
       }//fin funcion division
       public static void despedida()
       {//inicio funcion despedida
       System.out.println("chao conchetumare");
       }//fin funcion despedida
       public static int multiplicacion(int numero1 ,int numero2)
       {//inicio funcion multiplicacion
       int rta;
       return numero1 * numero2;
       }//fin funcion multiplicacion
       public static int cedula(int edad)
       {
       return edad;
       }
       public static int resta(int numero1 ,int numero2)
       { 
       int total_resta;
       total_resta = numero1 - numero2;
       System.out.println("el resultado de la resta es "+ total_resta);
       return total_resta;
       }
       public static int bisiesto(int year)
       {
       return year;
       }
//Determinar si un año es bisiesto (verificar las condiciones)
// Un año es bisiesto si es divisible por 4 
// excepto aquellos divisibles por 100 pero no por 400 
// Según el año determine la cantidad de dias de un mes.   
       
}// fin clase       

