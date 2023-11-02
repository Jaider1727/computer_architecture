Introducción

Se integrarán los componentes de hardware previamente desarrollados en un sistema informático completamente funcional donde el objetivo principal es ensamblar una plataforma de hardware capaz de ejecutar programas escritos en el lenguaje de máquina Hack introducido en el Proyecto 4 con 3 componentes, memoria, CPU y computadora.

Desarrollo:
#Memoria: Esto incluye RAM16K, Pantalla y Teclado. Si bien los chips de Pantalla y Teclado están disponibles como componentes integrados, se recomienda usar la versión integrada de RAM16K para agilizar el proceso de desarrollo.

#CPU: La Unidad Central de Procesamiento se construirá utilizando la ALU del Proyecto 2, junto con los chips de Registro y PC del Proyecto 3 y compuertas lógicas del Proyecto 1. Sin embargo, para mantener la coherencia con los scripts de prueba del proyecto, se recomienda utilizar los chips integrados ARegister, DRegister y PC.

#Memoria de Instrucciones: Para almacenar y ejecutar programas, utilizarás el chip integrado ROM32K, que es similar en función a los chips de RAM desarrollados en el Proyecto 3, pero cuenta con una interfaz para cargar programas desde archivos de texto.

#Computador: Este chip de nivel superior se crea combinando la CPU, la Memoria y el ROM32K. La CPU y la Memoria se construyen en este proyecto, mientras que el ROM32K es un chip integrado.

Para evaluar la funcionalidad de programas de prueba proporcionados: Add, Max y Rect.
