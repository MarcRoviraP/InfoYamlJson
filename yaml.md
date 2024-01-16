# Índice   
1. [YAML](#id1)
2. [JSON](#id2)


# YAML<a name="id1"></a>

## ¿Qué es YAML?
>[!Tip]
>
>**YAML** es un lenguaje de serialización de datos que las personas pueden comprender y suele utilizarse en el diseño de archivos de configuración. Para algunas personas, **YAML** significa otro lenguaje de marcado más, 
>para otras, es un acrónimo recursivo que quiere decir _"YAML no es un lenguaje de marcado"_, lo que enfatiza la idea de que se utiliza para los datos, no para los documentos. 



## Sintaxis de YAML

**YAML** utiliza una extensión de archivos **.yml* o **.yaml* y sigue reglas de sintaxis específicas. 

Este es un **ejemplo** muy básico de un archivo YAML:
```

#Comentario: esta es una lista de supermercado que utiliza YAML 
 
#Nota - el carácter representa la lista --- comida: - vegetales: tomates 
 
#primer elemento de la lista - frutas: #segundo elemento de la lista cítricos: naranjas tropicales: bananas nueces: maní dulces: pasas
  ```

## Etiquetas en YAML
El fichero YAML permite diferentes etiquetas, como por ejemplo:

+ **Nombre**: indica el nombre de la tarea a realizar. Se puede dar cualquier nombre lógico al archivo del codigo yaml
+ **Hosts*: este campo es obligatorio y se encarga de especificar las listas o grupos de hosts sobre los que el usuario quiere ejecutar una tarea. Es posible que las tareas se ejecuten en una misma máquina, un equipo remoto o incluso en varios dispositivos, por lo que la etiqueta de hosts también puede tener una entrada de grupo.
+ **Vars**: esta etiqueta permite definir las variables a usar en la lista de tareas.
+ **Tasks**: contiene la lista de tareas a ejecutar y funciona como una hoja de ruta o texto de ayuda para el usuario. Aunque no es obligatorio, este campo es de gran utilidad para los usuarios, especialmente en lo que respecta a la depuración de la task list.

  ![Image yaml](https://github.com/MarcRoviraP/InfoYamlJson/blob/main/img/yaml.png)

# JSON<a name="id2"></a>
## Que es JSON?
>[!Tip]
>**JSON** es un formato de texto que forma parte del sistema de *JavaScript* y que se deriva de su sintaxis, pero no tiene como objetivo la creación de programas, sino el acceso, almacenamiento e intercambio de datos.
>
>Usualmente es conocido como una alternativa al lenguaje **XML**.

## Sintaxis de JSON
+ El arreglo de información se hace mediante claves (keys).
+ La información se separa por comas.
+ Las llaves agrupan objetos.
+ Los corchetes agrupan arreglos de datos.
Sin embargo, **JSON** se distingue de *JavaScript* porque sus claves tienen que ser **strings** (o secuencias de caracteres), mientras que sus valores deben ser strings, números, objetos, arreglos, boleados o null.

## Ejemplos de archivos JSON

Estos son algunos de los ejemplos de JSON

### Strings
En JSON los strings siempre deben ir entre comillas dobles y la key debe ser una secuencia de caracteres:
```
{“Nombre”:“Juan”};
```
### Números

En el caso de los números, estos siempre deberán ser enteros o decimales:
```
{“Edad”:“30”}
```
### Objetos
Por su parte, cuando asignamos objetos a un valor necesitamos emplear signos de llave para contener la información del conjunto. La información contenida debe mantener el mismo formato, lo que da una apariencia mucho más simple y limpia:
```
{“Empleado”:{“Nombre”:“Juan”, “Edad”:“30”, “Ciudad”:“Madrid”}}
```
### Arreglos
Los arreglos deben ingresarse de una forma bastante similar al formato y sintaxis de los strings y números. La única diferencia radica en que no utilizaremos signos de llaves, sino corchetes, para contener los datos:
```
{“Empleados”:[“Juan”, 30, “Pedro”]}
```
### Booleanos
Los valores booleanos se utilizan cuando la información solo puede ser verdadera (true) o falsa (false). Por ejemplo, cuando una venta ha sido concretada o se requiere autenticación:
```
{“Venta”:true}
```
### Null
Null es una expresión única que identifica una key a la que aún no se le asigna un valor, pero que no está vacía. Típicamente se emplea para reconocer la falta de valor, por lo que, así como los booleanos, da como resultado null cuando no hay un contenido y datos cuando sí los hay:
```
{“Apellido”:null}
```
 ![Image JSON](https://github.com/MarcRoviraP/InfoYamlJson/blob/main/img/json.png)

## Bibliografia
>[!Important]
>https://www.redhat.com/es/topics/automation/what-is-yaml
>
>https://keepcoding.io/blog/que-es-y-para-que-sirve-el-fichero-yaml/
>
>https://blog.hubspot.es/website/que-es-json
>
>https://www.nextu.com/blog/que-es-json-por-que-es-importante-conocerlo-rc22/
>
