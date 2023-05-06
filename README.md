# Variable aleatoria discreta

## Actividad

Teniendo en cuenta lo información dada en la siguiente tabla:

| Tema  | Juan Diego Taborda | Juan Camilo Quiroga | Samuel Toro| Santiago Ramirez| Julian Hernandez|
| ---  | ----| --- | --- | --- | --- |
| **VA continuas**  | 2 | 5 | 1 | 4 | 3 |
| **Uniforme**  | 5 | 4 | 3 | 2 | 1 |
| **Exponencial**  | 3 | 1 | 2 | 5 | 4 |
| **Normal**  | 4 | 3 |5  |1  |2  |

Resuelva cada uno de los problemas claramente a **mano** (tal y como se vio en clase) y usando **python**. Los problemas resueltos a mano deberan ser entregados en clase en hojas mostrando la solución de manera clara, ordenada y bien explicada. Las notebooks de python (archivos con extención **ipynb**) que implementan la solución de los problemas que se la asigno, deberan ser subidos a este repositorio en una carpeta con las iniciales del autor y dentro de esta con los nombres de los archivos siguiendo el siguiente formato de acuerdo a la distribución que se toco y el numero que se le asigno:

|Distribución|Nombre|
|---|---|
|Uniforme|**```uni_#.ipybn```**|
|Exponencial|**```exp_#.ipybn```**|
|Normal|**```normal_#.ipybn```**|

Por ejemplo, de la tabla se puede ver que al estudiante **Santiago Ramirez Acevedo** le toco resolver los siguientes problemas:
* **VA continuas**: 2
* **Uniforme**: 2
* **Exponencial**: 5
* **Normal**: 1

Teniendo en cuenta lo anterior, el estudiante
**Santiago Ramirez Acevedo** debera crear una carpeta con sus iniciales **SRA** realizar lo siguiete y colocar dentro de esta la solución de los problemas  relacionados con las distribuciones de acuerdo nombrandolos de la siguiente manera:

|Distribución|Ejercicio Asignado|Nombre|
|---|---|---|
|Uniforme|5|**```uni_5.ipybn```**|
|Exponencial|4|**```exp_4.ipybn```**|
|Normal|1|**```normal_1.ipybn```**|

