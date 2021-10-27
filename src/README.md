# Huida del talento y falta de Personal, en el Sector hostelero post-COVID

Expertos hoteleros están presentando una realidad nunca vista, la huida del talento y escases de personal en el área del sector turístico, post-COVID , en dicho estudio se hará referencia específicamente a la Hostelería en la ciudad de Madrid. Problemática que al estar la ocupación de los hoteles muy bajo no se acentúa tanto como lo será en los próximos meses.

Tal como nos comenta Gonzalo Armenteros el CEO de Soho Boutique Hotels, en su entrevista por Hosteltur (8/10/2021) “Hay que trabajar el cliente interno porque sin el no habrá cliente externo”, entendiendo por cliente interno al capital humano del sector de Hostelería. 

Distintas cadenas hoteleras están buscando soluciones para mantener a sus empleados e intentar volver a tener ese capital humano capacitado de vuelta, luego de los ERTEs, o paro (si tenían contratos parciales). Pero la realidad es que ya se han fugado a otros sectores que les ofrece mejor calidad de vida, mejor salario y mejores condiciones.

# Variables:
Variable Independiente (causa) : bajo nivel de motivación, horarios del sector hostelero, tiempo libre, conciliación familiar (Esta variable es cualitativa y seria difícil de comprobar).

Variable Dependiente (efecto): El desempleo aumenta en el sector  hotelero y el talento busca alternativas fuera de la industria.

Variable interviniente : Ocupación hotelera, Personal contratado, Tasa de paro, Tasa de ERTEs, Tasa de afectados por COVID. 

# Hipótesis :
El personal contratado en Hostelería ha bajado en relación a la ocupación hotelera y al ADR , la alta tasa de ERTES no justifican esta bajada, a su vez se han incrementado el personal contratado en otros sectores.

# Datos disponibles
Para confirmar o refutar la hipótesis se buscaron datos en distintas fuentes, como por ejemplo en el Instituto Nacional de Estadísticas (INE),  World Turism Organization,  DATAESTUR.es - Información de la actividad Turística de España, EpDATA.es – Europa Press, Eurostat – European Statistic, Travelgatex, Skyscanner, entre otras. Organizados por temática a continuación: 
	Empleo en el Sector Turístico:
	Empleo turístico según afiliación en la Seguridad Social 2001/2021(8), por área del Sector Hostelería (hostelería, alojamiento, comida) en España, (xlsx).  
	Empleo turístico según población activa (Ocupados, Parados) 2009/2020(trimestres) (xlsx).
	Ocupados afectados por un ERTE por sector(Servicios) 2008/2020 (csv), INE 
	Nº de personas empleadas en establecimientos hoteleros en Madrid 2017/2021(08) INE (csv) 
	Ocupación Hotelera:
	Ocupación de Hoteles en Madrid 2017/2021(8) INE (csv) 
	Establecimientos Hoteleros abiertos 2013/2021(08) INE (csv) 

# Datos complementarios
	Llegadas de turistas a España por continentes de procedencia 1995/2019, (xlsx), World Turism Organization.
	Casos diagnosticados de COVID desde que comenzó la pandemia. "Ministerio de Sanidad, Servicios Sociales e Igualdad, Universidad Johns Hopkins" (csv) 
	Muertos por COVID en España "Universidad Johns Hopkins, Ministerio de Sanidad, Servicios Sociales e Igualdad" (csv). 

# Usos de los Datos
Tal como podemos ver, los datos mayoritariamente estaban en formatos de csv o xlsx, nuestra columna de referencia común para todos: fue la fecha, lo que ayudo a la comparativa de los mismos. Si bien, no se usaron todos los datos, nos sirvió de referencia a la hora de extraer información pertinente. 

Se realizó una Tabla General, en donde se juntaron cada base de datos en una columna de la misma, organizadas por la fecha, se realizó un proceso de transformación ya que las fechas no se mostraban en el mismo formato en todas, unos en meses y otro es trimestres. Además, se crearon varios data frames partiendo de Tabla General para realizar algunos filtros que facilitaran la graficación de los mismos.   

A nivel de limpieza se usaron en Python librerías como Numpy y Pandas para el tratamiento de los datos, la verdad fue bastante fácil, porque no había datos nulos, simplemente algunos datos fueron encontrados para mas años que los otros, pero a la hora de realizar comparaciones se toma en cuenta los rangos de fechas disponibles por categorías. 

A la hora de graficar se usaron distintas librerías de Python, como Seaborn, Plotly, Matplotly,  además de usar Tableu. Dependiendo de lo que se quería graficar se decantó por una u otra, según su versatilidad y funcionalidad. La dificultad estuvo en descubrir cual era la mejor herramienta para plasmar de la manera mas entendible cada información. 

# Presentación de los datos
Para la presentación se uso Power Point, guardando las graficas de Python como png, y en algunos casos creando objetos en gif para que se viera la progresión de los mismos. Se realizo una presentación bajo los principios del Storytelling donde se uso el personaje de Sofía, una recepcionista de Hotel en Madrid, que nos ayuda a desvelar porque huyen los empleados de hostelería tras la pandemia y como esta la situación del sector. 

La presentación comienza con un collage de artículos de prensa, que hablan de la huida del talento y falta de personal en el área de hostelería, debates relativamente recientes de finales del 2020 al presente. Posteriormente Sofía nos cuentas los pro y contra de trabajar en el sector, para poner en contexto al oyente.

