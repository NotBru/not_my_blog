Baye-a-saber
############

:date: 2021-08-22
:tags: probabilidad, filosofía, ciencia, epistemología
:category: Filosociencia
:author: Bru
:slug: baye-a-saber
:lang: ñl

Este post está basado en los primeros dos capítulos del libro `Probability Theory: The Logic of Science <https://bayes.wustl.edu/etj/prob/book.pdf>`_, de Edwin T. Jaynes. El primero detalla los conceptos, y es sumamente accesible, por lo que se lo recomiendo a quien sea que le gusten los tópicos del post. El segundo tiene las cuentas, que tampoco vienen mal, pero es una lectura un poco menos accesible.

Si empezás a ver cuentas en este post y te asustás o no las entendés nada, probá **ignorarlas y seguír**. Los conceptos se deberían entender todos sin entender las cuentas en particular, sólo saber que “existe alguna cuenta para tal cosa”. En todo caso, podés irte a la sección final; ahí hay un microresumen de qué se hizo en las secciones anteriores, y un par de cuestionamientos donde expongo mi punto de vista.

============
Introducción
============

Son las hace-tres-millones-de-años de la tarde. Te vas poniendo tu animal print 0% vegano porque pegó un chucho de la san mamut, y te juntás con Ugnorr a charlar de aquella vez que la muchachada encontró un `laser raptor <https://www.youtube.com/watch?v=bS5P_LAqiVg>`_ suelto o qué se yo. Acá no hay ningún paleontólogo leyendo, ¿no?

Mirás al horizonte y notás que el sol, que venía estando todo pipón hace rato, está cada vez más rojo y se mete cada vez más abajo en el horizonte. “Ah, la cachucha” decís... Se nos fue. “Aparecerá de nuevo”, pregunta Ugnorr, un poco preocupada. “Y, no sé, habrá que ver”, tirás.

Es en ese momento que el Bayergh, que justo andaba persiguiendo un mamut por ahí cerca o eso o algo, escucha de querusa y se prende a la conversación. Se para y dice, “Nah bro. Pero seguro viene otro. Mi grado de seguridad es el logaritmo de la cantidad de días que sigo vivo. ¿Kíííh?¿Qué pasó acá?

=====================
Deducción e inducción
=====================
Sí, ya sé cuál es tu problema con el escenario anterior: ¡La inescrupulosa afirmación de Bayergh no tiene fundamentos inquebrantables! Después de todo, yo conozco un planeta donde una vez el sol se puso, y no salió nunca más...

La `disyuntiva epistemológica <https://www.youtube.com/watch?v=p9ZdeARKTzE>`_ que aquí nos concierne es que nadie en esta conversación ha demostrado la afirmación que se estaba tomando por cierta. ¿Cómo demostrás que el sol va a salir todos los días? Hoy día no sólo poseemos abundante evidencia de que estamos parados en una roca orbitando una aglomeración gigante de átomos de hidrógeno que hacen pogo, y potencialmente un tazón de petuñas. Sabemos además que el sol es una estrella tipo enana amarilla, y de nuestro entendimiento observando otras estrellas sabemos cuánto va a durar ahí, etc...

Y aún así, nada te dice que qué se yo, no vaya a venir un `agujero negro salvaje <https://futurism.com/theres-a-rogue-black-hole-streaking-through-the-universe>`_ que vaya a ponerle fin a `Friedrick, Cesil y sus amigues, y todo lo que es bueno en esta vida <https://www.youtube.com/watch?v=jxepnIG1yQQ>`_. Hilando fino, no podemos tener una certeza absoluta al respecto. Y sin embargo, entendemos que el sol va a salir mañana con “casi certeza”. Nadie está particularmente dubitativo al respecto. Seguro, el sol capaz deja de salir algún día, pero eso sorprendería a todos.

