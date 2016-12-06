# dias-de-osio-
import java.util.ArrayList;
public class Pilar  extends ArrayList {
public void encolar(Object dato){
    if(dato != null){ //si dato es diferente de nulo
  this.add(dato);//agregara el dato
    } else {// sino imprimira si es un dato diferente de nulo
  System.out.println("introduzcan un dato diferente de null");    
    }
}
//este metodo desencolara la cola 
public void desencolar(){
  if(this.size()>0){//definiremos el tamaño
      this.remove(0);// y la removemos 
  }
}
//este metodo sera el frente de la cola 
public Object frente(){
 Object datoAuxiliar=null;
 if(this.size()>0){//si el tamaño es mayor a 0
  datoAuxiliar = this.get(0);
 }
 return datoAuxiliar;//retonara el datoauxiliar
}
//metodo para vaciar la cola
public boolean vacia(){
    return this.isEmpty();
}
}





import java.util.*;

public class Corchado {

    public static void main(String[] args) {
        Scanner teclado = new Scanner(System.in);
        Pilar chavoya = new Pilar();
        int opc = 0;
        String actividad = "Jugar campesinos";
        String actividad1 = "ir al parque";
        String actividad2 = "jugar xbox";
        String actividad3 = "Dibujar mandalas";
        String actividad4 = "Dormir";
        String actividad5 = "Estudiar";
        String actividad6 = "Programar";
        String actividad7 = "Escuchar musica";
        String actividad8 = "Usar redes sociales";

        chavoya.encolar(actividad);
        chavoya.encolar(actividad1);
        chavoya.encolar(actividad2);
        chavoya.encolar(actividad3);
        chavoya.encolar(actividad4);
        chavoya.encolar(actividad5);
        chavoya.encolar(actividad6);
        chavoya.encolar(actividad7);
        chavoya.encolar(actividad8);

        System.out.println("Cuantas actividades deseas hacer e a lo largo del día?");
        opc = teclado.nextInt();
        for (int i = 0; i < 9; i++) {
            int abc = (int) (Math.random() * 9);
            if(abc ==0){
                System.out.println(actividad);
            }
            if(abc ==1){
                System.out.println(actividad1);
            }
            if(abc ==2){
                System.out.println(actividad2);
            }
            if(abc ==3){
                System.out.println(actividad3);
            }
            if(abc ==4){
                System.out.println(actividad4);
            }
            if(abc ==5){
                System.out.println(actividad5);
            }
            if(abc ==6){
                System.out.println(actividad6);
            }
            if(abc ==7){
                System.out.println(actividad7);
            }
            if(abc ==8){
                System.out.println(actividad8);}
                else{
                
                System.out.println("*** Tienes estas opciones ****");
            }
            }
          
           
            
        }
        

    }
