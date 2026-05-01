# Lineamientos

---

![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.explicit.bing.net%2Fth%3Fid%3DOIP.l81pdDnqVKY0N-0jneuhEAHaEK%26pid%3DApi&f=1)

---

## Visión General

Bienvenido a la tarea de anotación. En esta tarea presentaremos un *tweet* en conjunto con el hilo de conversación asociado y te pediremos clasificarlo indicando a que clase pertenece dado su contexto, estos datos nos permitirán generar un *dataset* de libre acceso el cual será liberado a la comunidad científica, con el cual construiremos un modelo de baseline el cual permitirá generar comparativas ahondando en el desarrollo de esta área nivel nacional.

## Conceptos

Queremos que clasifiques cada *tweet* como **odio** o **no odio**, en el caso de ser de **odio** será obligatorio indicar la comunidad objetivo al cual esta dirigido el *tweet* pudiendo ser estas **comunidades migrantes**, **comunidad LGBTQ+**, **mujeres** y **pueblos originarios**, en caso contrario y ser un *tweet* de **no odio** si se encuentra alguna de las comunidades mencionadas será necesario indicarla.

El concepto de presencia de **odio** con el que se trabajará se encuentra ligado al concepto de discurso de odio definido por la ONU como: *"Cualquier forma de comunicación de palabra, por
escrito o a través del comportamiento, que sea un ataque o utilice lenguaje peyorativo o discriminatorio en relación con una persona o un grupo sobre la base de quiénes son o, en otras palabras,
en razón de su religión, origen étnico, nacionalidad, raza, color, ascendencia, género u otro factor de identidad"* Si se desea ahondar en el tema recomendamos revisar el [plan de acción de la ONU](https://www.un.org/en/genocideprevention/documents/advising-and-mobilizing/Action_plan_on_hate_speech_ES.pdf) para más definiciones respecto a que es el deicursso de odio)

En esta tarea utilizaremos la definición de discurso de odio acotada como:

* Discurso de Odio: Texto o mensaje que constituya un ataque o promueva la discriminación de una persona o grupo sólo sobre la base de pertenencia a uno de los siguientes grupos: **comunidades migrantes**, **comunidad LGBTQ+**, **mujeres** y **pueblos originarios**

La dificultad principal de esta tarea yace principalmente en dos casos el primero es cuando es discurso de odio pero no utiliza lenguaje peyorativo de por sí, si no que la frase completa busca mostrar al grupo mencionado como menos capaces en cualquier ámbito físico, mental, monetario, amoroso, etc. o menos merecedores del acceso a derechos a los cuales los miembros comunes del contexto social (entiéndase como todos aquellos que no forman parte del grupo mencionado) tienen acceso con facilidad. El segundo caso corresponde al uso de lenguaje peyorativo pero que en su contexto no es considerado dsicriminatoria es decir utilizar estas palabras al hablar de un amigo bromeando o de manera sarcástica, este caso es de vital importancia puesto que en el contexto social y comunicativo del dialecto chileno este método comunicativo es altamente frecuente en situaciones informales o al relacionarse con pares.

Para esta tarea también introduciremos el concepto de *contexto* cotexto se encuentra definido por la [RAE](https://www.rae.es/dpd/contexto) como *"Entorno lingüístico de una palabra, frase o fragmento considerados, del que depende muchas veces su sentido"*, para esta tarea es de vital importancia que al clasificar el *tweet* entregado usted utilice el contexto para encontrar el sentido real de la frase, es decir pueden existir frases con sentido aparentemente inocuos por sí solas como "si así debería ser" pero que revisando el contexto su significado puede cambiar notoriamente por ejemplo el *tweet* anterior puede darse como una respuesta al siguiente *tweet* "Solo la gente blanca debería controlar el país", donde si bien el *tweet* anterior no utiliza lenguaje peyorativo contra un grupo específico en este caso busca disminuir los derechos de todos aquellos que no pertenezcan al grupo en cuestión y por lo tanto en su contexto el tweet si contribuye al discurso de odio.

En general estos casos de odio utilizan argumentos falaces y esto nos permite facilitar su detección en cierto sentido a continuación se muestran algunos tipos usuales y en los siguentes links pueden ver falacias mas a fondo [clasificaciones de falacias](https://es.wikipedia.org/wiki/Falacia#Clasificaciones), [tipos](https://es.wikipedia.org/wiki/Anexo:Falacias)

### Clases

Para cada *tweet*, elija primero alguna de las siguientes clases

* **Odio** Si un *tweet* en el contexto del hilo en el que se encuentra incita al odio de acuerdo al concepto indicado con anterioridad. Por ejemplo
  * "lo llama matrimonio, bien por los que lucharon por eso pero para mí va a seguir siendo un concepto que une a un hombre y a una mujer. Simple."  (este tweet implica que el matrimonio entre parejas homosexuales no es valido, implica que los miembros de esta comunidad carecen de acceso a los mismo recursos y derechos que otras personas que no pertenecen a esta comunidad)
  * "Es que no se como la vamos a nombrar, porque no es persona menstruante ni persona eyaculante, le podremos decir maricon a secas?" (utiliza lenguaje peyorativo para referirse y burlarse de toda una comunidad, no siendo un caso de borma entre amigos o auto ironia)
* **No Odio** Si un tweet no presenta odio. Por ejemplo
  * "cansona triplehijueputa, hija de las tres miles putas, malparida, perra, puta, cansona, me tenés mamada, sapaaaaa

      de: mi
  
      para: mi ansiedad" (En este tweet se utiliza lenguaje peyorativo, sin embargo lo utilizar para burlarse de si misma por lo cual no corresponde a lenguaje de odio)

Para cada *tweet*, una vez clasificado en alguna de las clases anteriores determine  Si el tweet hace referencia a alguna de las siguientes comunidades:

* **Comunidad LGBTQ+** Por ejemplo:
  * "Yo soy heterosexual y quiero que mis hijos sean heterosexuales algún problema?" (Odio, el argumentar que la identidad sexual de los hijos es definida por los padres es incorrecto y busca promover que aquellos con orientaciones distintas son menos validos que quines poseen orientaciones sexuales covnecionales.)
  * "Profe, mi mamá me dijo que usted es gay." (No odio, no utiliza lenguaje peyorativo ni busca discriminar si no que mas bien parece estar realizando un cuestionamiento a alguien en base a a un comentario generado en torno al interlocutor mencionado)
* **Mujeres**  Por ejemplo:
  * "Existe vida tras ser feminazi. Hay gente que evoluciona cuando empieza a leer y pensar. Un aplauso." (Odio, busca perpetuar la visión del feminismo como una postura ideologica perteneciente a aquellos de bajo nivel intelectual con lo cual cae en al discriminación)
  * "Re sola estoy igual q vos gorda puta" (No Odio, si bien esta insultado a alguien el emisor del mensaje deja en claro que ambas se encuentran a un nivel de pares en los que respecta a su soledad)
* **Pueblos Originarios** Por ejemplo:
  * "Wnes imbeciles diciendo Que Emoción!!!! Mientras la mayoría de los Chilenos pagamos Contribuciones, no así los Mapuches, les siguen dando más beneficios, mientras el 90% se los debemos financiar. Aweonaos." (Odio, se utilizan argumentos falaces para apoyar la discriminación hacia pueblos originarios, señalando que ellos no pagan contribuciones y viven de dineros del estado)
* **Comunidades Migrantes** Por ejemplo:
  * "Todos los venezolanos son flojos, vienen a puro robar" (Odio, utiliza argumentos falaces como la generalizacion para señalar que toda la comunidad de migrantes venezolanos son flojos y criminales.)