Esto es lo que pasa más frecuentemente dentro de la ciencia, y también dentro de la vida cotidiana. La información a nuestro alcance nos permite declarar conclusiones *probables*, pero no *deducibles*. Si salgo afuera y las nubes están re negras, y hay un qué se yo en los huesos, es *probable* que llueva, pero no es una realidad inevitable. Si no llueve, no nos sorprendería demasiado nuestra equivocación.

A esa clase de razonamiento se le llama razonamiento inductivo, y contrasta con el razonamiento deductivo, donde de las premisas se derivan consecuencias ineludibles. Como ejemplo de este otro tipo de razonamiento tenemos el siguiente `silogismo <https://es.wikipedia.org/wiki/Silogismo>`_: “Todos los hombres son mortales. Sócrates es hombre. Por lo tanto, Sócrates es mortal.”. Es evidente que es un razonamiento deductivo porque la falsedad de la conclusión, o sea, que Sócrates no fuera mortal, es inadmisible bajo las premisas. Si Sócrates fuera inmortal, o hay hombres que no son mortales, o Sócrates no es un hombre.

Todos los razonamientos deductivos, en el fondo, toman la forma de los silogismos “**A** implica **B**. **A** es cierto. Por lo tanto, **B** es cierto” y “**A** implica **B**. **B** no es cierto. Por lo tanto, **A** no es cierto”. Aquí, **A** y **B** representan proposiciones lógicas, como “Llueve a las 16” y “Hay nubes negras a las 15:45”. En las circunstancias donde podemos aplicarlos son sumamente poderosos, ya que nos dan certeza absoluta, y podemos utilizar estas certezas a nuestra ventaja a la hora de decidir qué hacer. Por tal motivo, se los llama “silogismos fuertes”.

Los silogismos recíprocos a los anteriores, en contraste, son directamente inválidos. Por ejemplo, uno no puede decir “**A** implica **B**. **A** no es cierto. Por lo tanto, **B** no es cierto.” Sin embargo, en la vida real, una versión debilitada de este silogismo resulta sumamente útil. Por ejemplo, que llueva implica que el pasto se moja. Si no llueve, uno se ve inclinado a decir que el pasto no va a estar mojado. Sin embargo, esto no es lógicamente deducible, ya que existen factores alternativos que podrían mojarlo. Sin embargo, afirmar que no se puede decir nada sobre el pasto, sería menospreciar la información que saber que no llovió aporta.

============================================================
Las formas simbólicas del razonamiento deductivo e inductivo
============================================================
“Uuuh, ¿qué mierda quiso decir este flaco con este título?”.

Supongo que todos estamos de acuerdo con que es sumamente útil plasmar ideas en símbolos. Este mismo post lo atestigua. Podemos, por ejemplo, usar el Español para enunciar nuestros argumentos, como hacen los `sesgados a sueldo <https://dle.rae.es/abogado>`_. Los lenguajes naturales tienen propiedades muy copadas, como que podés enunciar ideas súmamente complejas, actuando como medio para transferir esos conceptos entre cosas pensantes. Proveen una expresividad amplia, que nos permite hacer poesía, evocar emociones ajenas. Muy piola.

Pero con la amplitud de posibilidades que presentan, llegan desventajas. Por ejemplo, las oraciones pueden ser ambiguas. Las palabras mismas admiten más de una acepción. En ciertas situaciones esto puede llegar a ser ventajoso, ya que nos permite razonar sobre problemas de maneras quizás más creativas, o más vagamente definidas, que luego pueden especializarse hacia argumentos más definidos. Pero también, por ejemplo, nos deja servidos recursos de mierda, como `malinterpretar al interlocutor <https://es.wikipedia.org/wiki/Falacia_del_hombre_de_paja>`_, que sea intencional o inintencional, es siempre dañino y dificulta el intercambio de ideas.

Pero cuando uno está interesado en exponer un argumento, uno puede prescindir de ciertas facilidades de los lenguajes naturales Esto permite construír formas de manejo de símbolos más limitadas, con varias ventajas. Por un lado, es mucho más robusto: podemos evitar malentendidos, podemos también evidenciar la formación de oraciones paradójicas. Por otro, hace más fácil la verificación de la validez de las proposiciones enunciadas en dicho lenguaje.

