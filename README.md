# Tarea-3_VLSI
Tarea #3
## Parte 1.
Primeramente, se realiazaron las intancias en el Custom Compiler de lo que es el equematico y el trazado del flip flop estático Amo-Esclavo de 1 bit, se adjunta las evidencias en las siguientes imágenes.

## Parte 2.
Seguidamente se implementó lo que sería una señal de reloj utilizando la fuente de pulsos, para simular un reloj real. Debido a que es una señal sin retardos, se le colocaron 2 inversores con un tamaño de 1X y 4X. De esta manera se hace una merara realista de lo que es una pendiente de clk a las entradas del flip flop. Se adjuntan las evidencias en las siguientes imágenes.

## Parte 3.
Para esta parte se debe realizar una comparación de datos simulados con los datos provistos por el fabricante. Utilizando Liberty Displayer, se obtuvieron las características eléctricas del flip flop. Una vez teniendo el reloj listo, se implementaron una serie de simulaciones que nos permitieron determinar y comparar los datos provistos por el fabricante. Se adjunta la tabla comparativa y las imágenes de las simulaciones.
| Tiempo | Fabricante | Simulado |
|--------------|--------------|------------|
| C. tpdf      | 276.8 ps     | 215 ps     |
| C. tcdf      | 203.23 ps    | 212 p      |
| C. tpdr      | 349 ps       | 269 p      |
| C. tcdr      | 146.2 ps     | 164 p      |
| S. tpdf      | 331.24 ps    | 316 ps     |
| S. tcdf      | 95.15 ps     | 76.2 ps    |
| S. tpdf      | 190.3 ps     | 176 ps     |
