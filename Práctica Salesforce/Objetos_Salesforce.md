# Datos en Salesforce

Salesforce almacena sus datos en tablas relacionales. Los registros contienen la información de la plataforma además de los datos creados por usuarios. También se pueden crear tablas personalizadas para almacenar información especifica de cada negocio.

Estas tablas relacionales son referenciadas como Objetos API u Objetos en Salesforce. Hay 3 tipos de objetos:

+ Objetos estándar: Los objetos creados por la plataforma Salesforce.
+ Objetos personalizados: Son los objetos creados en función a la estructura de negocio
+ Objetos externos: Son los objetos que se asignan para gestionar los datos externos a la empresa.

# Objetos Estándar

Estos son los objetos que ya existen en la plataforma Salesforce para administrar las configuraciones y los ajustes del entorno. Una vez que inicies sesión en la plataforma de Salesforce, podrás ver los objetos disponibles.

>**Ejemplo:**
>
>El objeto estándar más comúnmente mencionado se denomina Account Object *(objeto de cuenta)*. Es el objeto que almacena la información preliminar sobre un cliente, socio, competidor u otra organización. 

Podemos explorar el objeto de cuenta siguiendo los pasos a continuación.

### Paso 1

Haz login en Salesforce y accede al Schema Builder: Para ello accede Objetos y Campos -> Generador de Esquemas 

### Paso 2

Podrás ver todos los esquemas, nos fijaremos concretamente en el Account o Cuenta. Ahi podrás ver todos los elementos que forman parte del Objeto Cuenta de Salesforce

## Objetos importantes

|Nombre del objeto|Significado|Uso|
|-|-|-|
|**Cuenta**|Representa una cuenta individual, la cual puede ser un particular involucrado en las actividades de una empresa o un negocio|Este objeto es utilizado para listar y organizar cuentas dentro de una organización |
|**Historial de Cuenta**|Representa el historial de cambios a los valores de los campos de una cuenta|Este objeto es utilizado para identificar los cambios a una cuenta |
|**Caso**|Representa un caso, es decir, un problema o fallo de un cliente|Este objeto es utilizado para gestionar los casos de una organización |
|**Contacto**|Representa un contacto, es decir, un individuo asociado a una cuenta|Este objeto es utilizado para gestionar los contactos |
|**Usuario**|Representa un usuario dentro de una organización|Este objeto es utilizado obtener información sobre los usuarios y ayudar a proveer y modificar la información relacionada con los mismos  |
|**Asset**|Representa un asset, es decir, un objeto con valor comercial como un producto vendido por una empresa o un competidor que haya comprado e instalado un cliente|Este objeto es utilizado para gestionar y controlar los assets que se han vendido previamente a los clientes. Por medio de este control, una aplicación del cliente puede determinar previamente que productos han sido vendidos o están instalados en una cuenta especifica|
|**Dominio**|Es un objeto de solo lectura que representa una Web personalizada asignada a una organización|Este objeto es utilizado para obtener los dominios que están asociados con cada página web dentro de una organización|

# Objetos Personalizados

También podemos crear objetos personalizados, para ello simplemente tendremos que entrar en el Gestor de Objetos y clicar el botón en la esquina superior derecha Crear, entonces se nos pedirán todos los campos obligatorios para la creación del objeto. 

Para crear un nuevo campo, accede a Campos y Relaciones y desde ahi, con el boton Nuevo podrás crear un nuevo campo indicando todas las propiedades.

# Relaciones

Las relaciones entre en objetos son soportadas mediante el Campo Relaciones, el cual es un campo personalizado que se encarga de vincular un objeto a otro.

## Relación Master-Detail 

La Relación Master-Detail se utiliza cuando queremos controlar la visualización de registros en función del valor del registro maestro. Por ejemplo, en un modelo de una empresa de mensajería, una entrega siempre está vinculada a un destino. Si eliminamos una ubicación de entrega de nuestra lista, también se eliminarán todos las entregas relacionadas. 

**Características**

+ Al eliminar un registro maestro, se eliminan todos los registros de detalle.

+ No se puede crear un registro de detalle sin un registro maestro.

+ No se puede establecer el permiso en el registro de detalle. Hereda el permiso del registro maestro.

+ El registro de detalle también hereda la regla de uso compartido de los registros maestros.

+ Tanto los registros maestros como los de detalle se incluyen automáticamente en los tipos de registro del informe.

## Relación de Búsqueda

Una relación de búsqueda implica encontrar el valor de un campo en función del valor de otro campo en otro objeto. Se utiliza principalmente en el caso de datos compartidos entre dos objetos.