Manejando afirmaciones binarias
-------------------------------

En alguna afirmación allá arriba yo hablé de proposiciones lógicas **A** y **B**, y enuncié los silogismos fuertes. Resulta super útil poder *operar* con dichas afirmaciones, de forma simbólica. Por ejemplo, la frase “**A** y **B** son simultáneamente ciertas” es una proposición lógica en su justo derecho. La frase “**A** es cierto implica que **B** es cierto**” representa una relación entre estas proposiciones que también nos es de utilidad. Suponiendo entonces que podamos definir de alguna u otra manera dichas proposiciones lógicas, nos interesa tratarlas como cositas matemáticas que operen entre sí.

Esas consideraciones nos llevan a la definición del álgebra de Boole. Además, a fin de escribir menos, introducimos una notación matemática, idéntica a las del álgebra convencional, para manipular las afirmaciones, de la siguiente forma:

- :math:`A` representa la proposición “**A** es cierta”.
- :math:`AB` representa la proposición “**A** y **B** son simultáneamente ciertas.
- :math:`A+B` representa la proposición “Al menos una de las proposiciones **A** y **B** es cierta”
- :math:`¬A` representa la proposición “**A** es falsa”

Y uno obtiene reglas super intuitivas, con las que puede hacer álgebra. Ponele, la afirmación “A es cierto y al menos uno de B o C es cierto” es equivalente a decir que “A y B es cierto, o A y C es cierto”, entonces te queda :math:`A(B+C)=AB+AC`. O “No es cierto que A y B son ciertos a la vez” es equivalente a “A no es cierto o B no es cierto”, y toma la forma :math:`¬(AB)=¬A+¬B`.

En fin. Esta notación nos da un conjunto de reglas, que deben ser aplicables sin importar qué afirmaciones elijo que mis letras representen. Y usando esas reglas podemos decir cosas lógicas. Por ejemplo, la afirmación “A implica B” la podemos pensar como “No pasa nunca que A sea cierto y B no”. Es decir, :math:`¬(A¬B)`. Como estas reglas reconstruyen los silogismos fuertes (creeme porque te lo demuestro eh), este resulta ser un lenguaje perfectamente válido para trabajar con esa clase de afirmaciones.

Manejando afirmaciones no binaries
----------------------------------

Este ya es un problema más complicado. ¿Qué quiero decir con afirmaciones *no binarias*? Recordemos que en la subsección anterior, las afirmaciones son o verdaderas o falsas. O llueve, o no llueve. En la vida raramente tenemos una certeza. `Perdí <https://es.wikipedia.org/wiki/El_Juego_(juego_mental)>`_.

Nuestro objetivo acá es cuantificar “grados de creencia”, o “grados de seguridad”. ¿El propósito? es que así tomamos decisiones. Además, imaginate que querés hacer una cosa (un programa, ponele) que trabaje bajo incertidumbre. Vas a necesitar que se maneje de alguna forma, manejando símbolos y eso.

Bueno, sin tanto preámbulo, eso es el punto de partida del libro en el que baso la mayoría del post. Lo que queremos es que :math:`A` ya no represente un valor binario, sino un espectro. Que algunos de esos valores representen “casi certeza”, otros “casi nada de certeza”, y cosas así. Y queremos que símbolos tipo :math:`AB` representen nuestro grado de convicción sobre la veracidad de “A y B son ciertos a la vez”. Y, del mismo modo que antes obtuvimos un álgebra que nos deja manipular esas cosas, obtener reglas aquí para manipular estas cosas.

Esas reglas no pueden ser cualquier cosa. Por ejemplo, si :math:`A` y :math:`B` son extremadamente inverosímiles por su cuenta, queremos que :math:`AB` lo sea también. Entre otros. Entonces, establecemos un conjunto de *desiderata* (cosas que queremos que cumplan nuestras reglas), y vemos si podemos obtener un marco matemático que las respete. Sin más preámbulo, la desiderata es:

