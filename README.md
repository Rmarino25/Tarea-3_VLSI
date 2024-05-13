# Tarea-3_VLSI
Tarea #3
## Parte 1.
Primeramente, se realiazaron las intancias en el Custom Compiler de lo que es el equematico y el trazado del flip flop estático Amo-Esclavo de 1 bit, se adjunta las evidencias en las siguientes imágenes.
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Esquematico del flip flop Amo-Esclavo de 1 bit</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Layout del flip flop Amo-Esclavo de 1 bit</em>
</p>
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Post-trazado con parásitas del flip flop Amo-Esclavo de 1 bit</em>
</p>

## Parte 2.
Seguidamente se implementó lo que sería una señal de reloj utilizando la fuente de pulsos, para simular un reloj real. Debido a que es una señal sin retardos, se le colocaron 2 inversores con un tamaño de 1X y 4X. De esta manera se hace una merara realista de lo que es una pendiente de clk a las entradas del flip flop. Se adjuntan las evidencias en las siguientes imágenes.
<p float="center">
  <img src="https://github.com/Rmarino25/Tarea-2_VLSI/assets/110353604/c39b46da-6a98-491f-b0a4-98da1df38584" width="500"  /><br>
     <em>Flip flop con entradas y salidasd</em>
</p>

## Parte 3.
Para esta parte se debe realizar una comparación de datos simulados con los datos provistos por el fabricante. Utilizando Liberty Displayer, se obtuvieron las características eléctricas del flip flop. Una vez teniendo el reloj listo, se implementaron una serie de simulaciones que nos permitieron determinar y comparar los datos provistos por el fabricante. Se adjunta la tabla comparativa y las imágenes de las simulaciones.
| Tiempo | Fabricante | Simulado |
|--------------|--------------|------------|
| Setup D to CN (rise) | 0.2731 ns    | 215 ps     |
| Setup D to CN (fall) | 1.1499 ns    | 212 p      |
| Hold D to CN (rise)  | 1.6704 ns    | 269 p      |
| Hold D to CN (fall)  | 0.7623 ns    | 164 p      |
| Delay CN to Q (low to high) | 0.9109 ns   | 316 ps     |
| Delay CN to Q (high to low) | 0.9440 ns   | 76.2 ps    |

