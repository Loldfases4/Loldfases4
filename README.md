# Antonio Alcaraz Guirao – Desarrollador Web (DAW)

## Sobre mí
Estudiante de Desarrollo de Aplicaciones Web con interes en ser desarrollador de videojuegos. Quiero aprender todo lo posible para saber optimizar y hacerlo todo bien para tener exito.


## Objetivo profesional y Contacto
Objetivo: Trabajar en una empresa conocida como:(Corporación Microsoft,Corporación Nvidia) .
Contacto: loldfases@gmail.com 


## Habilidades
* **Frontend:** HTML5, CSS3, JavaScript.
* **Backend:** PHP, Java, Node.js.
* **Bases de Datos:** MySQL, PL/SQL.
* **Herramientas:** Git, Docker, VS Code.
* **Sistemas Operativos:** Windows11, Windows 10, Windows server 2016, Ubuntu 22.04,Ubuntu server  

## Proyectos destacados
*Tecnologías:* Java, `BufferedReader`, `BufferedWriter`, Algoritmos.
  * *Descripción:* Solución basada en el algoritmo de mezcla, optimizada para manejar flujos de datos (`I/O`) de manera eficiente, garantizando que el archivo resultante mantenga el orden.

## Bloque de código
Aquí tienes un ejemplo de cómo manejo la conexión de ficheros:

```java

    //Unir 2 ficheros ordenados en 1 fichero y ordenarlos.
    
    public BufferedReader ordenado(BufferedReader br1, BufferedReader br2) {
        
    }
    
    
    public void mezclar_ficheros(BufferedReader fr1, BufferedReader fr2, BufferedReader fr3, BufferedWriter wr) {
        String linea1;
        String linea2;
        
        try {
            linea1=fr1.readLine();
            linea2=fr2.readLine();
            while (linea1 !=null && linea2 !=null) {
                if (linea1.compareTo(linea2)<0) {
                    wr.write(linea1);
                    wr.newLine();
                    linea1=fr1.readLine();
                    
                }
                else{
                    if (linea1.compareTo(linea2)==0) {
                    wr.write(linea1);
                    wr.newLine();
                    wr.write(linea2);
                    wr.newLine();
                    linea1=fr1.readLine();
                    linea2=fr2.readLine();
                }
                    else{     
                        wr.write(linea2);
                        wr.newLine();
                        linea2=fr2.readLine();
                }
                
                }
                
                
            }
            if (linea1==null) {
                while (linea2!=null) {
                wr.write(linea2);
                wr.newLine();
                linea2=fr2.readLine();
                    
                }
            }
                else{
                        while (linea1!=null) {
                        
                        wr.write(linea1);
                        wr.newLine();
                        linea1=fr1.readLine();
                        
                         }
                    }
                  
        } catch (IOException e) {
            e.printStackTrace();
            
       }
      
     }
    
   }