* 1. Grados de plausibilidad son representados por números reales.
* 2. Correspondencia cualitativa con el sentido común
* 3. Consistencia

    - 3a. Si una conclusión puede ser razonada de más de una manera, entonces cada posible manera debe llevar al mismo resultado.
    - 3b. Siempre tomar en cuenta toda la evidencia que es relevante a una pregunta. No ignora arbitrariamente parte de la información, basando sus conclusiones sólo en lo que queda. En otras palabras, ser completamente no ideológico.
    - 3c. Siempre representar estados de conocimiento equivalentes con cuantificaciones de plausibilidad equivalentes. Eso es, si en dos problemas el estado de conocimiento es el mismo (aparte de quizás cambiar el nombre de proposiciones), entonces debe asignar las mismas plausibilidades en ambas.

Suena bastante razonable, ¿no cierto? El primero es casi obligatorio, porque queremos poder implementar este razonamiento de una manera abstracta. No queremos depender de cosas cualitativas como “muy mucho”, sino poder darle una forma definida. El segundo es menos subjetivo de lo que parece. El lector escéptico dirá, “ah, claro, ¿el sentido común de quién?”. En realidad Edwin usa ese término como un atajo en palabras. Te invito a realizar un escrutinio de cómo se usa, dentro del formalismo matemático, esta apelación al sentido común. Vas a ver que no hay ninguna ideología incorporada. Tal desideratum toma la forma de afirmaciones como “Si nueva evidencia hace a :math:`A` más probable, y deja intacto a :math:`B`, entonces :math:`AB` debe ser más probable”. El último es básicamente un requisito sobre nuestra lógica. Imaginate permitirte pensar de una forma profundamente contradictoria. Yo, en lo personal, no encuentro problema con ningún desideratum.

Luego sigue una demostración extensa que **ruego** lean o pispeen, de lo que se conoce como los teoremas de Cox (ejejej). Capítulo 1 y 2 del libro que ya mencioné. Pero al final del día, lo que se encuentra es que existe una *función* :math:`P` de nuestras asignaciones de plausibilidad :math:`A`, que satisface las siguientes cosas

.. :math:

   P(A)+P(¬A)=1,
   P(AB)=P(A)P(B|A)

No te asustes porque esa tal :math:`P` la usamos todo el tiempo en nuestro lenguaje. Es la *probabilidad*. Al número :math:`P(A)` es la probabilidad de que :math:`A` sea cierto. Las ecuaciones entonces se leen re fácil: la primera nos dice que la suma entre la probabilidad de que algo sea cierto y la de que sea falso tiene que sumar a 1; o sea, o uno o lo otro. La segunda incorpora un símbolo nuevo, :math:`B|A`, que representa la plausibilidad de que *B* sea cierto dado que *A* lo es. Entonces, esa expresión nos dice que la probabilidad de que *A* y *B* sean ciertos a la vez es el producto entre la probabilidad de que *A* sea cierto por la probabilidad de que *B* sea cierto **provisto** que *A* fuera cierto.

Lo loco es que de estas leyes se desprende toda la operatoria típica de la teoría de las probabilidades. Este resultado, que “a partir de la desiderata de representabilidad numérica, correspondencia cualitativa con el sentido común, y consistencia, se derivan tales restricciones numéricas”, nos indica algo fundamental: Cualquier persona que, en su asignación de probabilidades, violara cualquiera de las dos anteriores restricciones (o sus consecuencias), estaría necesariamente infringiendo algún desideratum. En otras palabras, hemos encontrado las leyes mínimas con las que regirnos para cuantificar plausibilidades.

===========
¿Y Bayergh?
===========

La segunda de las ecuaciones de allá arriba fueron usadas por Bayes y otra *pipol* para tomar conclusiones, sujeto a cierta información. Tomemos el ejemplo de la salida del sol mañana. ¿Qué probabilidad hay?

