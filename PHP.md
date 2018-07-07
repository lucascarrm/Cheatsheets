# PHP CHEATSHEET

Manejate con la Tabla de contenidos  o apretra **CTRL+F**
# Tabla de contenidos
- [Tabla de contenidos](#tabla-de-contenidos)
    - [Cosas importantes](#cosas-importantes)
        - [Mostrar algo en la pag con php](#mostrar-algo-en-la-pag-con-php)
        - [Concatenar strings](#concatenar-strings)
        - [Foreach](#foreach)
        - [Hacer referencia a un archivo](#hacer-referencia-a-un-archivo)
        - [Saber si un elemento de un array existe](#saber-si-un-elemento-de-un-array-existe)
        - [La puta hora](#la-puta-hora)
        - [Eliminar de un string espacios](#eliminar-de-un-string-espacios)
        - [Cortar un string a un array eliminando el/los caracteres que queremos](#cortar-un-string-a-un-array-eliminando-ellos-caracteres-que-queremos)
    - [Clases Normales](#clases-normales)
        - [Definir una clase](#definir-una-clase)
        - [Visibilidad](#visibilidad)
        - [Definir constructor](#definir-constructor)
        - [Funciones estaticas](#funciones-estaticas)
        - [Llamar funciones estaticas](#llamar-funciones-estaticas)
        - [Llamar funciones](#llamar-funciones)
        - [Parametros por defecto](#parametros-por-defecto)
        - [Retornos de funcion](#retornos-de-funcion)
    - [Clases Abstractas](#clases-abstractas)
        - [Definir clase abstracta](#definir-clase-abstracta)
    - [Interfaces](#interfaces)
        - [Definir interfaz](#definir-interfaz)
        - [Implementar interfaces](#implementar-interfaces)
    - [Herencia](#herencia)
        - [Implementar herencia](#implementar-herencia)
    - [Arrays](#arrays)
        - [Crear array indexados sin clave](#crear-array-indexados-sin-clave)
        - [Crear array indexados con clave](#crear-array-indexados-con-clave)
        - [Mostrar valores de array](#mostrar-valores-de-array)
        - [Acceder a array](#acceder-a-array)
        - [Mostrar valores de array](#mostrar-valores-de-array)
        - [Añadir elementos al array](#a%C3%B1adir-elementos-al-array)
        - [Eliminar elementos del array](#eliminar-elementos-del-array)
        - [Cuantos elementos tiene el array](#cuantos-elementos-tiene-el-array)
        - [Buscar elementos en array](#buscar-elementos-en-array)
    - [Archivos](#archivos)
        - [Abrir archivo](#abrir-archivo)
        - [Cerrar archivo](#cerrar-archivo)
        - [Escribir en archivo (Modo lectura w , a)](#escribir-en-archivo-modo-lectura-w--a)
        - [Leer de archivo linea por linea (Modo lectura r)](#leer-de-archivo-linea-por-linea-modo-lectura-r)
        - [Ripear un archivo (eliminarlo hehe)](#ripear-un-archivo-eliminarlo-hehe)
        - [Mover un archivo y renombrarlo si es lo que se busca (lo mas rompehuevos del mundo)](#mover-un-archivo-y-renombrarlo-si-es-lo-que-se-busca-lo-mas-rompehuevos-del-mundo)
            - [Mover un archivo subido desde el cliente](#mover-un-archivo-subido-desde-el-cliente)

## Cosas importantes

#### Mostrar algo en la pag con php
```
echo 'Hola mundo'
```
#### Concatenar strings
```
Se usa el operador '.' Ej:
"hola" . "mundo";
```

#### Foreach
```
foreach($array as $elemento)
```

#### Hacer referencia a un archivo
```
require_once('archivo.php');
require_once 'archivo.php';
```

#### Saber si un elemento de un array existe
```
isset($array['algo'])
isset($_POST['algo_2']
```

#### La puta hora
```
date("his"); // Horas minutos segundos
date("mdy"); // Mes dia año
```

#### Eliminar de un string espacios
```
trim('Hola  ahre') // Holaahre
```
#### Cortar un string a un array eliminando el/los caracteres que queremos
```
explode('-',"Hola-Lucas") // ['Hola','Lucas']
```


## Clases Normales

#### Definir una clase

```
class Persona {} 
```

#### Visibilidad
``` private $variable_1;
protected $variable_2;
public $variable_3;
```

#### Definir constructor
``` 
public function __construct($nombre){
$this->_nombre=$nombre;
} 
```

#### Funciones estaticas
```
public static function HaceAlgo(){}
```

#### Llamar funciones estaticas
```
Clase::HaceAlgo();
```

#### Llamar funciones
```
MiObjeto->HaceAlgo();
```

#### Parametros por defecto
```
public function HaceAlgo($variable=1){}
```

#### Retornos de funcion
No es necesario indicar que tiene que retornar la funcion solo hacelo.
``` 
public function RetornaAlgo(){
    return $algo;
}
```

## Clases Abstractas

#### Definir clase abstracta
``` 
abstract class ClaseAbstracta{
    abstract protected function getValor();
    abstract public function valorPrefijo($prefijo);
    // OJO EN LAS CLASES ABSTRACTAS PUEDEN HABER METODOS COMUNES.
}
```

## Interfaces

#### Definir interfaz
``` 
interface IVendible{
    public function PrecioMasIva();
}
```

#### Implementar interfaces
```
class Clase implements Interfaz{}
```

## Herencia

#### Implementar herencia
```
class Clase extends Hijo{}
```

## Arrays

#### Crear array indexados sin clave
```
$array = array("hello", "world");
```

#### Crear array indexados con clave
```
 array(
    clave  => valor,
    clave2 => valor2,
    clave3 => valor3,
    );
```

#### Mostrar valores de array
```
var_dump($array);
```

#### Acceder a array
```
$arr[clave];
```

#### Mostrar valores de array
```
var_dump($array);
```

#### Añadir elementos al array
```
$arr[8]='algo';

array_push($array, "algo1", "algo2", ...);
```

#### Eliminar elementos del array
```
unset($arr[4])
```

#### Cuantos elementos tiene el array
```
count($array) // Devuelve el ultimo indice + 1
```

#### Buscar elementos en array
```
array_search($elemento,$array); //  Devuelve true o false
```

## Archivos

#### Abrir archivo
```
$archivo=fopen('path.txt',"w"); // Modos de lectura: w r a (Intenten no usar w+)
```

#### Cerrar archivo
```
fclose($archivo);
```

#### Escribir en archivo (Modo lectura w , a)
```
fwrite($archivo,'algo'); 
```

#### Leer de archivo linea por linea (Modo lectura r)
```
 while(!feof($archivo))
        {
           $stringArchivo=fgets($archivo);
           //Yo suelo usar esta de abajo
           //$arrayHelado=explode("-",fgets($archivo));
        }

```

#### Ripear un archivo (eliminarlo hehe)
```
unlink($path); 
```

#### Mover un archivo y renombrarlo si es lo que se busca (lo mas rompehuevos del mundo)
```
rename("/img/lolis.txt", "/script/nosonlolis.txt");
```

#### Mover un archivo subido desde el cliente
```
move_uploaded_file($_FILES['foto']['tmp_name'], $path);
```
