<<<<<<< HEAD
# Oled_I2C
## Ejemplo de arduino para importar de imagenes jpg, png a pantalla Oled
### Probar en código que tanto se puede animar un rostro en este tipo de pantallas.
=======
# Oled_I2C 
Ejemplo de arduino para importar de imagenes jpg, png a pantalla Oled,
 
2
 

 
Probar en código que tanto se puede animar un rostro en este tipo de

pantallas.
>>>>>>> 23485bb15f5a60aef1e00232864b97a03d910af2

Para poder probar la OLED 128x32 es necesario instalar las siguientes librerías

de Adafruit
 ![img1](https://github.com/ArtilRobotics/Oled_I2C/blob/main/Images/Libreria%20Arduino%20OLED.jpg)

En la opción de ejemplos se puede probar la OLED
 
 ![img2]()
 
Tener en cuenta que si se trata de una OLED 128x64 o 128x32 se puede cambiar unos aspectos de la programación de la librería dependiendo el caso
![img3]()

En lo subrayado se encuentra para una OLED 128x64 si se trabajase con una OLED 128x32 se cambia los siguientes aspectos.

*64 por 32 y el 3D por 3C*

Animar la cara en mapa de bits

Link: https://diyusthad.com/image2cpp
 
![img4]()
![img5]()

1. Se selecciona la imagen a convertir en mapa de bits

2. Configuramos las medidas de la OLED (128x32 a 128x64), y se

configura su centrado como en la imagen

3. Visualización previa

4. Puede visualizar el codigo de la OLED_I2C donde en el caso de que tratase de una oled de 128x32 o 128x64 debera modificar el 32 por 64

``` 
Adafruit_SSD1306 display(128, 32, &Wire, OLED_RESET);
``` 
Y cambiar la C por la D
``` 
display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
``` 
