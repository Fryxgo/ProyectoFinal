# Proyecto

### Semanal 01/04 - 08/04


- De estos videos me parecio muy interesante algo que tiene React que es el virtual DOM que basicamente precarga los cambios para no hacerlos de 1 en 1 
lo que ayuda a mejorar el funcionamiento de una web, y el funcionamiento del arbol DOM tambien esta mas optimizado, es decir los eventos pasan primero por ese nuevo arbol
tambien que el renderizado de react es que utiliza un adaptador para pasar de navegador de movil tanto de android como ios a pc

- Basicamente visto toda la parte intoductoria de que es react y sus componentes y lo basico, me toca empezar con el codigo 

### Semanal 08/04 - 15/04

  - Creando el proyecto ayer me di  cuenta de que muchos de los comandos que manda en el video estan desactualizados y he tenido que ir viendo como se hace actualmente por que esos comandos no funcionana ya, se nota que tiene sus años el curso.
  El profesor de un video al otro aparece con alguna cosa hecha y es un cristo seguirle asi, luego de instalar el Eslint da basatnte fallos

  - Una gran parte del curso, se pasa instalando paquetes al proyecto como prettier y Eslint y esturcturando este mismo, da basatnte por hecho que se sabe javascript(Es algo que ya pone el curso que es necesario) tira para alante basatnte en ese sentido y pone mucho codigo que copia y pega, que hay que parar si quieres copiarlo para poder ponerlo

  - A la hora de contar teoria es bastante aburrido, habla monotono y hay bastante continido que ni me sonaba de nada, asi que he ido viendo un poco todo por encima 

   He terminado este curso, en el examen he suspendido el primer intento, por 1 fallo, al repetirlo ya lo aprobe sin mas problemas

   - Empiezo el segndo curso y el profesor me gusta mas como explica, estoy viendo por ejemplo lo que es un toDTO que es una funcion creada para la comunicacion del front con el back, y si usa con Get y Post por ejemplo para conseguir o devolver datos al servidor
   - Este tema esta basado en usar Fetch que es para comunicarse con el servidor, y esta expicando como usarlo, se basa en responses aun que siempre tira para alante sea que te devuelve algo o no, para poder gestionar eso existens los interceptores por ejemplo.
   - Router, en react el router es el encargado de que se muestra en la pagina en cada momneto, ya que react "es una SPA" es decir usa una sola pagina html y muesta lo que quiere condicionalmente y tiene internamente la gestion de volver a la "pagina" anterior
   - Voy ahora mismo mas o menos por la mitad del curso intermedio y la verdad prefiero como habla este profesor, me parece mas ameno, eso si, se hace mas dificil entender, supongo que es por estar en el curso itnermedio
   - En este curso no hay ningun ejercicio, solo pone ejemplo pequeños de codigo, para entenderlo es mas complicado, por que ademas es codigo ya hecho

  Termine el segundo curso dentro de la carrera, aprobe el examen a la primera, y lo dicho anteriormente este ha sido un poco caos para entender pero me gustaba mas como explicaba este profesor un poco contradictorio la verdad ahora tocara empezar con React Avanzado

### Semanal 15/04 - 22/04

- Esta parte es explicada por el mismo profesor, la verdad es que esta es mas complicada de entender ya que pilla los conceptos anteriores y los lleva un poco mas.
- Aprobecho los "tiempos muertos" de las practicas para estar viendo estos videos ya que espero qeu me sirvan en un par de semanas
- En este curso habla mas sobre los Hooks, Redux y manejo de estado con ellos, habla tambien sobre gestion de errores, el modo extricto, que basicamente ayuda a que haya menos errores, renderiza todo una vez mas para ello, y habla sobre el testeo generado por React del DOM
- Este curso de React avanzado es cortito la verdad, ya me hice con este el tercer examen, aprobado al primer intento y me dispongo a empezar el primer taller, que trata de los hooks.

