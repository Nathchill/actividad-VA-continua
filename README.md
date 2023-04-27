# Variable aleatoria discreta

## Actividad

Teniendo en cuenta lo información dada en la siguiente tabla:

| Tema  | Juan Diego Taborda | Juan Camilo Quiroga | Samuel Toro| Santiago Ramirez| Julian Hernandez|
| ---  | ----| --- | --- | --- | --- |
| **VA continuas**  | 2 | 5 | 1 | 4 | 3 |
| **Uniforme**  | 5 | 4 | 3 | 2 | 1 |
| **Exponencial**  | 3 | 1 | 2 | 5 | 4 |
| **Normal**  |  |  |  |  |  |

Resuelva cada uno de los problemas claramente a **mano** (tal y como se vio en clase) y usando **python**. Los problemas resueltos a mano deberan ser entregados en clase en hojas mostrando la solución de manera clara, ordenada y bien explicada. Las notebooks de python (archivos con extención **ipynb**) que implementan la solución de los problemas que se la asigno, deberan ser subidos a este repositorio en una carpeta con las iniciales del autor y dentro de esta con los nombres de los archivos siguiendo el siguiente formato de acuerdo a la distribución que se toco y el numero que se le asigno:

|Distribución|Nombre|
|---|---|
|Uniforme|**```uni_#.ipybn```**|
|Exponencial|**```exp_#.ipybn```**|
|normal|**```normal_#.ipybn```**|

sss
|Distribución|Ejercicio Asignado|Nombre|
|---|---|---|
|Binomial|2|**```bin_2.ipybn```**|
|Geometrica|5|**```geom_5.ipybn```**|
|Hipergeometrica|4|**```hiper_4.ipybn```**|
|Poisson|1|**```poisson_1.ipybn```**|

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


<!--

1. Se construye un complejo sistema electrónico con cierto número de piezas de respaldo en sus subsistemas. Un subsistema tiene cuatro componentes idénticos, cada uno con una probabilidad de 0.2 de fallar en menos de 1000 horas. El subsistema funciona si dos de los cuatro componentes están operando. Suponga que los componentes operan de manera independiente. Encuentre la probabilidad de que
   <ol style="list-style-type: lower-alpha">
   <li>Exactamente dos de los cuatro componentes dure más de 1000 horas. (<b>Rta</b>: 0.1536) </li>
   <li>El subsistema opere más de 1000 horas. (<b>Rta</b>: 0.9728)</li>
   </ol>


2. El sistema de seguridad de una casa está diseñado para tener un 99% de confiabilidad. Suponga que nueve casas equipadas con este sistema experimentan un intento de robo. Encuentre las probabilidades de estos eventos:
   <ol style="list-style-type: lower-alpha">
   <li>Al menos una de las alarmas se activó. (<b>Rta</b>: 1) </li>
   <li>Más de siete de las alarmas se activaron  (<b>Rta</b>: 0.997)</li>
   <li>Ocho o menos alarmas se activaron   (<b>Rta</b>: 0.086)</li>
   </ol>

3. Muchas empresas que generan energía eléctrica promueven el ahorro de energía, para lo cual ofrecen tarifas de descuento a consumidores que mantengan su uso por debajo de ciertos estándares establecidos de subsidio. Un reciente informe de la EPA (agencia de protección ambiental) observa que 70% de los residentes en Puerto Rico han reducido su consumo de electricidad lo suficiente para tener derecho a tarifas de descuento. Si se seleccionan al azar cinco suscriptores residenciales de San Juan, Puerto Rico, encuentre la probabilidad de cada uno de los siguientes eventos:
   <ol style="list-style-type: lower-alpha">
   <li>Los cinco tienen derecho a las tarifas favorables. (<b>Rta</b>: 0.1681) </li>
   <li>Al menos cuatro tienen derecho a tarifas favorables.  (<b>Rta</b>: 0.5282)</li>
   </ol>

