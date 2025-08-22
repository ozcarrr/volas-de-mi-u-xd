
### Diccionario de Datos: 





| ENTIDAD | ATRIBUTO  | TIPO DE DATO (OPC) | PK  | FK DE | NULO | DESCRIPCIÓN |
| ------- | --------- | ------------------ | --- | ----- | ---- | ----------- |
| CLIENTE | ATRIBUTO1 |                    |     |       |      |             |
| CLIENTE | ATRIBUTO2 |                    |     |       |      |             |
| PEDIDO  | ATRIBUTO1 |                    |     |       |      |             |
| PEDIDO  | ATRIBUTO2 |                    |     |       |      |             |
| PEDIDO  | ATRIBUTO3 |                    |     |       |      |             |
| ...     |           |                    |     |       |      |             |
|         |           |                    |     |       |      |             |


# EJERCICIO 

### Convertir el MER (clase 3) en un diccionario: 


| ENTIDAD     | ATRIBUTO         | TIPO_DATO     | PK    | NULO  |     | DESC.                                               |
| ----------- | ---------------- | ------------- | ----- | ----- | --- | --------------------------------------------------- |
| PROPIETARIO | NIF              | int           | true  | false |     | Identificador del propietario lol                   |
| PROPIETARIO | NOMBRE Y AP      | var char[30]  | false | false |     | Nombre y apellido del propietario                   |
| PROPIETARIO | TELEFONO         | int           | false | false |     | Telefono de contacto del propietario                |
| PROPIETARIO | DIRECCIÓN        | var char[150] | false | false |     | Dirección de residencia del propietario             |
| PROPIETARIO | EMAIL            | var char[30]  | false | true  |     | Mail del propietario                                |
| VIVIENDA    | COD_VIVIENDA     | int           | true  | false |     | Codigo de la vivienda                               |
| VIVIENDA    | CALLE            | var char[20]  | false | false |     | Calle de la vivienda                                |
| VIVIENDA    | NUMERO           | int           | false | false |     | Numero de la vivienda                               |
| VIVIENDA    | PISO             | int           | false | false |     | Piso de la vivienda                                 |
| VIVIENDA    | CP               | int           | false | false |     | Codigo postal de la vivienda                        |
| VIVIENDA    | POBLACIÓN        | int           | false | false |     | Cantidad de residentes en el sector de la vivienda  |
| VIVIENDA    | DESCRIPCIÓN      | var char[150] | false | false |     | Breve descripcioón de la vivienda y sus alrededores |
| ALQUILER    | FECHA FIRMA      | date          | false | false |     | Fecha de la firma del alquiler                      |
| ALQUILER    | FIANZA           | int           | false | false |     | Pago inicial                                        |
| ALQUILER    | CODIGO_ALQ       | int           | true  | false |     | Codigo del alquilar                                 |
| ALQUILER    | RANGO_FECHA      | date          | false | false |     | Periodo de estadia del alquiler                     |
| ALQUILER    | IMPORTE_MENSUAL  | int           | false | false |     | Pago mensual del alquiler                           |
| ALQUILER    | MISH             | mish          | false | false |     | se estan comiendo al mish                           |
| INQUILINO   | NIF              | int           | true  | false |     | Identificador principal del inquilino               |
| INQUILINO   | NOMBRE_APELLIDOS | var char[50]  | false | false |     | Nombre y apellidos del inquilino                    |
| INQUILINO   | FECHA NACIMIENTO | date          | false | false |     | Fecha de nacimiento del inquilino                   |
| INQUILINO   | DESC/PREF        | var char[150] | false | false |     | Preferencias de vivienda                            |
| INQUILINO   | TELEFONO         | int           | false | false |     | Telefono de contacto                                |