Bueno, depende. Si estuviéramos segures de que “Saldrá el sol mañana”, diríamos :math:`P(\text{“Saldrá el sol mañana”})=1`. Si estuviéramos convencides de lo contrario, pondríamos :math:`0` en cambio. De hecho, trabajar con probabilidades que son o 1 o 0 nos devuelve a la lógica deductiva. “A implica B” sería :math:`P(B|A)=1`, por ejemplo. Pero lo lindo es que podemos cuantificar conocimiento parcial ahora.

Imaginaremos entonces que Bayergh bebé, la primera vez que vio al sol ponerse, le atribuyó una probabilidad de 1/2 de que vuelva a salir. Esto básicamente significa que no le sorprendería ningún resultado, medio como que no sabe nada. En su abordaje bayesiano innato, cada vez que vea al sol salir, irá incrementando la probabilidad que le atribuye a la subsecuente salida del sol, hasta que esté bastante cerca de 1 y Bayergh se considere casi convencido de ello.

¿Cómo hace eso exactamente? Este es un modelo poco sofisticado, pero en primera instancia él puede suponer que cualquier salida del sol es equivalente a la anterior. Y que cada día nuevo, se tira un “dado sesgado” que va a definir si sale o no el sol. Pongámosle nombre: :math:`f=P(\text{“Salga el sol un día cualquiera”})` a la probabilidad esa de que salga el sol. En el transcurso de su vida, fue acumulando *evidencia* de que el sol iba a volver a salir. ¿Por qué? Porque sabe que todos los días de su vida salió el sol.

Cuentas salteables
------------------

En particular, nuestro Bayergh hizo la siguiente cuenta. Para él todos los días eran equivalentes, entonces le puso una probabilidad :math:`f` a que salga el sol cualquier día. Él vio al sol salir :math:`N` veces, y se preguntó, ¿cuál es la probabilidad de eso? Bueno, la probabilidad de que el sol salga dos días seguidos termina siendo el producto de las probabilidades para cada día, o sea, :math:`f^2`. La de que salga :math:`N` días seguidos será :math:`f^N`. Este es el *modelo* de Bayergh.

Entonces, si la probabilidad :math:`f` de que salga el sol fuera :math:`1/2`, y Bayergh vivió 10 años, tendríamos una probabilidad de :math:`1/2^3650`, que nos da... Cero, según Python. O sea, un número re re chiquitito. ¿Qué significa esto? Que la hipótesis esta en particular es inverosímil; no se condice con los datos. Bayergh entonces se golpea la cabeza un rato hasta que pienza... ¡Ajá! No necesito quedarme con la hipótesis :math:`f=1/2` en particular. Por cada valor distinto que le ponga a :math:`f` yo tengo una hipótesis distinta. Y yo quiero averiguar cuál hipótesis, o sea, qué valor de :math:`f`, se condice mejor con los datos. En otras palabras, si con :math:`D` represento mis datos, y con :math:`H` una hipótesis, *la probabilidad de la hipótesis :math:`H` dados los datos :math:`D` es lo que me interesa*.

En ese caso, el teorema de Baye...rgh dice,

.. :math:

   P(DH)=P(D)P(H|D)
   P(DH)=P(H)P(D|H)

Porque ni :math:`D` ni :math:`H` tiene un estatus privilegiado, puedo plantear dos igualdades distintas, invirtiendo sus roles. Y acá está lo lindo: yo ya sé calcular la probabilidad de los datos dada mi hipótesis, como hice arriba. O sea, tengo :math:`P(D|H)` y quiero :math:`P(H|D)`. Entonces, mezclando esas dos ecuaciones, obtengo

.. :math:

   P(H|D)=P(D|H)P(H)/P(D)

Lindo, ¿no? hay tres números a la derecha. :math:`P(D|H)` es el modelo, eso lo tenemos. Por una magia, :math:`P(D)` no es relevante; se puede deducir del requisito de que las probabilidades de todas las hipótesis posibles deben sumar a uno. Lo único que nos falta es :math:`P(H)`. ¿De donde la sacamos? Y, nos la inventamos.

