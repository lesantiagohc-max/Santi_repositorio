**Documentación de trabajos realizados en la materia de Introducción a la Mecatronica**

---
*Primera Practica*
---
En la primera practica se realizo con la compuerta 74ls555, un circuito que debe prender una luz led en un periodo de 3 a 5 seguntos y viceversa , haciendo que este prenda y se apague dentro de este tiempo dado.

Despues, con el osciloscopio visualizamos las señales de encendido y apagado que nos daba el circuito.







*Segunda Practica*
---
En la segunsa practica se abordo el tema del ESP32, con el cual despues de introduirnos a el, realizamos un circuito el cual concistia en encender una luz led, mediante el uso de un boton. Despues de terminar ese circuito, se procedio a realizar otro, el cual hace que la luz del parpade intermitentemente.

Código de circuito 1:

const int led-26;

const int boton=34:

void setup() {

Serial.begin(115200);

pinMode (led, OUTPUT):

pinMode (boton, INPUT):
}
void loop() {

// put your main code

int estado - digitalRead (boton);

if(estado == 1){

digitalwrite(led,1);
}
else{

digitalwrite(led,0);
}
}

Código de circuito 2:








*Tercera Practica*
---
En la tercera practica se usaron el ESP32 y motores, con los cuales se hizo un circuito el cual su funcion era hacer el motor funcionar, despues de eso se añadio una midificacion al codigo, haciendo que el mototor acelerara gradualmente a su maximo y despues disminuir su velocidad gradualmente hasta dejar se funcionar.

Codigo:





*Cuarta Practica (Proyecto Segundo Parcial)*
---
