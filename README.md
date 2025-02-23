# EJERCICIOS DE BÚSQUEDAS

## Ejercicio 1

Considérese el problema de encontrar un camino, en la situación representada en la figura, desde la posición $i$ hasta la posición $e$. El NPC (*non-player character*) puede moverse de forma horizontal y vertical, un solo cuadrado en cada movimiento (cada movimiento tiene coste uno). Las zonas sombreadas impiden el paso del NPC a través de ellas.

### Algoritmos a aplicar:

Aplicaremos los distintos algoritmos de búsqueda que se tratan en las sesiones del módulo para resolver el problema, en el siguiente orden:

1. Búsqueda en anchura.

![Ejercicio1 - Busqueda en anchura](anchura.jpeg)


2. Búsqueda en profundidad.

![Ejercicio1 - Busqueda en profundidad](profundidad.jpeg)

- Con límite de profundidad 5 no se alcanza el objetivo, provocando fracaso por valor de corte (en el límite propuesto, no se alcanza el objetivo).
- Con límite 6 se alcanza una solución más eficiente que en la versión sin límite, la cual alcanza el objetivo en profundidad 10.


3. Búsqueda de coste uniforme.
![Ejercicio1 - Busqueda de coste uniforme](coste_uniforme.jpeg)

5. Algoritmos **A** y **A***.
![Ejercicio1 - Algoritmos A y A*](algoritmo_A_A*.jpeg)


## Ejercicio 2

### Preguntas específicas:

#### La heurística utilizada en el algoritmo **A**, ¿es admisible? ¿Por qué?
Sí, la heurística es admisible ya que nunca sobreestima el costo real hacia la meta.


#### ¿Podemos decir que el algoritmo es **A***?   
Sí, usando una heurística admisible logró encontrar la ruta más eficiente (de menor costo).

## Ejercicio 3

En el hipotético caso de que el servicio Google Maps empleara el algoritmo de **búsqueda por coste uniforme** para encontrar la ruta más corta (en km) entre dos localidades, calcula la solución que ofrecería para la ruta **Ourense-Calatayud** dadas las siguientes distancias kilométricas:


![Ejercicio3 - mapa_Ourense Calatayud](mapa.png)




| Trayecto            | Distancia en km      |
| :------------------ | :------------------:|
| Ourense, Ponferrada | 175                 |
| Ourense, Benavente  | 236                 |
| Ponferrada, León    | 113                 |
| Ponferrada, Benavente | 125               |
| Benavente, León     | 75                  |
| Benavente, Valladolid | 112               |
| Benavente, Palencia | 112                 |
| Palencia, León      | 131                 |
| Palencia, Valladolid | 48                 |
| Palencia, Osorno    | 49                  |
| Palencia, Burgos    | 92                  |
| León, Osorno        | 121                 |
| Osorno, Burgos      | 59                  |
| Valladolid, Aranda  | 95                  |
| Burgos, Aranda      | 84                  |
| Aranda, Osma        | 58                  |
| Osma, Calatayud     | 140                 |
| Osma, Soria         | 58                  |
| Burgos, Soria       | 143                 |
| Burgos, Logroño     | 150                 |
| Logroño, Soria      | 106                 |
| Soria, Calatayud    | 91                  |


### Para facilitar la escritura durante la realización del ejercicio se renombraron las ciudades (nodos) de la siguiente manera:
| Ciudad             | Nodo                 |
| :------------------ | :------------------:|
| Ourense              | i                |
| Ponferrada          | A                |
| Benavente  | B               |
| León | C               |
| Osorno     | D                  |
| Palencia | E               |
| Valladolid | F                |
| Burgos      | G                 |
| Aranda | H                 |
| Osma    | I                 |
| Soria    | J                  |
| Logroño        | K                 |
| Calatayud      | e                 |

![Ejercicio3 - búsqueda por coste uniforme Ourense Calatayud](recorte_ourense_calatayud.jpeg)

