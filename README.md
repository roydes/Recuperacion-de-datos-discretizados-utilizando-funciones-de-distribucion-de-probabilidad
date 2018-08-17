# Planteamiento del Problema

<div style="text-align: justify">
Diseñar un algoritmo que logre recuperar los datos que han sido discretizados de un conjunto determinado de datos independientemente del método de discretización utilizado.
<div/>
<br/>
    <h2>Propuesta de Solución</h2>
<div style="text-align: justify">
La distribución de probabilidad de una variable aleatoria es una función que realciona a cada suceso definido sobre la variable aleatoria la probabilidad de que dicho suceso se observe. La distribución de probabilidad se define sobre el conjunto de todos los sucesos y cada uno de los sucesos es el rango de valores de la variable aleatoria. La función de probabilidad está asociada a las distribuciones de frecuencia de un conjunto de datos. Ya que una función de distribución de probabilidades no es más que una frecuencia teórica, siendo ésta última la que describe cómo se espera que varíen los resultados.
<br/>
Se definirán primero los conpectos de Variable Aleatoria, Espacio de probabilidad y de Función de Distribución de Probabilidad.
<br/>
Una variable aleatoria ${\displaystyle X}$ es una función real definida en el espacio de probabilidad, ${\displaystyle (\Omega ,{\mathcal {A}},P)}$ asociado a un experimento aleatorio. Donde ${\displaystyle \Omega }$  es llamado espacio muestral, conjunto de los posibles resultados del experimento, llamados sucesos elementales. Segundo, por la colección ${\displaystyle {\mathcal {B}}} $ de todos los sucesos aleatorios (no solo los elementales), o resultados que se pueden dar en el experimento aleatorio.Por último, una medida de probabilidad o función de probabilidad ${\displaystyle P\ } $, que asigna una probabilidad a todo suceso.
La función de Distribuciónde Probabilidad entonces se define como: 
$F(x)=\operatorname {P}(X\leq x)$,	Una función de nombre "F" le asigna a cada valor real $x$, el de la probabilidad de que una variable aleatoria $X$ asuma un valor inferior o igual a $x$.
Luego la probabilidad de que X se sitúe en un intervalo $]a, b]$(abierto en a y cerrado en b) es $F(b) − F(a)$ si $a ≤ b$ se define como:

${\displaystyle \mathbb {P} (a\leq X \leq b) =F_{X}(b)-F_{X}(a)} $
<br/>
<h2>Algoritmo Propuesto</h2>
<br/>
El algoritmo propuesto utiliza la función de probabilidad de los datos para así conocer la posiblidad de que cierto dato apareca en el conjunto de datos. Ya que se conoce el tamaño del conjunto se puede generar el dato cuantas veces ha sido observado en conjunto original antes de ser discretizados. El algoritmo realiza los siguientes pasos:
<ol>
<li>Estimar la Función distribución de probabilidad normalizada para un determinado número de beans (intervalos)</li>
<li>A partir de la probabilidad asignada a cada beans generar $P*N$ valores mediante una distribución normal, donde $P$ es la probabilidad del intervalo y $N$ es la cantidad de elementos del conjunto de datos</li>
<ol/>
<div/>
