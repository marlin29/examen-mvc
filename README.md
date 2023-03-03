# examen-mvc
Tenemos los codigos de mvc, en el cual el controlador se encarga de llamar a la vista y al modelo que es el que tiene las funciones del CRUD
Controlador
require 'modelo.php';
require 'vista.php';

Modelo:
require 'bd/conexion_bd.php';
	class Productos extends BD_PDO
	{
		function insertar($nombre, $cant, $precio)
		{
			$this->Ejecutar_Instruccion("insert into productos(nombre,cant,precio) values('$nombre','$cant','$precio')");
			echo '<script>alert("Ha Insertado Correctamente");</script>';
		}
     }
     
