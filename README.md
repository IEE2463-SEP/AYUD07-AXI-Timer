# AYUD07 · AXI Timer

> En esta ayudantía utilizaremos el IPCore AXI Timer en nuestro diseño de hardware para luego habilitar interrupciones periódicas mediante software. Se implementa en la tarjeta ZYBOZ7.

Ejercitaremos el uso de interrupciones y también aprenderemos a habilitar el modo PWM que admite AXI Timer, esto último para variar la intensidad del canal R del led RGB modificando el duty cycle de la señal PWM que generaremos.

Adicionalmente también revisaremos cómo programar la Zybo desde ambos programas: desde Vitis y desde Vivado.

---

## 🎥 Antes de la ayudantía

Previo a nuestra ayudantía debes revisar este [video](https://youtu.be/eUUw3ANzMpg) y ejecutarlo en tu casa.

[![Video de la ayudantía 07](https://img.youtube.com/vi/eUUw3ANzMpg/hqdefault.jpg)](https://youtu.be/eUUw3ANzMpg)

---

## 📂 Material

Los documentos asociados a la ejecución de este laboratorio son:

| Archivo | Descripción |
| :--- | :--- |
| [AYUD07-Guia Ejercicio](https://github.com/IEE2463-SEP/AYUD07-AXI-Timer/blob/HEAD/AYUD07_AXI_TIMER.pdf) | Guía de ejercicios asociado a la ayudantía. |
| [Timer_Ints.c](https://github.com/IEE2463-SEP/AYUD07-AXI-Timer/blob/HEAD/Timer_Ints.c) | El cual contiene el código C utilizado en la ayudantía para generar las interrupciones |
| [Zybo-Z7_Master.xdc](https://github.com/IEE2463-SEP/AYUD07-AXI-Timer/blob/HEAD/Zybo-Z7-Master.xdc) | El cual contiene los constraints de nuestra tarjeta (mapeo de pines) |
| [Ay_AXI_Timer_Ints.zip](https://github.com/IEE2463-SEP/AYUD07-AXI-Timer/blob/HEAD/Ay_AXITimer_Ints.zip) | Contine el projecto en vivado/vitis desarrollado en la ayudantía |

---

## 🧪 Durante la ayudantía

Durante la ayudantía se busca que desarrollen el ejercicio propuesto de la guía, el cual consiste en trabajar sobre el código [test_pwm.c](https://github.com/IEE2463-SEP/AYUD07-AXI-Timer/blob/HEAD/test_pwm.c) haciendo una leve modificación de hardware, donde se habilita el modo PWM del IP Core AXI Timer, pero los parámetros PWM_PERIOD, CYCLE_PER_DUTYCYCLE y DUTYCYCLE_DIVISOR deben ser modificados de forma que la PWM generada sea lo suficientemente rápida para que en el canal R del led RGB se aprecie una variación en la intensidad de la luz que emite. Más detalles pueden consultarse en la guía [AYUD07-Guia Ejercicio](https://github.com/IEE2463-SEP/AYUD07-AXI-Timer/blob/HEAD/AYUD07_AXI_TIMER.pdf).

---

<sub>IEE2463 · Sistemas Electrónicos Programables</sub>
