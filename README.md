# Conceptos de dinamica de sistemas
## 1. Sistemas
Un sistema es un conjunto de componentes que interactuan entre si para alcanzar un objetivo especifico

**Ejemplo:** Un sistema de calefaccion domestico, donde el termostato, la caldera y los sensores tranajan entre si para mantener una temperatura deseada
## 2. Sistema dinamico
Si la salida del sistema depende de la historia pasada de la entrada, se le dice que es un **sistema dinamico**

**Ejemplo:** Un automovil, cuya velocidad en un momento dado depende de la aceleracion o frenado aplicados previamente

### Diferencia entre un sistema estatico y dinamico:

**1. Sistema estatico:** Un resistor electrico en el que la corriente depende instantaneamente del voltaje aplicado

**2. Sistema dinamico:** Un circuito con condensadores e inductores, donde la respuesta depende del tiempo
## 3. Planta
Se refiere a la parte fisica del sistema que realiza la trasformacion de entrada a salida

**Ejemplo:** Un motor electrco que convierte la energia electrica en movimiento mecanico
## 4. Proceso
Es un conjunto de pasoso para lograr un objetivo en un sistema

**Ejemplo:** En la industria quimica, la destilacion del petroleo es un proceso donde se separan sus componentes en diferentes fracciones
# Modelamiento matematico de sistemas
## 1. Modelos dinamicos
Estos modelan la variacion de una variable conforme pasa el tiempo, estos son expresados con **ecuaciones diferenciales**

**Ejemplo:**

1. Sistema de un tanque de agua con salida:

El nivel de agua h(t) en un tanque con una válvula de salida se modela con la ecuación:

$$A\frac{dh}{dt} = -C\sqrt{h}$$

2. Modelo de crecimiento poblacional:

Si una población crece proporcionalmente a su tamaño:

$$\frac{dP}{dt} = rP$$

donde r es la tasa de crecimiento. La solución es $$P(t) = Po * e^{rt}$$
## Recordando calculo diferencial

**Ejemplos**

1. Movimiento rectilíneo uniformemente acelerado:

Un automóvil parte del reposo y acelera a razón de $$a=5 m/s^2.$$

La velocidad es $$v(t)=∫5dt=5t$$

La posición es $$x(t)=∫5tdt=\frac{5}{2}t^2$$

2. Temperatura de un objeto (Ley de Newton del Enfriamiento):

Un café caliente a 80°C en una habitación a 25°C se enfría según: 

$$\frac{dT}{dt}=−k*(T−25)$$

donde k es una constante de enfriamiento.
## Caracteristecas de ecuaciones diferenciales

1. Ecuación lineal invariante en el tiempo:

$$\frac{d^2x}{dt^2} + 3*\frac{dx}{dt} +2x=0$$

Su solución describe el comportamiento de un resorte amortiguado.

2. Ecuación no lineal variante en el tiempo:

$$\frac{d^2y}{dt^2} + e^tsin(y)=0%%

No se puede resolver fácilmente con métodos clásicos.
