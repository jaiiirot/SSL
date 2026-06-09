# TP0
COMPILACION Y EJECUCION:
1. Compilar en MINGW64: gcc -o hello hello.c
2. Ejecutar en MINGW64: ./hello
 
TEORIA:
- printf(): Función que imprime texto en la consola
- __STDC_VERSION__: Macro que devuelve el estándar C utilizado (ej: 201112L para C11)
- %ld: Especificador de formato para long int
- return 0: Indica que el programa finalizó exitosamente
- En Windows, el ejecutable generado suele ser .exe
 
FUNCIONES UTILIZADAS:
1. printf(const char *format, ...):
   USO: Imprime texto formateado en la salida estándar (consola)
   PARA QUE: Mostrar mensajes y valores al usuario. Acepta especificadores de formato
             como %d (int), %ld (long), %s (string), \n (salto de línea)
   RETORNA: Número de caracteres impresos
 
2. main(void):
   USO: Función principal del programa, punto de entrada
   PARA QUE: Todo programa en C debe tener una función main() que se ejecuta al iniciar
   RETORNA: int (0 = éxito, otro valor = error)

**Publicación**
Publique el trabajo en el repositorio personal `SSL` la carpeta `00-CHelloWorld` con `readme.md`, `hello.c`, y `output.txt`.

CREAR `output.txt`:
- Desde MINGW64/Linux: ejecutar el programa y redirigir la salida:
   ./hello > output.txt
- En Windows (PowerShell o CMD) si compiló a hello.exe:
   hello.exe > output.txt
- Alternativamente crear un archivo vacío manualmente:
   - En CMD: type nul > output.txt
   - En PowerShell: New-Item -Path output.txt -ItemType File
   - En un editor de texto, crear y guardar como `output.txt`.
 