“Wait wait wait wait, ¿qué? O sea, mucha desiderata mucha desiderata para decirme que me tengo que inventar algo”. Bueno, no, no lo inventamos. :math:`P(H)` debe representar nuestro conocimiento *a priori*, desde antes que tuviéramos los datos. En este caso, Bayergh va a decir que no tenía ni puta idea, y va a suponer que todas las hipótesis son igualmente probables *a priori*.

Y listo, esto te termina dando que la probabilidad de los datos dada cada hipótesis, en este caso, es

.. :math:

   P(f|N)=Nf^N

Entonces, ¿cuál es la probabilidad de que salga el sol cada día? La fórmula de arriba no nos lo termina de decir. Nos dice cuál es la probabilidad de que la probabilidad de que salga el sol cada día sea :math:`f`. Pero no te preocupes, porque la probabilidad de que salga el sol mañana (pongámosle M a tal afirmación), dado que la probabilidad de que salga el sol sea :math:`f`, es :math:`f`. Duh. Entonces, ponderando cada posible valor de :math:`f` podemos calcular la probabilidad que nos dan los datos de que salga el sol mañana. Yo hice la cuenta, da :math:`N/(N+1)`.

Cojonudo, ¿no? Reemplazando por los días de vida de Bayergh, eso nos da una probabilidad de un :math:`99.97...%`. Así de seguro está el Bayergh.

¿Ahora, qué onda el logaritmo? Nada, un detalle. Bayergh cuantificó su grado de certeza como una cantidad que se llama la *evidencia*, que es el logaritmo del cociente entre la probabilidad de la hipótesis sea cierta con la probabilidad de que la hipótesis sea falsa. Y como la probabilidad de que salga el sol es :math:`N/(N+1)` y la otra es (por completitud) :math:`1/(N+1)`, ese cociente da :math:`N`, y Bayergh le sacó el logaritmo a eso. *Unidades van, unidades vienen*.

================================================================
Filosofanding: ¿Qué onda el conocimiento?¿y la vida?¿y la jermu?
================================================================
El camino hasta ahora
---------------------
Consideramos los problemas del razonamiento deductivo e inductivo. El razonamiento deductivo consiste de afirmaciones que son o verdaderas o falsas, y a menudo podemos construír demostraciones rigurosas que cimientan una relación hipótesis-consecuencias ineludible. En la vida real, sin embargo, a menudo esta clase de razonamiento es insuficiente, pues las hipótesis sólo nos permiten cambiar nuestro grado de convicción en tanto a las consecuencias, pero sin descartar todas las alternativas. En ese caso, el razonamiento que debemos llevar a cabo es inductivo.

A partir de un par de puntos que deseamos incorporar en nuestra forma de realizar pensamiento inductivo, o “razonamiento plausible”, encontramos un conjunto de reglas matemáticas bien definidas: la “regla de la suma” de probabilidades, y el teorema de Bayes. Estos dos definen las reglas para manejar probabilidades que conocemos.

Ahora, esto está lejos de ser el final del recorrido. Hay preguntas abiertas dentro de la misma teoría, y nada quita que no sea superada por teorías venideras, más completas. Lo único que sabemos es, que si dicha teoría ha de respetar la desiderata, va a incorporar reglas por encima de las ya encontradas. A fin de motivar la filosofancia, dejo acá un par de secciones con comentarios que se me ocurren.

¿Entonces es subjetivo?
----------------------------
*It has always been...*

Bueno, es un decir. La pregunta deviene de que, en la interpretación bayesiana, para poder ver qué te dejan concluír los datos respecto de las hipótesis que estás considerando, tenés que definir tu grado de convicción **a priori** respecto de dichas hipótesis. `Pero eso es otra ventaja. Es un plus <https://youtu.be/EnSV7h6Lx4g?t=9>`_. Bajo esta interpretación, podemos usar la teoría de las probabilidades para cuantificar cómo nuestra incerteza sobre nuestras hipótesis se transforma en una incerteza respecto de nuestras conclusiones.

