#Readme Uploader

El objetivo de este script es 
automatizar el proceso de subir el progreso
de freecodecamp a mi github
El lenguaje usado es python pues es optimo
para trabajar con carpetas y textos
(y porque es el único que sé usar además de JS)
>> cabe resaltar que JS no sirve para este caso porque requiere node y es mucho trabajo (soy un poco vago)

## El programa debe funcionar de la siguiente manera:
### requerimientos
- los ejercicios de freecode serán descargados
en formato json y se almacenaran en un directorio
denominado "inputDir"
- los ejercicios deben ser leídos en json y escritos en el formato requerido 
el cual bien puede ser html o js
- los archivos de los ejercicios ya convertidos deben ser almacenados en un directorio de salida llamado "outputDir"
- los elementos de outputDir deben ser append a la carpeta requerida, bien puede ser carperta de ejercicios js o ejercicios html
>> nota: por lo pronto no se tiene en cuenta jerarquía de carpeta u otras opciones de taggeo y subcategorización de directorios.
### procesos
1. Iterar los archivos de inputDir y guardaros en un diccionario llamado inputFiles usando el método json.loads()
2. Agregar cada archivo json como un par clave valor del diccionario.
3. Eliminar cada archivo del inputDir una vez cargado en memoria (esto puede dar problemas, supongo)
4. Iterar el diccionario y crear un archivo HTML o JS según prompt.
5. if inputDir ir empty, salir del programa y proceder con commit & push.

El archivo inicial será "input.py"
El primer commit será crear el iterador de la inputFolder con print por cada clave. 