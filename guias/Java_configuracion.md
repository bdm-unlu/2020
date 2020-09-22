# Instalación y configuración de Java Development Kit (JDK)

A continuación se explica el paso a paso de la instalación de JDK, de acuerdo al Sistema Operativo que utilice.

### Sistemas Unix

1. Agregamos el repositorio para descargar Java8 de Oracle: 
  sudo add-apt-repository ppa:webupd8team/java 
  sudo apt-get update 
2. Instalamos desde los repositorios agregados Java: 
  sudo apt-get install oracle-java8-installer 
3. Definimos que por default se utilice Java 8:
  sudo apt-get install oracle-java8-set-default 
  sudo update-alternatives --config java
4. Una vez descargados e instalados, debemos configurar la variable de entorno JAVA_HOME (Verificar el path donde se instaló JDK en esa máquina):
    - Definimos la variable de entorno $JAVA_HOME:
      sudo gedit /etc/environment
      JAVA_HOME="/usr/lib/jvm/java-8-oracle"
    - Volvemos a cargar el archivo environment para que tome los cambios:
      source /etc/environment

### Sistemas Windows

1. En Windows, descargamos el instalador desde la web de Oracle en http://www.oracle.com/technetwork/java/index.html.
2. Una vez descargados e instalados, debemos configurar la variable de entorno JAVA_HOME (Verificar el path donde se instaló JDK en esa máquina):
    - Hacemos click derecho sobre “Mi PC” ó “Este equipo”, de acuerdo a la versión del SO, y seleccionamos la opción “Propiedades”. Luego accedemos a “Configuración avanzada / Cambiar configuración -> Opciones avanzadas -> Variables de entorno -> Nueva (Variables del sistema)”.
    - Configuramos la variable JAVA_HOME. Para ello, escribimos en el cuadro de texto lo siguiente:
        - Nombre de variable: JAVA_HOME,
        - Valor de variable: ruta en que se haya instalado Java. Por ejemplo “C:\Program Files\Java\jdk1.7.0_51”.
        