4. Problema Unos registros muestran que 30% de todos los pacientes ingresados en una clínica médica no pagan sus cuentas y que, en última instancia, esas cuentas son olvidadas. Suponga que n = 4 nuevos pacientes representan una selección aleatoria de entre un gran conjunto de prospectos de pacientes atendidos por la clínica. Encuentre estas probabilidades::
   <ol style="list-style-type: lower-alpha">
   <li>Las cuentas de todos los pacientes tendrán finalmente que olvidarse. (<b>Rta:</b> 0.0081) </li>
   <li>Una tendrá que olvidarse. (<b>Rta</b>: 0.4416)</li>
   <li>Ninguna tendrá que olvidarse.(<b>Rta</b>: 0.2401)</li>
   </ol>

5. Un estudiante que está tratando de escribir un ensayo para un curso tiene la opción de dos temas, A y B. Si selecciona el tema A, el estudiante pedirá dos libros mediante préstamo interbiblioteca, mientras que, si selecciona el tema B, el estudiante pedirá cuatro libros. El estudiante cree que un buen ensayo necesita recibir y utilizar por lo menos la mitad de los libros pedidos para uno u otro tema seleccionado. Si la probabilidad de que un libro pedido mediante préstamo interbiblioteca llegue a tiempo es de .9 y los libros llegan independientemente uno de otro
   <ol style="list-style-type: lower-alpha">
   <li>¿Qué tema deberá seleccionar el estudiante para incrementar al máximo la probabilidad de escribir un buen ensayo? (<b>Rta</b>: 0.0081) </li>
   <li>¿Qué pasa si la probabilidad de que lleguen los libros es de sólo 0.5 en lugar de 0.9? (<b>Tema A</b>: 0.99; <b>Tema B</b>: 0.9963)</li>
   <li>Ninguna tendrá que olvidarse.(<b>Tema A</b>: 0.75; <b>Tema B</b>: 0.6875)</li>
   </ol>

### Distribución de probabilidad Geometrica

1. Suponga que la probabilidad de mal funcionamiento de un motor durante cualquier periodo de una hora es p = 0.02. Encuentre la probabilidad de que un motor determinado funcione bien dos horas. (**Rta**: 0.9604)
   
2. Un contador público certificado (CPA, por sus siglas en inglés) ha encontrado que nueve de cada diez compañías auditadas contienen errores importantes. Si el CPA hace auditoría a una serie de cuentas de empresas
   <ol style="list-style-type: lower-alpha">
   <li>¿Cuál es la probabilidad de que la primera cuenta que contenga errores importantes sea la tercera en ser auditada?. (<b>Rta</b>: 0.009) </li>
   <li>¿Cuál es la probabilidad de que la primera cuenta que contenga errores importantes cualquier cuenta después de la segunda? (<b>Rta</b>: 0.01)</li>
   </ol>

3. La probabilidad de que llegue un cliente al mostrador de servicio de una tienda en un segundo cualquiera es igual a 0.1. Suponga que llegan clientes en forma aleatoria y por tanto que una llegada en un segundo cualquiera es independiente de las otras. Encuentre la probabilidad de que la primera llegada:
   <ol style="list-style-type: lower-alpha">
   <li>Ocurra durante el tercer intervalo de un segundo. (<b>Rta</b>: 0.081) </li>
   <li>No ocurra hasta al menos el tercer intervalo de un segundo. (<b>Rta</b>: 0.81)</li>
   </ol>
   
4. Una empresa de exploración petrolera va a hacer una serie de perforaciones de sondeo en una zona determinada en busca de un pozo productivo. La probabilidad de que tenga éxito en un intento dado es 0.2.
   <ol style="list-style-type: lower-alpha">
   <li>¿Cuál es la probabilidad de que la tercera perforación sea la primera en dar un pozo productivo? (<b>Rta</b>: 0.128) </li>
   <li>Si la empresa puede darse el lujo de perforar a lo sumo diez pozos, ¿cuál es la probabilidad de que no encuentre un pozo productivo? (<b>Rta</b>: 0.107)</li>
   </ol>

