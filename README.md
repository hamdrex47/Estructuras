Estructuras
===========
import javax.swing.JOptionPane;
import java.util.Scanner;
/**
 *
 * @author hamdrex
 */
public class Piramide {

    
    public static void main(String[] args) {
        
        Scanner s = new Scanner(System.in);
        int x;
        System.out.println("ingrese el numero de filas de la piramide : ");
        x=s.nextInt();
        int y=x;
        int w=x;
        int cont=0;
        for(int i=0; i<x; i++){
            y=w;
            for(int j=0; j<x*2;j++){
                if(j==y){
                System.out.print("*");
                    if(cont<i){
                        y+=2;
                        cont++;
                    }
                }
                else{
                    System.out.print(" ");
                }
            }
            w--;
            cont=0;
           System.out.print("\n");
        }
    }
}
