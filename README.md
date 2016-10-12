# SOLID: los principios de la programación orientada a objetos
----------------
SOLID es el acrónimo de una serie de buenas prácticas y tecnicas de programación:

**S: (The Single Responsibility Principle o Principio de Responsabilidad Única):** Una clase debe tener una, y solamente una, razón para cambiar.
El problema surge cuando tenemos la necesidad de utilizar ese mismo método desde otra clase. Si no se refactoriza en ese momento y se crea una clase destinada para la finalidad del método, nos toparemos a largo plazo con que las clases realizan tareas que no deberían ser de su responsabilidad.


**O: (The Open/Closed Principle o Principio Abierto / Cerrado):** Una clase debe permitir ser extendida, sin necesitar ser modificada. El uso más común de extensión es mediante la herencia y la reimplementación de métodos. Existe otra alternativa que consiste en utilizar métodos que acepten una interface de manera que podemos ejecutar cualquier clase que implemente ese interface.

**L: (The Liskov Substitution Principle o Principio de Sustitución de Liskov):** Las clases derivadas deben poder ser sustituibles por sus clases base. Cuando creamos clases derivadas debemos asegurarnos de no reimplementar métodos que hagan que los métodos de la clase base no funcionases si se tratasen como un objeto de esa clase base. 

**I: (Interface Segregation Principle o Principio de Segregación de Interfaces):** Hacer interfaces de grano fino que son específicos de clientes. Este principio fue formulado por Robert C. Martin y el principal objetivo de este principio es poder reaprovechar los interfaces en otras clases. Si tenemos un interface que compara y clona en el mismo interface, de manera más complicada se podrá utilizar en una clase que solo debe comparar o en otra que solo debe clonar.

**D: (The Dependency Inversion Principle o Principio de Inversión de Dependencias):** Las abstracciones no deben depender de los detalles, los detalles deben depender de las abstracciones. También fue definido por Robert C. Martin y el objetivo de este principio es el uso de abstracciones para conseguir que una clase interactue con otras clases sin que las conozca directamente.

Esa mentalidad de desarrollar el software de manera que sea extensible sin modificarlo, se consigue utilizando la herencia, el polimorfismo, la modularidad, el encapsulamiento, abstracción.