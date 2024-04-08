# PequenoCompilador
Creación de un pequeño compilador


# Tarea Semana 5

Leer Capítulo 5 del Libro Compiladores, Principios, Técnicas y exponer en clases

#Ejercicios y Presentación con los demás compañeros:

1)    Crear un pequeño Compilador con las siguientes características:

      a.    Analizador Léxico.

      b.    Analizador Sintáctico.

      c.    Analizador Semántico. (Opcional)

      d.    Generar Tabla de Símbolos.

      e.    Generador de Código Intermedio.

      f.     Lenguaje de programación a traducir el código del compilador.

      (Utilizar cualquier herramienta) en el Lenguaje de programación de su preferencia.

2)    Documentar su Compilador y lenguaje de programación para realizar las pruebas.

3)    Subir el código a Github, enviar el código fuente y el ejecutable del proyecto.


# Detecciones actuales del Analizador Semántico
- Si se declara una variable fuera de main.
- Si se declara una variable más de una vez en el mismo ambito.
- Si se le añade un tipo de dato que no le corresponde a una variable (solo funciona int, float o double).
- Si una variable no ha sido declarada.



# Código para prueba
int main() {  
  int a = 0;  
  int i = 0.5; // debe dar error porque es entero  
  float p = 0.5;  
  int d = 0;  
  int d=0; //debe dar error porque ya fue declarada  
  
  for (a = 0; a < 3; a++) {  
    i++;  
    d = i;  
  }  
  d=0.5; // debe dar error porque es entera  
  
}  
