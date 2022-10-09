# Práctica 1: Introducción a Unity

## Autor

Airam Rafael Luque León (alu0101335148@ull.edu.es)

## Descripción

En esta primera práctica de la asignatura hemos realizado una primera toma de contacto con la herramienta Unity, la cual nos permite desarrollar aplicaciones gráficas, como simuladores o videojuegos. A lo largo de la practica hemos visto las funcionalidades principales como el instanciar diferentes tipos de objetos, el instalar paquetes o mediante el package manager 

En esta práctica hemos realizado las siguientes tareas:

### Incluir objetos 3D básicos

Para esta tarea hemos ido al menu lateral, hemos hecho click izquierdo y hemos buscado la opción `3D Objects`, que nos permite instanciar objetos 3D básicos en Unity, como los cubos, por ejemplo. 

### Incluir en el proyecto el paquete Starter Assets.

Para esto tenemos que buscar en la página de Unity el asset correspondiente y adquirirlo, luego vamos otra vez a la aplicación y entramos en `Windows > Package Manager`. Finalmente veremos los paquetes que podemos instalar, lo seleccionamos, lo instalamos y finalmente lo importamos.

### Incluir un objeto libre de la Asset Store que no sea de los Starter Assets.

Para esta tarea hemos usado el paquete `Fantasy Forest Environment` y hemos instanciado un arbol en la escena.

### Crear un terreno (opcional).

En este punto simplemente instanciamos una entidad `terrain` de la misma forma que hicimos cuando introducimos el cubo y la esfera.

### Cada objeto debe tener una etiqueta que lo identifique.

Se han etiquetado todas las entidades en la escena, siendo estas las siguientes:

- Cube
- Sphere
- Player (etiqueta por defecto de la entidad jugador)
- Tree
- Terrain

Ejemplo:

![example](/img/tag_example.png)

### Utilizar prefabs de Starter Asset FPS o Third Person

Para cumplimentar este punto hemos tomado el asset indicado e instanciado un jugador, el cual nos permite movernos con los controles W, A, S, D y espacio.

Para hacer más cómodo el movimiento por el mapa, incluimo la cámara dentro de este objeto, de esta forma al movernos con el, la cámara también se moverá.

![example](/img/player_example.png)


### Agregar un script que escriba en la consola los objetos que se han utilizado.

Finalmente para este punto fuimos objeto a objeto agregando un scrip con la siguiente estructura:

```C#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class objectScript : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        Debug.Log("Im a ...");
    }
}
```

## Prueba de funcionamiento

![funcionamiento](/img/performance.gif)