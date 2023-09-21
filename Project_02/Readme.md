INTRODUCCIÓN

En el proyecto 1 se construyeron las compuertas básicas para el funcionamiento de una computadora, sin embargo, estas compuertas por si solas no tienen sentido en sí. Por este motivo, en el presente proyecto se crearán chips HalfAdder,FullAdder,Add16,Inc16, capaces de realizar operaciones aritméticas (derivadas de la suma) para que la CPU ya pueda procesar datos.
Por último, por medio de los chips aritméticos, se creará la unidad Aritmético-Lógica(ALU) que es la que recibe instrucciones y datos de la memoria y ejecuta las operaciones especificadas por el programa en ejecución, desempeñando un papel crucial en la ejecución de operaciones matemáticas y lógicas en una computadora.

![image](https://github.com/Jaider1727/computer_architecture/assets/132866666/e148ea8c-65d0-4355-82f9-1c3fea1092d6)

DESARROLLO
Se mostrará el funcionamiento de cada uno de los chips

#1. HalfAdder: Por medio del chip Xor y And se construyó esta compuerta la cual tiene como función principal es realizar la suma binaria de dos bits de entrada y generar dos salidas: una para el resultado de la suma (denominada suma) y otra para el acarreo (carry-out).

![WhatsApp Image 2023-09-21 at 5 49 26 PM](https://github.com/Jaider1727/computer_architecture/assets/132866666/68614e0b-ff74-408c-b6a2-ca716eb7935c)


#2. FullAdder: Por medio de 2 chips HalfAdder y un Or se construyó esta compuerta que a diferencia del Half Adder, el Full Adder es capaz de sumar tres bits de entrada en lugar de solo dos. Sus tres entradas son A, B y un acarreo de entrada (Cin), y tiene dos salidas: una para el resultado de la suma (Sum) y otra para el acarreo de salida (Cout).
es esencial en la aritmética binaria y se utiliza para sumar números binarios de múltiples bits, donde el acarreo de una suma anterior se introduce como acarreo de entrada en la siguiente suma.

![WhatsApp Image 2023-09-21 at 5 49 26 PM (1)](https://github.com/Jaider1727/computer_architecture/assets/132866666/4f6178eb-0fc9-4723-a19f-141491a1d366)


#3. Adder:
Un adder de 16 bits se puede construir utilizando múltiples Full Adders en cascada. Cada Full Adder toma tres bits de entrada (dos bits de los números que se suman y un acarreo de entrada) y genera dos salidas: la suma de tres bits y el acarreo de salida.

![WhatsApp Image 2023-09-21 at 5 49 26 PM (2)](https://github.com/Jaider1727/computer_architecture/assets/132866666/fd0a671d-c91f-4dc3-8f0d-ce78def81a74)

Para construir un sumador de 16 bits, se conectarían 16 Full Adders en serie, donde el acarreo de salida de un Full Adder se conecta como acarreo de entrada al siguiente Full Adder. Los dos números binarios de 16 bits que se desean sumar se aplican como entradas a los Full Adders, y el acarreo de entrada al primer Full Adder generalmente se establece en cero, ya que es la operación inicial.
El resultado de la suma se obtiene a partir de las salidas de suma de los Full Adders individuales, y el acarreo de salida del último Full Adder representa el acarreo más significativo de la suma de 16 bits.

#4. inc16:
Un incremento de 16 bits, a menudo llamado "inc16", es una operación que implica sumar 1 a un número de 16 bits. Esto es similar a realizar una adición de 1 al número almacenado en un registro o una ubicación de memoria de 16 bits.

![WhatsApp Image 2023-09-21 at 5 49 26 PM (3)](https://github.com/Jaider1727/computer_architecture/assets/132866666/af88975b-33a8-4179-a5d5-302185bf81ea)

Para llevar a cabo un incremento de 16 bits, puedes usar un sumador de 16 bits, como un sumador completo o un conjunto de Full Adders conectados en cascada, para agregar 1 al número binario de 16 bits.

#5. ALU:
El ALU se construyó mediante la combinación de componentes lógicos, sumadores y registros de resultado, controlados por una unidad de control, para realizar operaciones aritméticas y lógicas en los datos que se explicaron mediante comentarios en el .hdl.

![WhatsApp Image 2023-09-21 at 5 50 30 PM](https://github.com/Jaider1727/computer_architecture/assets/132866666/ee45f15b-bc9b-4476-9e41-f45575b68ab3)