5. Suponga que 30% de los solicitantes para cierto trabajo industrial posee capacitación avanzada en programación computacional. Los candidatos son elegidos aleatoriamente entre la población y entrevistados en forma sucesiva. 
   <ol style="list-style-type: lower-alpha">
   <li>Encuentre la probabilidad de que el primer solicitante con capacitación avanzada en programación se encuentre en la quinta entrevista. (<b>Rta</b>: 0.07203) </li>
   <li>¿Cuál es el número esperado de solicitantes que será necesario entrevistar para hallar el primero con capacitación avanzada? (<b>Rta</b>: 3.33)</li>
   </ol>
   
### Distribución de probabilidad Hipergeometrica

1. En el sur de California, un creciente número de personas que buscan una credencial para enseñanza están escogiendo internados pagados en los tradicionales programas estudiantiles para enseñanza. Un grupo de ocho candidatos para tres posiciones locales de enseñanza estaba formado por cinco candidatos, que se habían inscrito en internados pagados y tres candidatos que se habían inscrito en programas tradicionales estudiantiles para enseñanza. Supongamos que los ocho candidatos están igualmente calificados para las posiciones. Represente con x el número de candidatos capacitados en un internado que son contratados para estas tres posiciones.
   <ol style="list-style-type: lower-alpha">
   <li>Encuentre la probabilidad de que tres candidatos capacitados en internado sean contratados para estas posiciones. (<b>Rta</b>: 0.1786) </li>
   <li>¿Cuál es la probabilidad de que ninguno de los tres contratados sea capacitado en internado? (<b>Rta</b>: 0.01786)</li>
   <li>Encuentre P(X >= 1) (<b>Rta</b>: 0.2857)</li>
   </ol>

2. Es frecuente que las semillas sean tratadas con fungicidas para protegerlas en ambientes húmedos y con desecación defectuosa. Un intento a pequeña escala, que comprende cinco semillas tratadas y cinco no tratadas, fue realizado antes de un experimento a gran escala para explorar cuánto fungicida aplicar. Las semillas se plantaron en un suelo húmedo y se contó el número de plantas que brotaron. Si la solución no era efectiva y cuatro plantas brotaron en realidad, cuál es la probabilidad de que:
   <ol style="list-style-type: lower-alpha">
   <li>Las cuatro plantas brotaran de semillas tratadas. (<b>Rta</b>: 0.0238) </li>
   <li>Tres o menos brotaran de semillas tratadas. (<b>Rta</b>: 0.9762)</li>
   <li>Al menos una brotara de semillas no tratadas (<b>Rta:</b>: 0.9762)</li>
   </ol>

3. Un producto industrial se envía en lotes de 20. Es costoso realizar pruebas para determinar si un artículo es defectuoso y, por tanto, el fabricante muestrea su producción en lugar de usar un plan de inspección al 100%. Un plan de muestreo, construido para minimizar el número de piezas defectuosas enviadas a los clientes, exige muestrear cinco artículos de cada lote y rechazar el lote si se observa más de una pieza defectuosa. (Si el lote es rechazado, cada artículo del mismo se prueba posteriormente.) Si un lote contiene cuatro piezas defectuosas: 
   <ol style="list-style-type: lower-alpha">
   <li>¿cuál es la probabilidad de que sea rechazado?  (<b>Rta</b>: 0.2487) </li>
   <li>¿Cuál es el número esperado de piezas defectuosas en la muestra de tamaño 5? (<b>Rta</b>: 1)</li>
   <li>¿Cuál es la varianza del número de piezas defectuosas de la muestra de tamaño 5? (<b>Rta</b>: 0.632)</li>
   </ol>

4. Se capturaron, etiquetaron y liberaron cinco individuos de una población de animales que se piensa están al borde la extinción en una región para que se mezclen con la población. Después de haber tenido la oportunidad de mezclarse, se selecciona una muestra aleatoria de 10 de estos animales. Sea **X = el número de animales etiquetados en la segunda muestra**. Si en realidad hay 25 animales de este tipo en la región, ¿cuál es la probabilidad de que:
   <ol style="list-style-type: lower-alpha">
   <li>El numero de animales etiquetados en la segunda muestra sea de dos(<b>Rta</b>: 0.385) </li>
   <li>El numero de animales etiquetados en la segunda muestra no supere los dos (<b>Rta</b>: 0.699)</li>
   <li>Calcule la media y la varianza del problrma (<b>Media</b>: 2.0; <b>Varianza</b>: 1.0)</li>
   </ol>

