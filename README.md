# TP_ArquitecturaWeb

Nombre del grupo: Alquilando

Integrantes: Mariano Falcón

Descripción del negocio elegido: Es una web que permite por un lado subir información sobre departamentos a alquilar por localidad y por otro reservar y/o alquilar el departamento. Los usuarios deben estar logueados para poder realizar las acciones mencionadas. La búsqueda de departamentos puede filtrarse con: cantidad de ambientes, metros cuadrados, piso del departamento, cantidad de días máximos y mínimos de alquiler, si está reservado/disponible o no, equipamentos (S/N) como utensillos de cocina, lavaropas, etc.


Endpoints:

/usuarios                                   -> static
/usuarios/Y                                 -> static
/localidades                                -> static
/localidades/Y                              -> static
/localidades/Y/departamentos                -> static
/localidades/Y/departamentos/X              -> static
/localidades/Y/departamentos/X/imagenes     -> static
/localidades/Y/departamentos/X/imagenes/Z   -> static
/ingresar                                   -> api
/crearCuenta                                -> api
/localidades/Y/buscar                       -> api


Métodos

GET /usuarios - devuelve una lista de los usuarios

GET /usuarios/Y - devuelve al usuario “Y”
PUT /usuarios/Y - actualiza al usuario “Y”
PATCH /usuarios/Y - actualiza parcialmente al usuario “Y”
DELETE /usuarios/Y - elimina la usuario “Y”

GET /ingresar - api que permite el ingreso a la cuenta de usuario
GET /crearCuenta - api que permite crear un nuevo usuario

GET /localidades - devuelve una lista de las localidades
POST /localidades - crea una nueva localidad

GET /localidades/Y - devuelve la localidad “Y”
PUT /localidades/Y - actualiza la localidad “Y”
PATCH /localidades/Y - actualiza parcialmente la localidad “Y”
DELETE /localidades/Y - elimina la localidad “Y”

GET /localidades/Y/departamentos - devuelve una lista de los departamentos en la localidad “Y”
POST /localidades/Y/departamentos - crea un nuevo departamento

GET /localidades/Y/departamentos/X - devuelve el departamento “X” de la localidad “Y”
PUT /localidades/Y/departamentos/X - actualiza el departamento “X” de la localidad “Y”
PATCH /localidades/Y/departamentos/X - actualiza parcialmente el departamento “X” de la localidad “Y”
DELETE /localidades/Y/departamentos/X - elimina el departamento “X” de la localidad “Y”
GET /localidades/Y/departamentos/X/imagenes - devuelve una lista de las imagenes del departamento “X” en la localidad “Y”
POST /localidades/Y/departamentos/X/imagenes - crea una imagen del departamento “X” en la localidad “Y”

GET /localidades/Y/departamentos/X/imagenes/Z - devuelve la imagen “Z” del departamento “X” de la localidad “Y”
DELETE /localidades/Y/departamentos/X/imagenes/Z - elimina la imagen “Z” del departamento “X” de la localidad “Y”

GET /localidades/Y/buscar - api que da herramientas para la búsqueda de departamentos