Para cada archivo puede usar la plantilla mostrada en el siguiente [link](normal_x.ipynb) adaptandola a su problema en especifico. Recuerde que en al aula virtual del curso se encuentra abundante material de consulta (diapositivas, ejemplos, etc). Tambien, los ejemplos resueltos en clase usando python se encuentran recopilados en el siguiente [link](https://github.com/estocasticos-udem/curso_2023-1/tree/main/variables_aleatorias_continuas) para que recuerde los conceptos claves antes de empezar.

## Problemas

### Variables aleatorias continuas

1. La CDF de una variable aleatoria $W$ es:

$$F_W(w)=\begin{cases}
   0 & \text{; } w < -5 \\ 
   (w+5)/8 & \text{; } -5 \leq w < -3 \\ 
   1/4 +3(w-3)/8 & \text{; } -3 \leq w < 5 \\ 
   1 & \text{; } w \geq 5 
   \end{cases}$$
   
   Calcule:
   * $P[W \leq 4]$
   * $P[-2 \lt W \leq 2]$
   * $P[W > 0]$
   * ¿Cual es el valor de $a$ para el que $P[W \leq a] = 1/2$?

2. Un profesor nunca termina su clase antes del final de la hora y siempre termina dentro de dos minutos después de la hora. Sea ***X = el tiempo que transcurre entre el final de la hora y el final de la disertación*** y suponga que la función de densidad de probabilidad de $X$ es:

$$
   f(x)=\begin{cases}
   kx^2 & \text{; } 0 \leq x \leq 2 \\ 
   0 & \text{; eoc }
   \end{cases}
   $$

   * Determine el valor de $k$ y trace la curva de densidad correspondiente (Recuerde que el area total bajo la curva de $f(x) = 1$)
   * ¿Cuál es la probabilidad de que la clase termine dentro de 1 minuto del final de la hora?
   * ¿Cuál es la probabilidad de que la disertación continúe después de la hora durante entre 60 y 90 segundos?
   * ¿Cuál es la probabilidad de que la disertación continúe durante por lo menos 90 segundos después del final de la hora?

3. Una gasolinera opera dos bombas, cada una de las cuales puede bombear hasta 10000 galones de gasolina en un mes. La cantidad total de gasolina bombeada en un mes es una variable aleatoria ***Y*** (medida en 10000 galones) con una función de densidad de probabilidad dada por

$$
   f(y)=\begin{cases}
   y & \text{; } 0 \lt y \lt 1 \\ 
   2 - y & \text{; } 1 \leq y \lt 2 \\ 
   0 & \text{; eoc }
   \end{cases}
   $$

   * Grafique $f(y)$
   * Encuentre $F(y)$ y grafiquela
   * Encuentre la probabilidad de que la gasolinera bombee entre 8000 y 12000 galones en un mes particular.
   * Dado que la gasolinera bombeó más de 10000 galones en un mes particular, encuentre la probabilidad de que haya bombeado más de 15000 galones durante el mes.

4. El tiempo de falla (en cientos de horas) para un transistor es una variable aleatoria ***Y*** con CDF dada por:

$$
   F(y)=\begin{cases}
   0 & \text{; } y \lt 0 \\ 
   1 - e^{-y^2}  & \text{; } y \geq 0 
   \end{cases}
   $$

   * Encuentre el valor del $\eta$ para el 30° percentil.
   * Encuentre $f(y)$
   * Encuentre la probabilidad de que el transistor opere al menos 200 horas.
   * Encuentre $P(Y > 100 | Y \leq 200)$

5. La función de distribución acumulativa de la variable aleatoria $X$ es:

$$
   F_X(x)=\begin{cases}
   0 & \text{; } x < -1 \\ 
   (x+1)/2 & \text{; } -1 \leq x < 1 \\ 
   1 & \text{; } x \geq 1
   \end{cases}
   $$
   
   * Encuentre $P[X>1/2]$
   * Encuentre $P[-1/2 < X \leq 3/4]$
   * Encuentre $P[|X| \leq 1/2]$
   * ¿Cual es el valor de $a$ para el que $P[X \leq a] = 0.8$?

### Distribución uniforme

1. El artículo "Modeling Sediment and Water Column Interactions for Hidrophobic Pollutants" (Water Research, 1984: 1169–1174) sugiere la distribución uniforme en el intervalo (7.5, 20) como modelo de profundidad (cm) de la capa de bioturbación en sedimento en una región.
   * ¿Cuáles son la media y la varianza de la profundidad?
   * ¿Cuál es la probabilidad de que la profundidad observada sea cuando mucho de 10? ¿Entre 10 y 15?
   * ¿Cuál es la probabilidad de que la profundidad observada esté dentro de 1 desviación estándar del valor medio?
   * ¿Dentro de 2 desviaciones estándar?

2. Suponga que el valor de una acción varía cada día de 16 a 25 dólares con una distribución uniforme.
   * Calcule la probabilidad de que el valor de la acción sea superior a 19 dólares. (**Rta**: $2/3$)
   * Calcule la probabilidad de que el valor de la acción esté entre 19 y 22 dólares. (**Rta**: $1/3$)
   * Halle el cuartil superior (el $25 \%$ de todos los días que la acción está por encima de ¿qué valor?). (**Rta**: $22.75$)
   * Dado que el valor de la acción es mayor de $18$ dólares, calcule la probabilidad de que el valor de la acción sea mayor de 21 dólares. (**Rta**:$𝑃(𝑥 > 21|𝑥 > 18) = 4/7$)

3. Al estudiar bajas cotizaciones para contratos de embarques, una empresa fabricante de microcomputadoras encuentra que los contratos interestatales tienen bajas cotizaciones que están uniformemente distribuidas entre 20 y 25, en unidades de miles de dólares. Encuentre la probabilidad de que la baja cotización en el siguiente contrato interestatal:
   * Esté por debajo de 22000 (**Rta**: 2/5 = 0.4).
   * Sea de más de 24000 (**Rta**: 1/5 = 0.2).

4. El número de tarjetas de circuito defectuosas que salen de una máquina soldadora sigue una distribución de Poisson. Durante un día específi co de ocho horas, se encontró una tarjeta defectuosa.
   * Encuentre la probabilidad de que haya sido producida durante la primera hora de operación durante ese día. (**Rta**: 1/8).
   * Encuentre la probabilidad de que haya sido producida durante la última hora de operación durante ese día. (**Rta**: 1/8).
   * Dado que no se produjeron tarjetas defectuosas durante las primeras cuatro horas de operación, encuentre la probabilidad de que la tarjeta defectuosa se fabricara durante la quinta hora. (**Rta**: 1/4).

5. Al usar el método de triangulación para determinar el alcance de una sonda acústica, el equipo de prueba debe medir con precisión el tiempo que tarda en llegar el frente de onda esférica a un sensor de recepción. De acuerdo con Perruzzi y Hilliard (1984), los errores de medición se pueden modelar como si tuvieran una distribución uniforme de $-0.02\mu$ a $0.05\mu$. 
   * ¿Cuál es la probabilidad de que una medición particular de tiempo de llegada sea precisa con tolerancia de no más de $0.01 \mu s$? (**Rta**: 2/7)
   * Encuentre la media y varianza de los errores de medición. (**Rta**: $\mu = 0.015$; $V(Y) = 0.00041$)

### Distribución exponencial

1. Los datos recogidos en el Aeropuerto Internacional Toronto Pearson sugiere que una distribución exponencial con valor medio de 2.725 horas es un buen modelo para la duración de la lluvia (Urban Stormwater Management Planning with Analytical Probabilistic Models, 2000, p. 69).
   * ¿Cuál es la probabilidad de que la duración de un evento de lluvia en este lugar particular, sea por lo menos 2 horas? ¿A lo más 3 horas? ¿Entre 2 y 3 horas? (**Rta**: 0.480, 0.667, 0.147)
   * ¿Cuál es la probabilidad de que la duración de la lluvia supere el valor medio por más de dos desviaciones estándar? ¿Cuál es la probabilidad de que sea menor que el valor medio en más de una desviación estándar? (**Rta**: 0.050, 0)

2. Sea ***X*** la distancia (m) que un animal recorre desde el sitio de su nacimiento hasta el primer territorio vacante que encuentra. Suponga que para ratas canguro con etiqueta en la cola, ***X*** tiene una distribución exponencial con parámetro $\lambda=0.1386$ (como lo sugiere el artículo "Competition and Dispersal from Multiple Nests", Ecology, 1997: 873–883).
   * ¿Cuál es la probabilidad de que la distancia sea cuando mucho de 100 m? ¿Cuando mucho de 200 m? ¿Entre 100 y 200 m? (**Rta**: 0.7499, 0.9375, 0.1876)
   * ¿Cuál es la probabilidad de que la distancia exceda la distancia media por más de 2 desviaciones estándar? (**Rta**: 0.0498)
   * ¿Cuál es el valor de la distancia mediana? (**Rta**: 50.01m)
  
3. En estudios de medicamentos contra el cáncer se encontró que si a los ratones se les inyectan células cancerosas, el tiempo de supervivencia se puede modelar con la distribución exponencial. Sin tratamiento el tiempo de supervivencia esperado fue de 10 h.
   * ¿Cuál es la probabilidad de que un raton seleccionado aleatoriamente sobreviva al menos 8 h?, ¿a lo sumo 12 h?, ¿entre 8 y 12 h? (**Rta**: 0.4493, 0.6988, 0.1481)
   * ¿Cuál es la probabilidad de que el tiempo de supervivencia de un ratón excede el valor medio en más de 2 desviaciones estándar? ¿Más de 3 desviaciones estándar? (**Rta**: 0.0498, 0.0183)
  
4. Sea ***X = el tiempo entre dos llegadas sucesivas a la ventanilla de una sede bancaria***. Si X tiene una distribución exponencial con $\lambda = 1$
   * El tiempo esperado entre dos llegadas sucesivas (**Rta**: 1)
   * La desviación estandar del tiempo entre dos llegadas sucesivas (**Rta**: 1)
   * $P(X \leq 4)$ (**Rta**: 0.982)
   * $P(2 \leq X \leq 5)$ (**Rta**: 0.129)

5. El operador de una estación de bombeo ha observado que la demanda de agua durante las primeras horas de la tarde tiene una distribución aproximadamente exponencial con media de 100 pcs (pies cúbicos por segundo).
   * Encuentre la probabilidad de que la demanda sea mayor que 200 pcs durante las primeras horas de la tarde en un día seleccionado al azar. (**Rta**: 0.1353).
   * ¿Qué capacidad de bombeo de agua debe mantener la estación durante las primeras horas de la tarde para que la probabilidad de que la demanda sea mayor que la capacidad en un día seleccionado al azar sea de sólo 0.01? (**Rta**: 460.52 pcs).

### Distribución normal

1. Un experimentador publicó en la revista **Annals of Botany** un articulo en el que investigó si los diámetros de tallos del girasol dicotiledónea cambiarían, dependiendo de si la planta fue dejada para balancearse libremente en el viento o estaba artificialmente sostenida. Suponga que los diámetros de tallos no soportados en la base, de una especie particular de girasol, tienen una distribución normal con
un diámetro promedio de 35 milímetros (mm) y una
desviación estándar de 3 mm.
   * ¿Cuál es la probabilidad de que una planta de girasol tenga un diámetro de base de más de 40 mm? (**Rta**: 0.0477)
   * Si dos plantas de girasol se seleccionan al azar, ¿cuál es la probabilidad de que ambas plantas tengan un diámetro de base de más de 40 mm? (**Rta**: 0.00228)
   * ¿Dentro de qué límites esperaría usted que se encuentren los diámetros de base, con probabilidad .95? (**Rta**: 29.12 a 40.88)
   * ¿Qué diámetro representa el 90avo percentil de la distribución de diámetros? (**Rta**: 38.84)

2. Suponga que el diámetro a la altura del pecho (pulg) de árboles de un tipo está normalmente distribuido con $\mu=8.8$ y $\sigma=2.8$, como se sugiere en el artículo "Simulating a Harvester-Forwarder Softwood Thinning" (*Forest Products J.*, mayo de 1997; 36–41).
   * ¿Cuál es la probabilidad de que el diámetro de un árbol seleccionado al azar será por lo menos de 10 pulg? ¿Y que exceda de 10 pulg? (**Rta**: 0.334)
   * ¿Cuál es la probabilidad de que el diámetro de un árbol seleccionado al azar sea de más de 20 pulg? (**Rta**: Aproximadamente 0)
   * ¿Cuál es la probabilidad de que el diámetro de un árbol seleccionado al azar sea de entre 5 y 10 pulg? (**Rta**: 0.5795)
   * ¿Qué valor c es tal que el intervalo $(8.8 – c, 8.8 + c)$ incluya $98\%$ de todos los valores de diámetro? (**Rta**: 6.524)

3. Suponga que la concentración de cloruro en sangre (mmol/L) tiene una distribución normal con media de 104 y desviación estándar de 5 (información en el artículo **Mathematical Model
of Chloride Concentration in Human Blood**, *J. of Med. Engr. and Tech.*, 2006; 25–30).
   * ¿Cuál es la probabilidad de que la concentración de cloruro sea igual a 105? ¿Sea menor que 105? ¿Sea cuando mucho de 105? (**Rta**: 0, 0.5793, 0.5793)
   * ¿Cuál es la probabilidad de que la concentración de cloruro difiera de la media por más de 1 desviación estándar? ¿Depende esta probabilidad de los valores de $\mu$ y $\sigma$? (**Rta**: 0.3174, No)
   * ¿Cómo caracterizaría el .1% más extremo de los valores de concentración de cloruro? (**Rta**: Menores a 88.55 y mayores a 119.45)

4. Considere los bebés nacidos dentro del rango "normal" de gestación de 37 a 43 semanas. Numerosos datos respaldan la suposición de que para tales bebés (nacidos en los Estados Unidos) el peso al nacer tiene una distribución normal con una media de 3432 g y una desviación estándar de 482 g ("Are Babies Normal?" The American Statistician [1999]: 298–302).
   * ¿Cuál es la probabilidad de el peso de un bebe, seleccionado al azar:
     * al nacer exceda los 4000 g (**Rta**: 0.119)
     * Se encuentre entre entre 3000 y 4000 g (**Rta**: 0.696)
   * Cuál es la probabilidad de que el peso al nacer de un bebé, seleccionado al azar, sea menor de 2000 g o mayor de 5000 g (**Rta**: 0.0020)
   * ¿Cuál es la probabilidad de que el peso de un bebe seleccionado al azar exceda las 7 lb? (**Pista**: 1 libra = 453.59 g) (**Rta**: 0.702)
   * ¿Cómo caracterizaría al 0,1% más extremo de todos los pesos al nacer? (**Rta**: Los pesos menores que 1836 g o los pesos mayores que 5018 g)

5. Suponga que la distribución de la tasa de digitado neta en palabras por minuto (ppm) para mecanógrafos experimentados se puede aproximar mediante una curva normal con una media de 60 ppm y una desviación estándar de 15 ppm ("Effects of Age and Skill in Typing", Journal of Experimental Psychology [Effects of Age and Skill in Typing], Journal of Experimental Psychology [ 1984]: 345–371).
   * Cuál es la probabilidad de que la velocidad neta de un mecanógrafo seleccionado al azar:
     * Sea como máximo de 60 palabras por minuto. (**Rta**: 0.5)
     * Al menos de 60 palabras por minuto. (**Rta**: 0.5)
   * ¿Cuál es la probabilidad de que la tasa neta de un mecanógrafo seleccionado al azar esté entre 45 y 90 palabras por minuto? (**Rta**: 0.8185)
   * ¿Le sorprendería encontrar un mecanógrafo en esta población cuya velocidad neta supere las 105 palabras por minuto? (**Nota**: la mayor velocidad neta en una muestra descrita en el articulo es de 104 palabras por minuto). (**Rta**: Si, describa el porque)
   * Suponga que se seleccionan dos mecanógrafos de forma independiente. ¿Cuál es la probabilidad de que la tasa de mecanografía de ambos supere las 75 palabras por minuto? (**Rta**: 0.0252)
   * Suponga que se va a poner a disposición del 20% más lento de los mecanógrafos una capacitación especial. ¿Qué velocidades de escritura calificarían a las personas para esta capacitación? (**Rta**: Aquellas menores a 47.4)