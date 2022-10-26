![titulo](cooltext419799253098610.png)

Un potenciómetro es un resistor eléctrico con un valor de resistencia variable y generalmente ajustable manualmente. Los potenciómetros utilizan tres terminales y se suelen utilizar en circuitos de poca corriente, para circuitos de mayor corriente se utilizan los reóstatos.

En muchos dispositivos eléctricos los potenciómetros son los que establecen el nivel de salida. Por ejemplo, en un altavoz el potenciómetro ajusta el volumen; en un televisor o un monitor de ordenador se puede utilizar para controlar el brillo.

![](https://upload.wikimedia.org/wikipedia/commons/b/b5/Potentiometer.jpg)

![](https://i0.wp.com/www.ingmecafenix.com/wp-content/uploads/2017/04/Simbolo-potenciometro.webp?resize=683%2C384&ssl=1)

## Construcción de un potenciómetro
### Impresos:
Realizadas con una pista de carbón o de cermet sobre un soporte duro como papel baquelizado, fibra de vidrio, baquelita, etc. La pista tiene sendos contactos en sus extremos y un cursor conectado a un patín que se desliza por la pista resistiva.

![](https://i0.wp.com/www.ingmecafenix.com/wp-content/uploads/2017/04/Potenciometro.webp?resize=683%2C384&ssl=1)

### Bobinados:
Consiste en un bobinado toroidal de un hilo resistivo con un cursor que mueve un patín sobre el mismo.

![](https://i0.wp.com/www.ingmecafenix.com/wp-content/uploads/2017/04/Potenciometro-bobinado.webp?resize=683%2C384&ssl=1)


## Tipos de potenciometro
### Giratorios
Se controlan girando su eje, son los mas usados por que son de larga duración y usan poco espacio.

![](https://i0.wp.com/www.ingmecafenix.com/wp-content/uploads/2017/04/Potenciometro-deslizante.webp?resize=683%2C384&ssl=1)

### Deslizantes
El recorrido del cursor es de forma recta, se utilizan en  ecualizadores gráficos.

![](https://i0.wp.com/www.ingmecafenix.com/wp-content/uploads/2017/04/Potenciometro-lineal.webp?resize=683%2C384&ssl=1)

### Potenciómetros de ajuste
Controlan la tensión preajustándola, normalmente en fábrica. El usuario no suele tener que retocar, por lo que no suelen ser accesibles desde el exterior. Existen tanto encapsulados en plástico como sin cápsula, y se suelen distinguir potenciómetros de ajuste vertical, cuyo eje de giro es vertical, y potenciómetros de ajuste horizontal, con el eje de giro paralelo al circuito impreso.

![](https://i0.wp.com/www.ingmecafenix.com/wp-content/uploads/2017/04/Potenciometro-de-ajuste.webp?resize=683%2C384&ssl=1)

### Potenciómetros Digitales
Se usan para sustituir a los mecánicos simulando su funcionamiento y evitando los problemas mecánicos de estos últimos. Está formado por un circuito integrado que simula el comportamiento de su equivalente analógico. Tienen un divisor resistivo (divisor de tensión) con n+1 resistencias.

![](https://i0.wp.com/www.ingmecafenix.com/wp-content/uploads/2017/04/Potenciometro-digital.webp?resize=683%2C384&ssl=1)

### Codigo de prueba

```python
from machine import ADC
import utime

adc = ADC(2)

while True:
  pot = adc.read_u16()
  print(pot)
  utime.sleep_ms(200)
```

# Daniel Garcia Salas Daniel Alberto
