
# DDL (Lenguaje de definicón de datos)

#### Pequeña definición:
Es un subconjunto de SQL usado para **definir y gestionar la estructura** de la base de datos. Se usa para: 
- Crear bases de datos, tablas, índices y relaciones.
- Modificar estructuras existentes (agregar o cambiar columnas, restricciones, etc.).
- Eliminar estructuras cuando ya no se necesitan.

## Creando base de datos

 CREATE DATABASE 'nombreBDD';

## Creando Usuario y otorgar permisos 

CREATE USER 'usuario'@'localhost' IDENTIFIED BY 'contraseña';
GRANT ALL PRIVILEGES ON 'nombreBDD' TO 'usuario'@'localhost';

## Creando Tablas dentro de una bdd 


USE 'nombreBDD'; -- para usar la base de datos


CREATE TABLE nombretabla(
clavePrimaria INT PRIMARY KEY AUTO_INCREMENT,
ColumnaNumerica INT,
ColumnaChar VARCHAR(100),
ColumnaEsencial INT NOT NULL,
ColumnaUnica INT UNIQUE;
claveForanea INT,
FOREIGN KEY (claveForanea) REFERENCES otraTabla (claveForanea)
);

CREATE TABLE otraTabla(
INT claveForanea PRIMARY KEY AUTO_INCREMENT
);

## ÍNDICES (INDEX)

CREATE INDEX nombreIndex ON targetTabla (TargetColumn);
SHOW INDEX FROM targetTable; -- Mostrar indices en la tabla entera
SHOW INDEX FROM targetTable(targetColumn); -- Mostrar indices de una sola columna

## Modificar tablas (ALTER) (Añadir, modificar y eliminar columnas)

ALTER TABLE targetTable ADD COLUMN newColumn datatype;
ALTER TABLE targetTable MODIFY COLUMN targetColumn datatype; 
ALTER TABLE targetTable DROP COLUMN targetColumn;

## Eliminar indices, tablas o bases de datos

DROP INDEX targetIndex ON targetTable;
DROP TABLE IF EXISTS targetTable;
DROP DATABASE IF EXISTS targetDB;

Siempre revisar dependecias entre tablas antes de borrarlas para evitar errores de integridad
# DML (Lenguaje de manipulación de datos)

#### Pequeña definición:
Es un subconjunto de SQL usado para **manipular los datos** que están dentro de las tablas. Se usa para: 
- Insertar nuevos registros.
- Actualizar información existente.
- Eliminar registros de manera controlada.
- Consultar datos con filtros, agrupaciones y uniones.


## Insertar datos

INSERT INTO targetTable (targetColumn) VALUES ('value');

-- Para insertar dos datos en sus respectivas columnas en una linea
INSERT INTO targetTable (charColumn, intColumn) VALUES ('value', _numericValue_);

-- Para insertar muchos datos en una sola linea 
INSERT INTO targetTable (column1, column2, column3) VALUES 
(value1_row1, value2_row1, value3_row1), 
(value1_row2, value2_row2, value3_row2), 
(value1_rowN, value2_rowN, value3_rowN);

## Actualizar datos (UPDATE) 

-- Cambiar columna entera
UPDATE targetTable SET targetColumn = value;

-- Cambio Condicional
UPDATE targetTable SET targetColumn = value WHERE otherColumn = targetValue;
UPDATE targerTavle SET targetColumn = value WHERE condition1 AND condition2 ;

Nota: Mysql reconoce como otros operadores logicos como el OR, XOR, NOT, entre otros.

## ELIMINAR DATOS (DELETE)

-- Eliminar todos los datos de cierta columna
DELETE * FROM targetTable

-- Eliminar condicionalmente (solo un ejemplo)
DELETE FROM targetTable WHERE condition1 OR CONDITION2; 


## CONSULTAR DATOS (SELECT)

-- Muestra tabla entera
SELECT targetTable;

-- Muestra solo las partes condicionadas
SELECT targetTable WHERE conditions;

## USO DE ALIAS PARA COLUMNAS

La notación general es 't.columna' donde, normalmente, se define 't' como el alias de la tabla al escribir 'tabla t' 

### Ejemplo

-- Esta linea selecciona la fila de una tabla cuyo cierto valor de la clave foranea coincide con el valor de las claves primarias/foraneas de las otras tablas, según corresponda

SELECT e.nombres, c.nombre AS curso, a.codigo AS aula
FROM matriculas m
JOIN estudiantes e ON e.id_estudiante = m.id_estudiante
JOIN cursos c ON c.id_curso = m.id_curso
JOIN aulas a ON a.id_aula = c.id_aula;