5. Una corporación está muestreando sin reemplazo para n = 3 firmas para determinar aquella de la cual comprar ciertos abastecimientos. La muestra se ha de seleccionar de un grupo de seis fi rmas, de las cuales cuatro son locales y dos no. Denote con Y el número de fi rmas no locales de entre las tres seleccionadas.
   <ol style="list-style-type: lower-alpha">
   <li>P(Y = 1) (<b>Rta</b>: 0.6) </li>
   <li>P(Y >= 1) (<b>Rta</b>: 0.8)</li>
   <li>P(Y <= 1) (<b>Rta</b>: 0.8)</li>
   </ol>

### Distribución de probabilidad de Poisson

1. El número de errores mecanográficos hechos por una secretaria tiene una distribución de Poisson con
un promedio de cuatro errores por página. Si en una página se dan más de cuatro errores, la secretaria
debe volver a escribir toda la página. ¿Cuál es la probabilidad de que una página seleccionada al azar no
tenga que volver a ser escrita? (**Rta**: 0.6288)

2. El número promedio de accidentes de tránsito en cierto crucero de carretera es dos por semana. Suponga que el número de accidentes sigue una distribución de Poisson con $\lambda = 2$
   <ol style="list-style-type: lower-alpha">
   <li>Encuentre la probabilidad de que no haya accidentes en este crucero de carretera durante un periodo de 1 semana. (<b>Rta</b>: 0.135335) </li>
   <li>Encuentre la probabilidad de que haya tres accidentes como máximo en esta sección de carretera durante un periodo de 2 semanas. (<b>Rta</b>: 0.433471)</li>
   </ol>

3. El incremento del número de vuelos regionales cortos en aeropuertos importantes ha aumentado la preocupación por la seguridad en el aire. Un aeropuerto de la región este ha registrado un promedio mensual de cinco accidentes a punto de ocurrir en aterrizajes y despegues en los últimos 5 años.
   <ol style="list-style-type: lower-alpha">
   <li>Encuentre la probabilidad de que durante un mes determinado no haya accidentes a punto de ocurrir en aterrizajes y despegues en el aeropuerto. (<b>Rta</b>: 0.0067) </li>
   <li>Encuentre la probabilidad de que durante un mes determinado haya cinco accidentes a punto de ocurrir. (<b>Rta</b>: 0.1755)</li>
   <li>Encuentre la probabilidad de que haya al menos cinco accidentes a punto de ocurrir durante un mes particular. (<b>Rta</b>: 0.560)</li>
   </ol>

4. De acuerdo con un estudio realizado por el Departamento de Pediatría de la Universidad de California, en San Francisco, los niños que se lesionan dos o más veces tienden a sufrir estas lesiones durante un tiempo relativamente limitado, por lo general un año o menos. Si el número promedio de lesiones por año para niños en edad escolar es de dos, ¿cuáles son las probabilidades de estos eventos?
   <ol style="list-style-type: lower-alpha">
   <li>Un niño en edad escolar sufrirá dos lesiones durante el año. (<b>Rta</b>: 0.271) </li>
   <li>Un niño en edad escolar sufrirá dos o más lesiones durante el año. (<b>Rta</b>: 0.594)</li>
   <li>Un niño en edad escolar sufrirá a lo sumo una lesión durante el año. (<b>Rta</b>: 0.406)</li>
   </ol>

5. El número de solicitudes de ayuda recibidas por un servicio de grúas es un proceso de Poisson con razón cuatro por hora.
   <ol style="list-style-type: lower-alpha">
   <li>Calcule la probabilidad de que exactamente diez solicitudes sean recibidas durante un periodo particular de 2 horas. (<b>Rta</b>: 0.099) </li>
   <li>Si los operadores del servicio de grúas hacen una pausa de 30 minutos para el almuerzo, ¿cuál es la probabilidad de que no dejen de atender llamadas de ayuda? (<b>Rta</b>: 0.135)</li>
   <li>¿Cuántas llamadas esperaría durante esta pausa? (<b>Rta</b>: 2)</li>
   </ol>

-->