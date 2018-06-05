/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package imc;

/**
 *Atividade de IMC - Ciclo 03 Unis
 * @author Bruno Gabriel Corrêa
 */
import javax.swing.*;

public class Imc

{

public static void main(String args[])

{

    float peso, altura, imc;

        String entrada = new String();

 

        entrada = JOptionPane.showInputDialog("Digite o peso");

            peso = Float.parseFloat(entrada);

 

        entrada = JOptionPane.showInputDialog("Digita a altura");

            altura = Float.parseFloat(entrada);

                    imc = (peso)/(altura*altura);

 
        //Magressa Grave            
        if (imc <=16){

            JOptionPane.showMessageDialog(null, "Magressa Grave " +imc);

        }
        if (imc >16 && imc <=17){
            
            JOptionPane.showMessageDialog(null, "Magreza moderada" +imc);
        }

        //Saúdavel     
        if (imc >=18.5 && imc <=25){

            JOptionPane.showMessageDialog(null, "Saúdavel " +imc);

        }
        
        //Sobrepeso
        if (imc >=26 && imc <=30){

            JOptionPane.showMessageDialog(null, "Sobrepeso " +imc);

        }
        
        //Obesidade Grau I
        if (imc >=31 && imc <=35) {

            JOptionPane.showMessageDialog(null, "Obesidade Grau I " +imc);

        }
        //Obesidade Grau II (severa)
            if (imc >=36 && imc <=40) {

            JOptionPane.showMessageDialog(null, "Obesidade Grau II severa" +imc);

        }
        //Obesidade Grau III(mórbida)
            if (imc >=41) {

            JOptionPane.showMessageDialog(null, "Obesidade Grau III mórbida " +imc);

        }

}

}
