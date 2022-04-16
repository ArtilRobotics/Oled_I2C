# Oled_I2C
Ejemplo de arduino para importar de imagenes jpg, png a pantalla Oled
 
2
 

 
Probar en código que tanto se puede animar un rostro en este tipo de

pantallas.

Para poder probar la OLED 128x32 es necesario instalar las siguientes librerías

de Adafruit
 ![img1](https://github.com/ArtilRobotics/Oled_I2C/blob/main/Images/Libreria%20Arduino%20OLED.jpg)














 
En la opción de ejemplos se puede probar la OLED
 
3
 

 
Tener en cuenta que si se trata de una OLED 128x64 o 128x32 se puede

cambiar unos aspectos de la programación de la librería dependiendo el caso
 












 
En lo subrayado se encuentra para una OLED 128x64 si se trabajase con una

OLED 128x32 se cambia los siguientes aspectos.

64 por 32 y el 3D por 3C

Animar la cara en mapa de bits

Link: https://diyusthad.com/image2cpp
 
4 
5

1. Se selecciona la imagen a convertir en mapa de bits

2. Configuramos las medidas de la OLED (128x32 a 128x64), y se

configura su centrado como en la imagen

3. Visualización previa

4. Se selecciona la opción del Arduino code y generan el código y ese

código lo pegan en la siguiente programación

``` 
Adafruit_SSD1306 display(128, 32, &Wire, OLED_RESET);
``` 
Y cambiar la C por la D
``` 
display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
``` 
