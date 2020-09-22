# Instalación y configuración de Java Development Kit (JDK)

A continuación se explica el paso a paso de la instalación de JDK, de acuerdo al Sistema Operativo que utilice.

### Sistemas Unix

1. Agregamos el repositorio para descargar Java8 de Oracle:<br />
    ```sudo add-apt-repository ppa:webupd8team/java``` <br />
    ```sudo apt-get update```
2. Instalamos desde los repositorios agregados Java: <br />    
    ```sudo apt-get install oracle-java8-installer``` <br />  
3. Definimos que por default se utilice Java 8: <br />  
    ```sudo apt-get install oracle-java8-set-default ``` <br />  
    ```sudo update-alternatives --config java ``` <br />   
4. Una vez descargados e instalados, debemos configurar la variable de entorno JAVA_HOME (Verificar el path donde se instaló JDK en esa máquina):
    - Definimos la variable de entorno __$JAVA_HOME__: <br />  
          ```sudo gedit /etc/environment``` <br />  
        ```JAVA_HOME="/usr/lib/jvm/java-8-oracle"``` <br />        
    - Volvemos a cargar el archivo environment para que tome los cambios: <br />  
        ```source /etc/environment``` <br />     

### Sistemas Windows

1. En Windows, descargamos el instalador desde la web de Oracle en http://www.oracle.com/technetwork/java/index.html.
2. Una vez descargados e instalados, debemos configurar la variable de entorno __JAVA_HOME__ (Verificar el path donde se instaló JDK en esa máquina):
    - Hacemos click derecho sobre _“Mi PC”_ ó _“Este equipo”_, de acuerdo a la versión del SO, y seleccionamos la opción _“Propiedades”_. Luego accedemos a __“Configuración avanzada / Cambiar configuración -> Opciones avanzadas -> Variables de entorno -> Nueva (Variables del sistema)”__.
    - Configuramos la variable __JAVA_HOME__. Para ello, escribimos en el cuadro de texto lo siguiente:
          - __Nombre de variable__: JAVA_HOME,
          - __Valor de variable__: ruta en que se haya instalado Java. Por ejemplo “C:\Program Files\Java\jdk1.7.0_51”.
        