Esto permite, por ejemplo, realizar estimados que extrapolan a partir de la experiencia previa. Nos hace escépticos respecto de conclusiones que contradigan al conocimiento previo, lo cual es ciertamente deseable. Por ejemplo, imaginemos que viene alguien y nos dice que tal persona ha hecho una maldad. No nos inclinamos a creerlo de la misma manera si la tal persona era, en nuestro entendimiento, generalmente bien intencionada, que si la entendemos como alguien de morales livianas. ¡Y es razonable! Generalmente hay muchos factores que hacen que la data “Ramiro me habló mal de Lenargh” no me haga concluír mal sobre Lenargh. Ramiro puede estar equivocado, quizás intencionalmente, quizás inintencionalmente.

De este modo, la probabilidad Bayesiana nos deja incorporar distintas convicciones previas y ver qué conclusiones sacamos. Pero no siempre es bueno tener las conclusiones sesgadas a nuestro entendimiento previo. Por ejemplo, un científico que quiere poner a prueba una hipótesis en la que cree, no querrá interpretar sus resultados con amor; querrá ser *escéptico*. ¡Pos se puede! De la misma forma que uno puede poner su estado de creencia en las cuentas para saber qué le da como seguridad tras los hechos, uno puede poner en las cuentas un estado de creencia escéptico respecto de lo que uno cree. De ese modo, la evidencia recolectada tendrá que ser más abrumadora todavía, y si tal evidencia aún lleva a las mismas conclusiones, podremos estar más convencidos de que estamos concluyendo lo que concluímos no porque queremos, sino porque la evidencia lo amerita.

Ahora, plasmar el conocimiento previo no es tarea trivial, y es motivo de controversia también. Quizás en el ejemplo de la salida del sol, donde hay dos alternativas, es bastante sencillo decir “no sé nada” en probabilidades. Decimos “Y, cada alternativa me parece igualmente probable”. En la vida real eso se pone mucho más difícil. Ponele que incorporo todas las alternativas que se me ocurren; ¿puedo simplemente decir “son todas igualmente probables”?. No, no puedo, porque quizás hay una mayoría de las alternativas que se me ocurrieron que se inclinan a cierto resultado particular. Entonces, decir que son todas **esas** alternativas igualmente probables implica que ese resultado es particularmente más probable.

Los hijos de puta de los noticieros un poco aprovechan un fenómeno similar. A partir de seleccionar cuidadosamente de qué hablo y de qué no, puedo “no mentir”, y sin embargo llevar a la gente a concluír cosas sesgadas a favor de una postura que quiera beneficiar. De hecho, en mi diccionario personal, eso cuenta como mentir, aunque no haya “información falsa”.

¿Entonces si no me manejo con probabilidad bayesiana soy une pelotude?
----------------------------------------------------------------------
Y, yo me veo inclinado a pensar que sí, pero qué se yo. Esta pregunta viene de que un amigo me dice “lo que no me gusta de los bayesianos es que son sectarios, no admiten alternativas”. ¡Pero vos lo viste al teorema! El teorema nos da a la probabilidad bayesiana como requisito inexorable para cumplir con la desiderata, que es bastante razonable. Al menos respecto a la desiderata 2 y 3, no le veo sentido a permitirse fallarle. ¿Qué mérito hay en tener tu propia forma de pensar, si te hace inconsistente, o sesgado?

Pero sí pueden pasar varias cosas que ameriten no ser bayesiano.

**Posibilidad 1:** El teorema podría estar mal. Hasta donde tengo entendido no es el caso, pero si ocurriera, la premisa entera cae. Nos veríamos nuevamente buscando algún compás en un mundo de incertidumbre.

**Posibilidad 2:** Es difícil o impracticable. Y sí papu, yo no tengo una lista de *priors* contra las cuales contrasto toda la data que me viene. Este es un tema que por ahí me gustaría ahondar más en un futuro, porque da la impresión que el cerebro es *bastante* bayesiano (`excepto <https://www.youtube.com/watch?v=cFv5DvrLDCg>`_). ¿En qué sentido? yyy, más o menos sigue la desiderata 2. La de la correspondiencia con el sentido común. En fin, el tema es que a menudo tenés que *estimar* el procedimiento bayesiano, sin usar numeritos. Yo siento que pienso en nubecitas, además.

