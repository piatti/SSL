# Fases de la Traducción y Errores

### Objetivos
Identificar las fases de traducción y errores


### Temas
- Fases de traducción.
- Preprocesamiento.
- Compilación.
- Ensamblado.
- Vinculación (Link).
- Errores en cada fase.

### Tareas
1. Investigar  las  funcionalidades  y  opciones  que  su  compilador  presenta  paralimitar el inicio y fin de las fases de traducción.
2. Para la siguiente secuencia de pasos:
a. Transicribir en readme.md cada comando ejecutado y
b. Describir en readme.md el resultado u error obtenidos para cada paso.

### Secuencia de Pasos
1. Escribir hello2.c, que es una variante de hello.c:
Secuencia de Pasos
``` C
#include <stdio.h>

int/*medio*/main(void){
     int i=42; prontf("La respuesta es %d\n");
```
2. Preprocesar   hello2.c,   no   compilar,   y   generar hello2.i.   Analizar su contenido.
3. Escribir hello3.c, una nueva variante:
``` C
int printf(const char *s, ...);
int main(void){
     int i=42; 
     prontf("La respuesta es %d\n");
```
4. Investigar la semántica de la primera línea.
5. Preprocesar hello3.c, no compilar, y generar hello3.i. Buscar diferencias entre hello3.c y hello3.i.
6. Compilar el resultado y generar hello3.s, no ensamblar.
7. Corregir  en  el  nuevo  archivo  hello4.c  y  empezar  de  nuevo,  generar hello4.s, no ensamblar.
8. Investigar hello4.s.
9. Ensamblar hello4.s en hello4.o, no vincular.
10. Vincular hello4.o con la biblioteca estándar y generar el ejecutable.
11. Corregir en hello5.c y generar el ejecutable.
12. Ejecutar y analizar el resultado.
13. Corregir en hello6.c y empezar de nuevo.
14. Escribir hello7.c, una nueva variante:
``` C
int main(void){
    int i=42;
    printf("La respuesta es %d\n", i);
}
```
15.Explicar porqué funciona.

### Restricciones
El programa ejemplo debe enviar por stdout la frase La respuesta es 42, elvalor 42 debe surgir de una variable.

### Resolucion

2. gcc -E hello2.c -o hello2.i Sigue siendo legible, se importan librerias estandar

4. Es el prototipo de printf

5. Haciendo un dif ala unica diferencia esta en el encabezado de hello3.i

6. No se puede compilar por un warning en la definicion de prontf. Sugiere la declaracion printf

8. Es hello4.c en assembler

9. Error en la referencia de prontf

10. No se puede generar el ejecutable

12. Se genera el ejecutable pero la respuesta no es la esperada

13. En este caso se genera el ejecutable y la respuesta es la esperada

15. A pesar de la advertencia del compilador por la falta del prototipo de la funcion printf el linker logra en encontrar la definiciones
