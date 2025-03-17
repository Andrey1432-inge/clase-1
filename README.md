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

**1. Sistema de un tanque de agua con salida:**

El nivel de agua h(t) en un tanque con una válvula de salida se modela con la ecuación:

$$A\frac{dh}{dt} = -C\sqrt{h}$$

**2. Modelo de crecimiento poblacional:**

Si una población crece proporcionalmente a su tamaño:

$$\frac{dP}{dt} = rP$$

donde r es la tasa de crecimiento. La solución es $$P(t) = Po * e^{rt}$$
## 2. Recordando calculo diferencial

**Ejemplos**

**1. Movimiento rectilíneo uniformemente acelerado:**

Un automóvil parte del reposo y acelera a razón de $$a=5 m/s^2.$$

La velocidad es $$v(t)=∫5dt=5t$$

La posición es $$x(t)=∫5tdt=\frac{5}{2}t^2$$

**2. Temperatura de un objeto (Ley de Newton del Enfriamiento):**

Un café caliente a 80°C en una habitación a 25°C se enfría según: 

$$\frac{dT}{dt}=−k*(T−25)$$

donde k es una constante de enfriamiento.
## 3. Caracteristecas de ecuaciones diferenciales

**1. Ecuación lineal invariante en el tiempo:**

$$\frac{d^2x}{dt^2} + 3*\frac{dx}{dt} +2x=0$$

Su solución describe el comportamiento de un resorte amortiguado.

**2. Ecuación no lineal variante en el tiempo:**

$$\frac{d^2y}{dt^2} + e^tsin(y)=0$$

No se puede resolver fácilmente con métodos clásicos.
## 4. Sistemas lineales y no lienales

**1. Sistema lineal:**

Un amplificador de audio: La señal de salida es proporcional a la señal de entrada.

**2. Sistema no lineal:**

Una brújula con fricción: La respuesta no es proporcional a la entrada debido a efectos de saturación y resistencia.

## 5. Modelamiento y validacion
**1. Validación de un modelo de caída libre:**

Se mide la caída de una pelota desde 10 m y se compara con la ecuación 

$$y = \frac{1}{2}gt^2$$

**2. Validación de un modelo de control de temperatura:**

Se compara la respuesta de un sistema de calefacción con predicciones del modelo de control PID.
## 6. Influencia de parametros

Cómo los parámetros afectan la respuesta de un sistema.

**Ejemplos:**

**1. Efecto de la fricción en un péndulo:**

Un péndulo sin fricción oscila indefinidamente, pero con fricción, la amplitud disminuye con el tiempo.

**2.Efecto de la resistencia en un circuito RLC:**

Si la resistencia es alta, el circuito es sobreamortiguado y vuelve lentamente al equilibrio.
# Trasformada de Lapalace
## 1. Introduccion
La Transformada de Laplace convierte ecuaciones diferenciales en ecuaciones algebraicas en el dominio de la frecuencia.

Permite analizar sistemas de control, circuitos eléctricos, y vibraciones mecánicas.

**Ejemplos:**

**1. Sistema de masa-resorte-amortiguador**

La ecuación diferencial del sistema es:

$$m\frac{d^2x}{dt^2} + c\frac{dx}{dt} + kt = F(t)$$

Aplicando la Transformada de Laplace:

$$(ms^2 + cs + k)X(s) = F(s)%%

Se convierte en una ecuación algebraica en s

**2. Circuito RLC en serie:**

La ecuación diferencial del voltaje es:
 
$$L\frac{d^2i}{dt^2} + R\frac{di}{dt} + \frac{i}{c} = V(t)$$

Aplicando la Transformada de Laplace:

$$(Ls^2 + Rs + \frac{i}{C})I/s) = V(s)$$

Facilita la solución del sistema.
## Definicion matematica
Se define como:

$$X(s)=∫{0}{∞} x(t)e^{−st} dt$$

Permite convertir ecuaciones diferenciales en algebraicas.

**Ejemplos:**

**1. Transformada de una función exponencial:**

Si $$x(t)=e^{−at}$$, su transformada es:

$$L{e^{−at} = \frac{1}{s+a}$$
​
 
**2. Transformada de una función senoidal:**

Si $$x(t)=sin(ωt)$$, su transformada es:

$$L{sin(ωt)} = \frac{ω}{s^2+w^2}$$
​