**Posibilidad 3:** El teorema podría estar mal aplicado. Esto no es tanto un “amerita no ser bayesiano”, sino un, “hay que serlo donde hay que serlo”. ¿Cuándo hay que serlo” cuando queremos cuantificar grados de entendimiento siguiendo lo pautado en la desiderata. ¿Queremos hacer siempre eso? No. Veamos varios ejemplos.

En la ciencia: Cuando fuéramos a reportar alguna estimación, por supuesto que está bueno usar probabilidad bayesiana. Qué se yo, vas a querer reportar probabilidades de que tal cosa te de cáncer con un análisis sólido y con fundamentos. Pero después, ponele, a la hora de pensar, no hace falta condicionar nuestros divagues a ello. A menudo es útil ponderar sobre ideas inverosímiles, que quizás o nos permite encontrar herramientas que luego apliquen en otras circunstancias, o nos permite darnos cuenta que en realidad no eran tan inverosímiles.

Otro ejemplo. Ponele que vas caminando por una plaza y te topás a un Bru salvaje arriba de un árbol. Si quieren les cuento de la vez que me rodearon 7 policías por subirme a un árbol. Pero nada, cuestión. Si ponés los números, claramente es más probable, aunque sea mínimo, que me pegue un palo por estar subido ahí. Ahora, la evaluación costo-diversión que yo hago no tiene por qué coincidir con la que vos hacés. Y esto pasa con todo. Con la salud, el deporte, los estilos de vida. La teoría cuantifica conocimientos. Después, lo que uno haga con eso, nuevamente, es subjetivo.

La métrica de las ideas
-----------------------

Muchas veces escucho a la gente decir “vos opinás de una forma, yo de otra”. Lo cual es cierto. Todes tenemos opiniones, creencias, valores, y hasta formas de tomar conclusiones. Sería imposible encontrar un terreno común a todos, y ni siquiera sé si sería deseables: del intercambio de ideas es que nace el entendimiento.

Pero esa frase a veces me da la impresión de que se sugiere por lo bajo que “toda forma de tomar conclusiones es válida”. Ahí no, mi niñe. Ciertamente nuesta manera de pensar condiciona nuestra manera de actuar. Si las consecuencias de nuestras acciones nos importan, entonces nos debe importar la forma en la que formamos las ideas que preceden a las decisiones.

Los teoremas de Cox (ejejej), limitados como sean, nos dan un ejemplo claro de que si tenemos determinadas expectativas respecto de nuestra forma de pensar, no lo conseguiremos de cualquier manera y a ciegas. No toda la desiderata es alcanzable, como la de tener todo en numeritos. Difícilmente sea posible encontrar una metodología cerrada e infalible para ser consistentes e imparciales en nuestra forma de pensarlo. Ciertamente “remitirse a los datos” no lo es, pues normalmente hay una etapa interpretativa previa, que te dice qué datos registrar, y una posterior, que te dice cómo interpretarlo.

Todo este palabrerío debería entonces servirnos no de desmotivador, sino lo contrario. Debemos hacer nuestro mejor esfuerzo para revisar *qué pensamos*, *cómo pensamos*, y *por qué* lo pensamos. Cada error no es sino una huella medio desviada en un largo camino hacia comprendernos, comprender el mundo que nos rodea, que por consecuencia nos permitirá decidir a conciencia, y sólo así, ser libres.

Etcétera
--------

A fin de publicar esto de una vez, lo dejo ahí. Me quería tomar el trabajo de sacarle juguito, pero va a ser más fructífero volver esto algo colaborativo. Entonces, si llegaste a leer hasta acá y tenés dudas, objeciones, críticas, o ganas de flashearla, me contactás <3.
