# QESA-Quadratic-equation-solving-app
QESA will help schoolchildren quickly and easily check the correct solution of algebraic quadratic equations

Основной Java код:
package gdiclab.qesa;
import static java.lang.Math.*;

public class Qesa {

public static void main(String[] args) {
	float a, b, c;
    double D, x1, x2;
        
//вычисление дискриминанта D
    D = (b*b-4*a*c); 
  System.out.println("D = "+D);    

//если D>0 определяем корни
        if  (D>0){
        x1 = (-b - sqrt(D))/(2*a);
        x2 = (-b + sqrt(D))/(2*a);
		System.out.println("x1 = "+x1);
        System.out.println("x2 = "+x2);
        }

//если D<0 выводим сообщение в текст.поле об отсутствии действ.корней  
        else if(D<0){
        System.out.println("The equation has no actual roots");
        }
//если D=0 определяем корни х1=х2 
        else{
        x1=-b/(2*a);
        x2=x1;
		System.out.println("x1 = x2 = "+x1);
		}
	}
}
