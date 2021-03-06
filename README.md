# CursodeP00PHP

Repo para el Curso de Programación Orientada a Objetos en PHP

# Resumen

La programación orientada a objetos es una forma de programar, un paradigma o una técnica. Los conceptos que aquí aprendiste te servirán en PHP y en otros lenguajes de programación. Recordemos que para programar de esta forma en realidad debemos crear objetos, y un objeto es una instancia de una clase y una clase es el molde. Ejemplo:

Programación orientada a objetos: es la técnica.
PHP: es el lenguaje de programación (donde implementamos la técnica).
Podemos resumir los diferentes conceptos de la siguiente manera:

Herencia: compartir métodos entre clases padres y clases hijas.
Abstracción: significa aislar, separar y sacar.
Polimorfismo: capacidad o virtud que tienen los métodos donde, por ejemplo, un mismo método puede tener diferentes comportamientos y dar diferentes resultados.
Modularidad: este principio básicamente nos ayuda a tener cada vez piezas de código más pequeñas y entendibles, donde cada pieza es un módulo y muchos módulos forman el sistema entero.
Encapsulamiento: un objeto debe estar aislado y ser un módulo natural. Esto se cumple aplicando la protección a las propiedades impidiendo su modificación y básicamente se refiere a controlar el acceso.
Al entender este estilo conseguimos organizar mucho mejor nuestro código agrupando tareas comunes para crear una sola solución y usarla las veces que sean necesarias en nuestro proyecto. Evitamos con esto repetir código y ganamos mucho al dar mantenimiento en el futuro.

Comienza con la palabra reservada class.
El código va entre llaves { }.
La información se guarda en propiedades que pueden ser públicas, privadas o protegidas.
Cada acción la colocamos en métodos que básicamente son funciones o bloques de código dentro de una clase.
$this es una variable reservada por el lenguaje que podemos usar para acceder a elementos propios, siempre y cuando estemos en la instancia de la clase.
new es la palabra clave usada para crear un objeto a partir de una clase.
En el mundo de la programación tenemos muchas técnicas y formas, podemos instanciar una clase dentro de otra y navegar por sus métodos sin restricción.

```php
<?php
class User
{
    public $type;
}

class Admin
{
    public function greet()
    {
        echo "Hola Administrador";
    }
}

$user = new User;
$user->type = new Admin;
$user->type->greet();

<?php
class Person
{
    public function greet()
    {
        echo "Hola $this->name";
    }
}

class User
{
    public $type;
}

class Admin extends Person
{
    public $name = 'Administrador';
}

$user = new User;
$user->type = new Admin;
$user->type->greet();
```

Son conceptos, métodos o formas que usamos a veces sin saber que estos conceptos existen. Revisa en detalle cada cosa y trata de hacer un ejercicio por concepto para que estos formen parte de ti.
