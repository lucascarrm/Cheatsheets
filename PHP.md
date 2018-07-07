# ❤️ PHP CHEATSHEET ❤️

## Modelos de parcial que te pueden servir
 [Modelo parc 2 TOTO](https://github.com/tomasmattia/proyecto.aprobar.lab/tree/master/proyecto.aprobar.prog/backend.1) 👅👄💧

 [Modelo parc 2 Lucas](https://github.com/lucascarrm/Program-y-lab3/tree/master/ProgramacionBackEnd/ParcialesFinales/Modelo_Parc_2)

 [Parcial 2 REAL + PDFs](https://github.com/lucascarrm/Program-y-lab3/tree/master/ProgramacionBackEnd/ParcialesFinales/Parc_2)

 ⚡️ Manejate con la Tabla de contenidos  o apretra **CTRL+F** ⚡️
# Tabla de contenidos
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Cosas importantes](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-cosas-importantes)
    - [Mostrar algo en la pag con php](#mostrar-algo-en-la-pag-con-php)
    - [Concatenar strings](#concatenar-strings)
    - [Foreach](#foreach)
    - [Hacer referencia a un archivo](#hacer-referencia-a-un-archivo)
    - [Saber si un elemento de un array existe](#saber-si-un-elemento-de-un-array-existe)
    - [La puta hora](#la-puta-hora)
    - [Eliminar de un string espacios](#eliminar-de-un-string-espacios)
    - [Cortar un string a un array eliminando el/los caracteres que queremos](#cortar-un-string-a-un-array-eliminando-ellos-caracteres-que-queremos)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Clases Normales](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-clases-normales)
    - [Definir una clase](#definir-una-clase)
    - [Visibilidad](#visibilidad)
    - [Definir constructor](#definir-constructor)
    - [Funciones estaticas](#funciones-estaticas)
    - [Llamar funciones estaticas](#llamar-funciones-estaticas)
    - [Llamar funciones](#llamar-funciones)
    - [Parametros por defecto](#parametros-por-defecto)
    - [Retornos de funcion](#retornos-de-funcion)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Clases Abstractas](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-clases-abstractas)
    - [Definir clase abstracta](#definir-clase-abstracta)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Interfaces](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-interfaces)
    - [Definir interfaz](#definir-interfaz)
    - [Implementar interfaces](#implementar-interfaces)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Herencia](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-herencia)
    - [Implementar herencia](#implementar-herencia)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Arrays](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-arrays)
    - [Crear array indexados sin clave](#crear-array-indexados-sin-clave)
    - [Crear array indexados con clave](#crear-array-indexados-con-clave)
    - [Mostrar valores de array](#mostrar-valores-de-array)
    - [Acceder a array](#acceder-a-array)
    - [Mostrar valores de array](#mostrar-valores-de-array)
    - [Añadir elementos al array](#a%C3%B1adir-elementos-al-array)
    - [Eliminar elementos del array](#eliminar-elementos-del-array)
    - [Cuantos elementos tiene el array](#cuantos-elementos-tiene-el-array)
    - [Buscar elementos en array](#buscar-elementos-en-array)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Archivos](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-archivos)
    - [Info de un archivo](#info-de-un-archivo)
    - [Abrir archivo](#abrir-archivo)
    - [Cerrar archivo](#cerrar-archivo)
    - [Escribir en archivo (Modo lectura w , a)](#escribir-en-archivo-modo-lectura-w--a)
    - [Leer de archivo linea por linea (Modo lectura r)](#leer-de-archivo-linea-por-linea-modo-lectura-r)
    - [Ripear un archivo (eliminarlo hehe)](#ripear-un-archivo-eliminarlo-hehe)
    - [Mover un archivo y renombrarlo si es lo que se busca (lo mas rompehuevos del mundo)](#mover-un-archivo-y-renombrarlo-si-es-lo-que-se-busca-lo-mas-rompehuevos-del-mundo)
    - [Mover un archivo subido desde el cliente](#mover-un-archivo-subido-desde-el-cliente)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> PDO](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-pdo)
    - [Crear objeto de la DB](#crear-objeto-de-la-db)
    - [Preparar sentencia PDO](#preparar-sentencia-pdo)
    - [Ejecutar sentencia](#ejecutar-sentencia)
    - [Excepciones](#excepciones)
    - [Agarrar elementos de la DB](#agarrar-elementos-de-la-db)
    - [Saber si se pudo ejecutar la consulta a la DB despues de ejecutar](#saber-si-se-pudo-ejecutar-la-consulta-a-la-db-despues-de-ejecutar)
    - [Bindear valores en la consulta](#bindear-valores-en-la-consulta)
    - [Como acceder a los objetos que deja fetch](#como-acceder-a-los-objetos-que-deja-fetch)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> REST API](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-rest-api)
    - [Acceder a los parametros de la api](#acceder-a-los-parametros-de-la-api)
    - [Retornar un JSON con codigo de estado](#retornar-un-json-con-codigo-de-estado)
    - [Ruta opcional](#ruta-opcional)
    - [Ruteo con params](#ruteo-con-params)
    - [Mapeo de verbos para ruta](#mapeo-de-verbos-para-ruta)
    - [Entrar a ruta con cualquier verbo](#entrar-a-ruta-con-cualquier-verbo)
    - [Grupos con ruta adentro](#grupos-con-ruta-adentro)
    - [Verificar si se entro por tal verbo](#verificar-si-se-entro-por-tal-verbo)
    - [Mostrar por que verbo se entro](#mostrar-por-que-verbo-se-entro)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> JWT](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-jwt)
    - [Crear JWT](#crear-jwt)
    - [Verificar o acceder a JWT](#verificar-o-acceder-a-jwt)
    - [Acceder a elementos de JWT](#acceder-a-elementos-de-jwt)
- [<img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Middlewares](#img-src%22httpsimageflaticoncomiconssvg426426833svg%22-width%2220%22-middlewares)
    - [Pasar de middleware a proxima funcion](#pasar-de-middleware-a-proxima-funcion)
    - [Poner middleware con metodo de clase](#poner-middleware-con-metodo-de-clase)
    - [Poner varios middlewares](#poner-varios-middlewares)

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Cosas importantes

#### Mostrar algo en la pag con php
```
echo 'Hola mundo'
```
#### Concatenar strings
```
// Se usa el operador '.' Ej:
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


## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Clases Normales

#### Definir una clase

```
class Persona {} 
```

#### Visibilidad
``` 
private $variable_1;
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
``` 
// No es necesario indicar que tiene que retornar la funcion solo hacelo.
public function RetornaAlgo(){
    return $algo;
}
```

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Clases Abstractas

#### Definir clase abstracta
``` 
abstract class ClaseAbstracta{
    abstract protected function getValor();
    abstract public function valorPrefijo($prefijo);
    // OJO EN LAS CLASES ABSTRACTAS PUEDEN HABER METODOS COMUNES.
}
```

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Interfaces

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

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Herencia

#### Implementar herencia
```
class Clase extends Hijo{}
```

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Arrays

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
// o podes usar
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

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Archivos

#### Info de un archivo
```
$archivoInfo = pathinfo($_FILES['foto']['name']);
// Se puede acceder a la extension asi
$archivoInfo['extension'];
```

#### Abrir archivo
```
$archivo=fopen('path.txt',"w"); // Modos de lectura: w r a (Intenten no usar w+)
```

#### Cerrar archivo
```
fclose($archivo); // acordate de cerrar hdp
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
           // Yo suelo usar esta de abajo
           // $arrayHelado=explode("-",fgets($archivo));
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

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> PDO

#### Crear objeto de la DB
```              
$objetoPDO = new PDO('mysql:host=localhost;dbname=juansitodb;charset=utf8', $usuario, $pass);
                                                  'NOMBRE DB'
```

#### Preparar sentencia PDO
```
$sql = $objetoPDO->prepare('SELECT * FROM `db`');
```

#### Ejecutar sentencia
```
$sql->execute();
```

#### Excepciones
```
   catch (PDOException $e) {
        echo $e->getMessage();
   }
```

#### Agarrar elementos de la DB
```
  while ($result = $sql->fetchObject()) {
        var_dump($result);
  }
```

#### Saber si se pudo ejecutar la consulta a la DB despues de ejecutar
```
  if ($sql->rowCount()) {}
  // O tambien se puede usar este
  // if($sql->fetch())
```

#### Bindear valores en la consulta
```
  // Hacemos  una consulta a la DB asi
  // 'DELETE FROM `productos` WHERE `id`=:id'
  // Despues de  prepararla hacemos esto:
  $sql->bindValue(':id', $id);
```

#### Como acceder  a los objetos que deja fetch
```
  $result = $sql->fetch();
  $result['nombre'];
  $result2= $sql->fetchObject();
  $result2->nombre;
```

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> REST API

#### Acceder a los parametros de la api
```
   $parametros = $request->getParsedBody();
```

#### Retornar un JSON con codigo de estado
```
   return $response->withJson(['clave' => 'valor'],200);
```

#### Ruta opcional
```
   $app->get('/ruteo/{param}', function (Request $request, Response $response, $args) {
        $params = $args['param'];
});
```
#### Ruteo con params
```
   Se pone con '[/]' ejemplo de otras  rutas /entrar[/]
});
```

#### Mapeo de verbos para ruta
```
  app->map(['POST', 'GET'], '/ruta', function (Request $request, Response $response, $args) {
  });
```

#### Entrar a ruta con cualquier verbo
```
  $this->any('/ruta', function (Request $request, Response $response, $args) {});
```

#### Grupos con ruta adentro
```
   $app->group('/login', function () {
    $this->post('[/]', function (Request $request, Response $response) {
    });
```

#### Verificar si se entro por tal verbo
```
   $request->isDelete()
   // isPost , isGet ...
```

#### Mostrar por que verbo  se entro
```
   $request->getMethod();
```

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> JWT

#### Crear JWT
```
        $key = "llave";
        $fecha = time();
        $payload = array(
            "email" => $params['email'],
            "clave" => $params['clave'],
            "iat" => $fecha,
            "exp" => $fecha+20000
        );
        $jwt = JWT::encode($payload, $key);
        $objRetorno = new stdClass();
        $objRetorno->jwt = $jwt;
        return $response->withJson($objRetorno,200);
```
#### Verificar o acceder a JWT
```
        $elToken= $request->getHeader('miToken');
        try
        {
            $jwtDecode = JWT::decode($elToken[0],'llave',array('HS256'));
            return $response->withJson(["mensaje" => 'token valido'],200);
        }
        catch(Exception $e)
        {
            return $response->withJson(["mensaje"=>"token invalido"],409);
        }
```
#### Acceder a elementos de JWT
```
        // Siempre usen catch(Exception $e) pls
        $jwtDecode = JWT::decode($elToken[0],'llave',array('HS256'));
        $jwtDecode->clave; 
```

## <img src="https://image.flaticon.com/icons/svg/426/426833.svg" width="20"> Middlewares 

#### Pasar de middleware a proxima funcion
```
   $response=$next($request,$response);
```
#### Poner middleware con metodo de clase
```
    ->add(\Middlewares::class.":VerificarSeteados"); // Se usa ':' para metodo de instancia y  // '::' para estatico
```
#### Poner varios middlewares
```
   ->add(\Middlewares::class.":VerificarBD") // Este se ejecuta ultimo
    ->add(\Middlewares::class."::VerificarVacios")
    ->add(\Middlewares::class.":VerificarSeteados"); // Este se ejecuta primero
```

