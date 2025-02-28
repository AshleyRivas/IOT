# IOT
Código en MicroPython para un sistema de monitoreo de temperatura basado en Internet de las Cosas (IoT) utilizando una Raspberry Pi Pico W y un sensor LM35, con el propósito de capturar, procesar y visualizar datos en la nube mediante ThingSpeak.
Además, se implementará MathWorks en la plataforma para realizar análisis de datos en tiempo real, como el cálculo del promedio de temperatura y la generación de alertas cuando los valores superen un umbral predefinido.

Herramientas necesarias:

-Raspberry Pi Pico W
-Sensor de temperatura LM35
-ThingSpeak (almacenamiento y visualización de datos)
-MathWorks (análisis y procesamiento de datos en ThingSpeak)
-Protoboard y cables.
-Conexión wi-fi.
-Computadora.
-Programa Thonny.

Instalar:
-Programa Thonny https://thonny.org/ 
-Conectar raspberry pi pico W a la computadora
-Ir a la opción de interpreter y seleccionar la raspberry.
-instalar programa y copiar el codigo que te proporcione.

Conexión :

Parte 1: Configuración del Hardware 

-Conectar el sensor LM35 a la Raspberry Pi Pico W:

     VCC: 5V (conectar a VBUS (pin 40) - revisar Pinout)
     
     GND: GND
     
     Salida (Vout): GP26 (ADC0)
     
-Leer la temperatura usando el convertidor ADC de la Pico W.


Parte 2: Programación en MicroPython 

-Utilizar el codigo porporcionado en MicroPython para:

-Conectarse a Wi-Fi (utiliza el usuario y contraseña de tu red).

-Leer la temperatura en °C usando el LM35.

-Convertir la señal analógica a temperatura.

-Enviar los datos a ThingSpeak en field1.

-Enviar datos cada 180 segundos.


Parte 3: Visualización en ThingSpeak 

-Configurar gráficas (Charts) en ThingSpeak para visualizar los datos en tiempo real.

-Configurar MathWorks en ThingSpeak para:

-Calcular el promedio de temperatura en los últimos 10 datos.

-Mostrar un mensaje de alerta si la temperatura es mayor a 35°C.

