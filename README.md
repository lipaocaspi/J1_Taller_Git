# Taller Alias Git

1. Está trabajando en un proyecto Git colaborativo con varias ramas y commits. Tu tarea es utilizar el comando git log con algunas opciones específicas para obtener un resumen gráfico de los últimos 5 commits en todas las ramas.

   ```
   git config --global alias.lastFive "log --all --decorate --oneline --graph -n 5"
   ```

   * **--all** : muestra el registro de todas las ramas.

   * **--decorate** : muestra los nombres de las ramas y las etiquetas junto a los commits.

   * **--oneline** : muestra cada commit en una sola línea.

   * **--graph** : muestra una representación gráfica del historial de commits con líneas que indican bifurcaciones y fusiones.

   * **-n 5** : limita la salida a los últimos 5 commits.

     

2. Está trabajando en un proyecto Git colaborativo y necesitas obtener una visión gráfica y detallada del historial de commits. Tu tarea es utilizar el comando git log con opciones específicas para personalizar el formato y presentación de la salida. La salida debe tener las siguientes especificaciones:

   * Muestra una representación gráfica del historial de commits.

   * Muestra el hash corto del commit en color rojo.

   * Muestra las referencias (ramas o tags) en las que está involucrado el commit en color amarillo.

   * Muestra el mensaje del commit.

   * Muestra la fecha relativa del commit en color verde.

   * Muestra el hash del commit como un identificador abreviado.

   * Muestra las fechas de los commits de forma relativa.

     ```
     git config --global alias.graphDetail "log --graph --abbrev-commit --decorate --format=format:'%C(bold red)%h%C(reset) - %C(bold green) (%ar)%C(reset) - %C(white)%s%C(reset) - %C(dim white)-%an%C(reset) - %C(bold yellow)%d%C(reset)' --all"
     ```

     

3. Estás trabajando frecuentemente con el comando git log -1 HEAD para obtener detalles sobre el último commit en la rama actual. Sin embargo, encuentras que escribir este comando completo es un poco tedioso. Quieres simplificarlo creando un alias personalizado.

   Tu tarea es utilizar el comando git config para crear un alias llamado last que represente el comando git log -1 HEAD.

   ```
   git config --global alias.last "log -1 HEAD"
   ```

   * **-1** : limita la salida a un solo commit (el último).
   * **HEAD** : especifíca la rama actual.

4. Imagina que deseas simplificar el proceso de editar la configuración global de Git. Tu tarea es utilizar el comando git config para crear un alias que te permita abrir facilmente la configuración global de tu editor de texto preferido. Ejecuta el comando para crear un alias llamado ec que cumpla con la especificación dada.

   ```
   
   ```

   

5. Imagina que estás trabajando en un proyecto Git colaborativo con múltiples colaboradores y ramas. Tu tarea es utilizar el comando git log con opciones específicas para personalizar la salida del historial del commits y resaltar información clave. El resultado de la ejecución del comando se debe ver como el ejemplo siguiente:

   ![](https://raw.githubusercontent.com/lipaocaspi/J1_Taller_Git/main/resultadoEj05.png)

   ```
   
   ```
