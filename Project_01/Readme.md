# Proyecto_01
(POR FAVOR ABRIR EL EDITOR)
INTRODUCCIÓN
Se desarrolló una serie de compuertas con el lenguaje de HDL(chips) ,las cuales por medio de funciones secuenciales a las cuales se les ingresaba "INs" y "OUTs" 
se fueron creando. Con el tiempo se crearon y mejoraron la cantidad de compuertas debido a que se iban reutilizando los chips.


DESARROLLLO

Estas fueron las compuertas que se usaron junto con su tabla de verdad: 
![1_Compuertas_logicas_digitales](https://github.com/Jaider1727/computer_architecture/assets/132866666/6eb6cf56-4c73-4299-9878-2a276f4b5999)

Se intentaron implementar en HDL mediante la siguiente sintaxis (Ejemplificado en la compueta "NOT"): 

CHIP Not {
    IN in;
    OUT out;

    PARTS:
    Nand(a=in, b=in, out=out);
}


La parte superior (CHIP) representa las entradas y salidas del chip, y la función inferior (PARTS) es la función que le da funcionalidad al presente chip. Para esto debemos tener en cuenta que ya hemos creado funciones previas y que la función principal del programa es la compuerta "NAND" que es la base para futuras compuertas.

CONCLUSIÓN

1*Este programa es muy útil ya que podemos crear compuertas más complejas, reutilizando compuertas ya creadas. 
2*El programa que se usa en el curso es bastante intuitivo y fácil de aprender, por lo que no será problema crear cosas nuevas. 

