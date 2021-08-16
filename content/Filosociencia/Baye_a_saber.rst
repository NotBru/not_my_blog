Baye-a-saber
############

:date: 2021-08-15
:tags: probabilidad, filosofía, ciencia, epistemología
:category: Filosociencia
:author: Bru
:slug: baye-a-saber
:lang: ñl

(Este post está basado en los primeros dos capítulos del libro “Probability Theory: The Logic of Science”, de Edwin T. Jaynes. El primero detalla los conceptos, y es sumamente accesible, por lo que se lo recomiendo a quien sea que le gusten los tópicos del post. El segundo tiene las cuentas, que tampoco vienen mal, pero es una lectura un poco menos accesible.)

Son las hace-tres-millones-de-años de la tarde. Te vas poniendo tu animal print 0% vegano porque pegó un chucho de la san mamut, y te juntás con la Ugnorr a charlar de aquella vez que la muchachada encontró un `laser raptor <https://www.youtube.com/watch?v=bS5P_LAqiVg>`_ suelto o qué se yo. Acá no hay ningún paleontólogo leyendo, ¿no?

Mirás al horizonte y notás que el sol, que venía estando todo pipón hace rato, está cada vez más rojo y se mete cada vez más abajo en el horizonte. “Ah, la cachucha” decís... Se nos fue. “Aparecerá de nuevo”, pregunta la Ugnorr, un poco preocupado. “Y, no sé, habrá que ver”, tirás.

Es en ese momento que el Bayergh, que justo andaba persiguiendo un mamut por ahí cerca o eso o algo, escucha de querusa y se prende a la conversación. Se para y dice, “Nah bro. Pero seguro viene otro. Estoy :math:`10\log_{10} N` seguro de ello, donde :math:`N` es la cantidad de días que llevo vivo.”. ¿Kíííh?¿Qué pasó acá?

=====================
Deducción e inducción
=====================
Sí, ya sé cuál es tu problema con el escenario anterior: ¡La inescrupulosa afirmación de Bayergh no tiene fundamentos inquebrantables! Después de todo, yo conozco un planeta donde una vez el sol se puso, y no salió nunca más...

La `disyuntiva epistemológica <https://www.youtube.com/watch?v=p9ZdeARKTzE>`_ que aquí nos concierne es que nadie en esta conversación ha demostrado la afirmación que se estaba tomando por cierta. ¿Cómo demostrás que el sol va a salir todos los días? Hoy día no sólo poseemos abundante evidencia de que estamos parados en una roca orbitando una aglomeración gigante de átomos de hidrógeno que hacen pogo, y potencialmente un tazón de petuñas. Sabemos además que el sol es una estrella tipo enana amarilla, y de nuestro entendimiento observando otras estrellas sabemos cuánto va a durar ahí, etc...

Y aún así, nada te dice que qué se yo, no vaya a venir un `agujero negro salvaje <https://futurism.com/theres-a-rogue-black-hole-streaking-through-the-universe>`_ que vaya a ponerle fin a `Friedrick, Cesil y sus amigues, y todo lo que es bueno en esta vida <https://www.youtube.com/watch?v=jxepnIG1yQQ>`_. Hilando fino, no podemos tener una certeza absoluta al respecto. Y sin embargo, entendemos que el sol va a salir mañana con “casi certeza”. Nadie está particularmente dubitativo al respecto. Seguro, el sol capaz deja de salir algún día, pero eso sorprendería a todos.

Esto es lo que pasa más frecuentemente dentro de la ciencia, y también dentro de la vida cotidiana. La información a nuestro alcance nos permite declarar conclusiones *probables*, pero no *deducibles*. Si salgo afuera y las nubes están re negras, y hay un qué se yo en los huesos, es *probable* que llueva, pero no es una realidad inevitable. Si no llueve, no nos sorprendería demasiado nuestra equivocación.

A esa clase de razonamiento se le llama razonamiento inductivo, y contrasta con el razonamiento deductivo, donde de las premisas se derivan consecuencias ineludibles. Como ejemplo de este otro tipo de razonamiento tenemos, por ejemplo: “Todos los hombres son mortales. Sócrates es hombre. Por lo tanto, Sócrates es mortal.”

Todos los razonamientos deductivos, en el fondo, toman la forma de los silogismos “**A** implica **B**. **A** es cierto. Por lo tanto, **B** es cierto” y “**A** implica **B**. **B** no es cierto. Por lo tanto, **A** no es cierto”. Y en las circunstancias donde podemos aplicarlos son sumamente poderosos, ya que nos dan certeza absoluta, y podemos utilizar estas certezas a nuestra ventaja a la hora de decidir qué hacer.
