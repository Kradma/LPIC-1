* Átomos simples de las expresiones regulares:
  * `.`: Cualquier caracter.
  * `^`: Coincide con el inicio de línea.
  * `$`: Coinicide con el final de línea.
* **En las expresiones regulares básicas hay que escapar**

# Expresión de corchetes
* Lista de caracteres literales encerrados por \[\], hace que el grupo coincida con uno de los caracteres de dentro de los corchetes.
* Se hace que NO coincida con uno de los carácteres del interior.
* [x-X] indica un rango de caracteres.
  * \[:alnum:\]: Caracter alfanumérico.
  * \[:alpha:\]: Caracter alfabético.
  * \[:ascii:\]: Carácter del juego ASCII.
  * \[:blank:\]: Caraácter en blanco.
  * \[:cntrl:\]: Carácter de control.
  * \[:digit:\]: Dígito del 0 al 9.
  * \[:graph:\]: Cualquier carácter, salvo el espacio.
  * \[:lower:\]: Cualquier carácter en minúscula.
  * \[:print:\]: Cualquier carácter imprimible.
  * \[:punct:\]: Cualquier caracter imprimible, salvo espacios y alafuméricos.
  * \[:space:\]: Caracteres d eespacio en blanco.
  * \[:upper:\]: Cualquier letra en mayúscula.
  * \[:xdigit:\]: Dígitos hexadecimales.


# Cuantificadores
* Vendrían indican la cantidad de veces que aparece un átomo simple.
* `*`: El átomo aparece cero o mas veces.
* `+`: Una o más veces.
* `?`: Una vez o ningúna.

# Límites
* `{i}`: El átomo aparece exactamente **i** veces.
* `{i,}`: El átomo aparece al menos **i** veces.
* `{i,j}`: El átomo aparece mínimo **i** veces y máximo `j`. 

# Ramas y referencias posteriores
* `|`: Se utiliza como separador.
* Se suele utilizar con `()`.
* Se puede utilizar tal que `(a|b|aeio)\2` de forma que se seleccione aquella que aparece menos dos veces.

# Búsqueda con expresiones regulares
* `find <DIRECTORIO> **-regex** '<REGEX>'`: Se utiliza el parámetro `-regex` seguido de `'` para indicar una expresión regular.
* Para utilizar expresiones regulares extendidas hay que hacer uso de `-regextype posix-extended` o `-regextype egrep`
* `less`: permite realizar búsquedas de ficheros utilizando expresiones regulares.
* 