Se realiza una primera gráfica comparativa entre los establecimientos abierto, ocupación de los establecimientos hoteleros, empleados de hostelería en situación de ERTE y cantidad de empleados en establecimientos hosteleros en Madrid. Esta primera aproximación nos ayudaría a desvelar si el personal contratado en Hostelería ha bajado en relación a la ocupación hotelera y si la alta tasa de ERTEs no justifican esta bajada. Posteriormente se agregan los valores de ADR para continuar con la comparativa. 

Dichos resultados arrojan que a nivel de los establecimientos hoteleros se ve una W mientras que en la ocupación y cantidad de empleados contratados mas bien un símbolo de Nike, de acá podemos ver como los hosteleros se apresuraron a abrir y por la baja demanda tuvieron que volver a cerrar. 

Bajo la premisa que partía la hipótesis de que había menos empleados en relación a la ocupación, tenemos que indicar que, aunque hay una relación entre el incremento de los empleados tras la apertura de los hoteles, actualmente la proporción de los empleados es mayor si se compara con la ocupación. También es de entender que, en un hotel, tanto si hay turistas como si no, requiere de un trabajo mínimo de mantenimiento y preservación.  

Con relación al ADR, que también se presumía que la baja cantidad de empleados era por el bajo ADR, vemos como luego de la apertura post pandemia, los precios son mucho mas bajos de lo que venían siendo, aunque hay una tendencia al alza, donde en pocos meses igualará el precio anterior, en donde no se podría justificar que la falta de empleados se vea afectado por ello.

También explicamos la bajada de la ocupación que han tenidos los hoteles, relacionándolo a la procedencia del turista que llega a Madrid basándonos en datos de los últimos 5 años y relacionándolo a su vez a las restricciones por COVID para viajar. 

Las graficas de ocupación y empleo tienen una significante bajado para el ultimo trimestre, esto se explica con la temporalidad del turismo en Madrid, al no ser una zona de Sol y Playa, el turismo es estacional, y verano suele ser de muy baja afluencia, siendo básicamente solo una ciudad de escala, lo cual se confirma con las altas laborales de la Seguridad Social. 

Para explicar si los ERTEs han sido un efecto puramente del sector de Hostelería se presenta un gráfico de la evolución de los ERTE por sectores (Agricultura, Servicio, Construcción, Industria) donde se muestra que todos los sectores (casi de la misma manera)han recurrido a este procedimiento de despedir trabajadores, suspender contratos de trabajo o reducir jornadas de manera temporal. De igual manera mostramos nuevamente como en el gráfico de los ERTEs actualmente en el Sector de Hostelería ya no cuentan con empleados en esa situación, lo cual es entendible ya que el Estado ya no está ofreciendo esa ayuda, que fue solo para ERTE por fuerza mayor. Con tales datos refutamos que la baja cantidad de empleados sea por que el personal siga en situación de ERTE.  

Si bien se quería confirmar, a que sectores estaban huyendo los empleados de hostelería, estos datos, al no tener ni un año de ocurrido, no son factibles de obtener, por tal razón se aportó una grafica de barras (por sexo) con los salarios por sectores, organizados de manera decreciente donde Hostelería encabeza la lista, a continuación, se presenta una grafica de burbujas en donde se presentan los Sectores mas afectadas tras la pandemia, donde igualmente Hostelería está a la cabecera.

Sumado a eso, se agrega una Nube de Palabras realizada con las valoraciones de una encuesta sobre las razones por la cual dejarías/o has dejado la hostelería realizada en LinkedIn, donde resaltan palabras como “Falta” (de lideres, respuestas, dialogo, empatía, compasión, comprensión…). 

Luego se culmina con una interpretación de las cualidades de Sofía (Softskills), para hacer ver que es totalmente posible que buscase en otros sectores y que es factible que con su preparación, ella este ya trabajando en algún otro Sector.

# Conclusiones
Se ha elegido el tema, ya que luego de 8 años de trabajo en Hoteles de lujo 5 estrellas, se tiene conocimiento del negocio, lo cual facilita la interpretación de los mismos, y la búsqueda de información pertinente y relevante. 

Por tal razón se ha planteado la hipótesis basada en la experiencia de dicho trabajo, al ser una hipótesis empírica basada en la intuición, una vez se compara con los datos, podemos ver la correlación entre las variables y como el COVID a modificado los comportamientos habituales.   

La calidad y veracidad de los datos esta garantizada ya que son extraídos de Entes gubernamentales e internacionales y especialistas en el área de Turismo. En relación a la disponibilidad el problema está que, con la pandemia, muchos de los datos que solían estar disponibles en el primer trimestre del año, aun no han sido publicados, posiblemente por que aun no se han procesado o porque no se pudieron extraer. 
    
Es de acotar que los datos obtenidos se refieren a la Hostelería de Madrid en general y que, si se extrapolaran los valores por tipo de hoteles según estrellas, posiblemente podríamos encontrar cambios, ya que el comportamiento de un Hotel perteneciente a una Cadena Hotelera Internacional , no será igual al pequeño hostelero que le cuesta mantenerse a flote.

Para un próximo estudio se pueden analizar mas variables como: el sexo, y el tipo de hoteles (estrellas), los casos de COVID por países de proveniencia de turista a Madrid, las fechas especificas de cierres de fronteras y restricciones de los mismos, entre otras. Que por cumplimiento de fechas de entrega no han dado tiempo de verificar. 