### Semanal 22/04 - 29/04

- Estoy viendo el penultimo curso de esta carrera, y basicamdente esta hablando de la gestion de estados en React y las distintas formas de usar el state, ya bien sea recogiondolo o seteandolo y ha enseñado como usar el local storage del navegador, que esta genial para poder guardar datos
- Termine el curso, aprobe el examen al primer intento, no se si fue por el acento que me hacia gracia o que, pero a este fue al que mas entretenido se me hice esccuhar de los 3 profesores que he visto en la plataforma
- Ahora estoy viendo el siguietne curso, el ultimo, luego solo quedan un par de talleres, y lo da el mismo profesor
- Flux es un patron que define el flujo de datos para la UI y se puede usar flux sin usar Redux ya que redux funciona utilizando Flux
  
### Semanal 29/04 - 06/05
  
- Una Action es cualquier evento que se produce en nuestra app lo que produce normalmente un cambio de estado por tanto habrá un cambio en la vista
- Action Creator es basicamente una acccion que crea acciones, nosotros no deberiamos de crear acciones deberian de ser todo a traves del action creator, es basicamente por consisatencia, es bueno usarlo ademas por que te quitras de errores semanticos ya que llemas a una funcion que te devuelve una "string" (constante) y asi no escribir esa string y luego tener fallos y que la aplicacion falle
- Selectores -> la forma de nuestro estado debe estart optimizada al como actualiza y no como se visualiza, un selector es u na función que toma un estado y devuelve una visu alizacion
- Para testear un reducer es muy sencillo por que son funciones puras de javascript entonces se pueden hacer test de forma sencilla
- Context -> nos ofrece una forma de poder compartir una prop entre componentes sin necesidad de tener que ir pasándola en cascada a todos nuestros componentes, es decir poder tener el contexto en todos los componentes eso si exportandolo claro
- React.memo en conjunción con useCallback usados en el sitio adecuado puede aportar una mejora en el rendimiento de nuestra aplicacion, pero hay que tener cuidado, por que tampoco se puede usar como locos, ya que al hacerlo conseguimos el efecto contrario, es decir en vez de mejorar mejora ralentiza la app al hacer llamadas continuamente

- DataFetching traer datos de una fuente externa, de un servidor por ejemplo o LocalStorage
- Debido a que las funciones que acceden a localStorage o a un servidor externo está fuera de nuestro control, no son consideradas funciones puras.
- Para poder lanzar side effects o efectos en React, tenemos que usar siempre "useEffect"
- Es practicamente una necesidad hacer un customHook para poder hacer varais peticiones para poder abstraer los datos no solo de 1 peticion
- Reducer y DataFetching el reducer aparte de supararnos la lógica de estado de los componentes, nos permite aunar una única función todos los cambios de estado necesarios ppara una acción
Y es en dataFeching donde cobra sentido ya que normalmente queremos varios cambiosa de estado
d
### Thunk

- Un thunk es la función devuelta por otra función const add = (a,b) => () => a+b
- Thunks con Reducers -> son usados principalmente para hacer middlewares
- Un reducer aparte de separarnos la lógica de estado de nuestros componentes, nos permite aunar en una única función todos los cambios de estado necesarios dada una acción.
Y es precisamente con Data Fetching donde cobran mucho sentido, ya que por lo general vamos a querer realizar varios camios en el estado depende de la acción.

Examen, realizado 1 vez con 16 aciertos  -> Aprobado
- Ahora haré los talleres, los cuales subire directamente a git una vez hechos

  
### Semanal 06 /04 - 13/05

- Se me habia olvidado hacer el commit del taller 2, lo he hecho en local y se me olvido hacer el commit, no pude hacerlo el lunes tampoco o el martes a primera por lo ya comentado, estuve ocn otitis y no estuve en la empresa y este taller lo hice alli para aprovechar el tiempo

## Termine la carrera, tanto los cursos como los talleres
