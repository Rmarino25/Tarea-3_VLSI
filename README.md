# Tarea-3_VLSI
Esta tarea se cetrará en la instanciación y caracterización de un flip flip estático Amo-Esclavo de 1 bit, utilizando la herramienta de Custom Compiler. El objetivo principal es validar el comportamiento eléctrico del flip flop mediante simualciones detallas y comparaciones con los datos del fabricante. Estos procesos son de suma importancia para asegurar fiabilidad y el rendimiento de los sistemas digitales.
## Parte 1.
Primeramente, se realiazaron las intancias en el Custom Compiler de lo que es el equematico y el trazado del flip flop estático Amo-Esclavo de 1 bit, se adjunta las evidencias en las siguientes imágenes.
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-3_VLSI/assets/110353604/8cb61afa-1b4a-4020-a1e9-c7fe0c90b375" width="500"  /><br>
     <em>Esquematico del flip flop Amo-Esclavo de 1 bit</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-3_VLSI/assets/110353604/0dcacbeb-ed65-4807-9a45-b2adfd48a3e4" width="500"  /><br>
     <em>Layout del flip flop Amo-Esclavo de 1 bit</em>
</p>

<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-3_VLSI/assets/110353604/304c6e0f-92da-47a2-b3f3-f8dcfb3b44a5" width="500"  /><br>
     <em>Post-trazado con parásitas del flip flop Amo-Esclavo de 1 bit</em>
</p>

## Parte 2.
Seguidamente se implementó lo que sería una señal de reloj utilizando la fuente de pulsos, para simular un reloj real. Debido a que es una señal sin retardos, se le colocaron 2 inversores con un tamaño de 1X y 4X. De esta manera se hace una simulación realista de lo que es una pendiente de clk a las entradas del flip flop. Se adjuntan las evidencias en las siguientes imágenes.
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-3_VLSI/assets/110353604/3f00d393-24fd-4d62-bddb-0c47f4dcbec5" width="500"  /><br>
     <em>Flip flop con entradas y salidas</em>
</p>

## Parte 3.
Para esta parte se debe realizar una comparación de datos simulados con los datos provistos por el fabricante. Utilizando Liberty Displayer, se obtuvieron las características eléctricas del flip flop. Una vez teniendo el reloj listo, se implementaron una serie de simulaciones que nos permitieron determinar y comparar los datos provistos por el fabricante. Adémas se le incoroporó una carga a la salida de F04 con inversores mínimos. Se adjunta la tabla comparativa y las imágenes de las simulaciones.
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-3_VLSI/assets/110353604/1262b192-d5f5-4e53-8128-6ac78fc99f62" width="500"  /><br>
     <em>Tiempo de setup D to CN (rise)</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Error de setup D to CN (rise)</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-3_VLSI/assets/110353604/181784e1-559a-4c3a-8166-895e5b2df348" width="500"  /><br>
     <em>Tiempo de setup D to CN (fall)</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-3_VLSI/assets/110353604/91cbf82a-d2a5-4e86-b0bf-7c785a909c95" width="500"  /><br>
     <em>Error de setup D to CN (fall)</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Tiempo de hold D to CN (rise)</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Tiempo de hold D to CN (fall)</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Tiempo de CN to Q (low to high)</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Tiempo de CN to Q (high to low)</em>
</p>

En la siguiente tabla se hace una comparación de los datos simulados con los provistos por fabricante.

| Tiempo | Fabricante | Simulado |
|--------------|--------------|------------|
| Setup D to CN (rise) | 0.2731 ns    | 215 ps     |
| Setup D to CN (fall) | 1.1499 ns    | 212 p      |
| Hold D to CN (rise)  | 1.6704 ns    | 269 p      |
| Hold D to CN (fall)  | 0.7623 ns    | 164 p      |
| Delay CN to Q (low to high) | 0.9109 ns  | 316 ps  |
| Delay CN to Q (high to low) | 0.9440 ns  | 76.2 ps |

