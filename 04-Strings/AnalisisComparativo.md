# Análisis Comparativo del tipo String en Lenguajes de Programación

Realizar un análisis comparativo de dato String en el lenguaje C versus un lenguaje de programación a elección. El análisis debe contener, por lo menos, los siguientes ítems:

#### a. ¿El tipo es parte del lenguaje en algún nivel?
* C: No existe el tipo de dato String
* P: Existe el tipo de dato str, pertence al lenguaje

#### b. ¿El tipo es parte de la biblioteca?
* C: No porque no existe el tipo de dato
* P: Si

#### c. ¿Qué alfabeto usa?
* C: ASCII
* P: ASCII + Unicode


#### d. ¿Cómo se resuelve la alocación de memoria?
* C: Mediante la alocacion estatica (no se puede cambiar durante la ejecucion) y alocacion dinamica (se reserva en tiempo de ejecucion)
* P: Cuenta con un garbage collector que permite la abstraccion de liberar memoria cuando un objeto ya no esta siendo referenciado en el programa

#### e. ¿El tipo tiene mutabilidad o es inmutable?
* C: Mutabilidad 
* P: Inmutabilidad

#### f. ¿El tipo es un first class citizen?
* C: No
* P: Si

#### g. ¿Cuál es la mecánica para ese tipo cuando se los pasa como argumentos?
* C: Se pasa el primer caracter de la cadena
* P: Se pasa la variable como argumento

#### h. ¿Y cuando son retornados por una función?
* C: Retorna el puntero al primer caracter de la cadena 
* P: Retorna la variable
