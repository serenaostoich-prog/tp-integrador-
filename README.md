# Sistema de Posicionamiento y Calibración de Sensores

  El proyecto consiste en realizar una estación de caracterización de sensores y control de posición digital en tiempo real construida sobre la estructura de un riel y carro de impresora reciclado. El sistema cumple una doble función: 
  
## 1. Modo Caracterización / Calibración:
  Realiza un barrido mecánico paso a paso a lo largo del riel. En cada posición fija, se toman lecturas del sensor analógico de distancia y envía pares de datos (Posición_Real, Voltaje_ADC) por comunicación serie UART a una PC para generar automáticamente la curva de calibración ( V vs. D ) del sensor. 
  
## 2. Modo Control de Posición: 
  Recibe una posición deseada desde la PC o teclado. El microcontrolador ejecuta internamente un algoritmo de control Proporcional-Integral (PI) que ajusta la velocidad y sentido del motor mediante PWM, garantizando que el carro se ubique en la posición objetivo con error estacionario cero y sin sobrepasos bruscos.

  
  
