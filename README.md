
**Actividad 07 - Parte 1: Optimización heurística**

**Decisiones bajo incertidumbre**

**Por: Giovanna Andrea Carmona Valencia - Hilber García López**

**Objetivo**: Optimización de funciones de prueba utilizando algunos métodos de optimización heurística además del método de gradiente descendente, como:

1. Los algortimos evolutivos
2. Optimización de partículas
3. Evolución diferencial

**Actividad: Optimización**

1. Escoja dos funciones de prueba

Para efectos de esta actividad se seleccionaron las funciones de Rosenbrock y Goldstein-Price:

**Función de Rosenbrock:** f(x1,x2)=100(x2−x21)2+(1−x1)2, xi∈[−2.048,2.048], i=1,2. Alcanza su valor mínimo en x1=1 y x2=1.

**Función Goldstein-Price:** f(x1,x2)=[1+(x1+x2+1)2(19−14x1+3x21−14x2+6x1x2+3x22)] ×[30+(2x1−3x2)2(18−32x1+12x21+48x2−36x1x2+27x22)], xi∈[−2,2], i=1,2. Alcanza su valor mínimo en x1=0 y x2=−1.

**1.1.** Optimice las funciones en dos y tres dimensiones usando un método de descenso por gradiente con condición inicial aleatoria:

El método del gradiente descendente permite converger hacia el valor mínimo de una función a través de un proceso iterativo, este consiste  en:
-	Seleccionar aleatoriamente un punto de inicio
-	Calcular la primera derivada respecto a x y y
-	Restar a la derivada cada uno de los parámetros multiplicado por la velocidad de aprendizaje
-	Iterar el cálculo del valor de la función del costo de acuerdo con los puntos encontrados
-	Repetir el proceso iterativo hasta minimizar la función
Este método es comúnmente utilizado para funciones lineales 
 
En el archivo [Punto 1_1](1.1 Gradiente_descendente.py) se desarrolla el método de gradiente descendente para las dos funciones seleccionadas

**1.2.** Optimice las funciones en dos y tres dimensiones usando: algoritmos evolutivos, optimización de partículas y evolución diferencial

**1.2.1. Algoritmos evolutivos:** Son estrategias de optimización y búsqueda de soluciones que toman como inspiración la evolución en distintos sistemas biológicos. La idea fundamental de estos algoritmos es mantener un conjunto de individuos que representan una posible solución del problema. Estos individuos se mezclan y compiten entre sí, siguiendo el principio de selección natural por el cual sólo los mejor adaptados sobreviven al paso del tiempo. En estos algoritmos se busca una pareja de valores que minimice la función, luego se crea una población de cromosomas sobre los cuales se aplican uno o varios operadores genéticos y se fuerza una presión selectiva (los operadores utilizados se aplicarán sobre estos cromosomas, o sobre poblaciones de ellos).

Este algortimo se desarrolla en el archivo [1.2.1. Algortimos genéticos](1.2.1. Algortimo_genetico.py)

**1.2.2. Optimización de partículas:** La optimización por enjambre de partículas (Particle Swarm Optimization, PSO) es un método de optimización heurística orientado a encontrar mínimos o máximos globales. Su funcionamiento está inspirado en el comportamiento que tienen las bandadas de pájaros o bancos de peces en los que, el movimiento de cada individuo (dirección, velocidad, aceleración), es el resultado de combinar las decisiones individuales de cada uno con el comportamiento del resto.

Este algortimo se desarrolla en el archivo [1.2.2. Optimización de partículas](1.2.2. Optimizacion_particulas.py)

**1.2.3. Evolución diferencial:** El algoritmo funciona manteniendo una población de soluciones candidatas representadas como vectores de valor real. Las nuevas soluciones candidatas se crean mediante la creación de versiones modificadas de las soluciones existentes que luego reemplazan a una gran parte de la población en cada iteración del algoritmo. Las nuevas soluciones candidatas se crean con una solución base a la que se agrega una mutación y otras soluciones candidatas de la población a partir de la cual se calcula la cantidad y el tipo de mutación, llamado vector de diferencia.  Este método genera nuevos vectores de parámetros sumando la diferencia ponderada entre dos vectores de población a un tercer vector.

Este algortimo se desarrolla en el archivo [1.2.3. Evolución diferencial](1.2.3. Evolucion_diferencial.py)

1.3. Represente con un gif animado o un video el proceso de optimización de descenso por gradiente y el proceso usando el método heurístico

En los archivos [1.3.1 GD](1.3.1. GDGif.gif) y [1.3.2. Optimización de partículas](1.3.2. EPGif.gif) se desarrollan los gifs animados para el proceso de optimización de descenso del gradiente descendiente y el método de optimización de partículas

