# env-type README

Cree un archivo con la extensión `.env.type` y seleccione como lenguaje **DL Typed Environment.**

## Características

Te permite definir variables de entorno con tipos estáticos:

\!\[feature X\]\(images/feature-x.jpeg\)

## Requerimientos

Solo debes crear un archivo con el nombre `.env.type`.

## Configuración de la extensión

Esta extensión no requiere alguna configuración adicional.

## Problemas conocidos

Cuando defina un tipo estático para correo electrónico, si su correo es inválido, lo va a marcar como inválido, por ejemplo:

```envtype
DL_EMAIL: email = uncorreo-inválido
```

Sin embargo, puede marcar como válido un correo que tenga varios puntos seguidos, por ejemplo:

```envtype
DL_EMAIL: email = dlunam...ontilla@gmail.com
```

Sin embargo, el intérprete va a marcar como inválido este correo `dlunam...ontilla@gmail.com`, a menos que lo defina así:

```envtype
DL_EMAIL: email = dlunam.ontilla@gmail.com
```

Porque un correo válido no puede tener más de 1 caracter especial.

El intérprete funciona correctamente. La única observación indicada acá es que si pone más de un caracter especial permitidos en los correos electrónicos, lo va a marcar como un correo válido en el resaltado de sintaxis, mientras que el intérprete no.

## Notas de la versión

Este es el primer lanzamiento.

> Si notas algún problema, por favor, notifíquelo a `davidlunamontilla@gmail.com`.

### 1.0.0

Lanzamiento inicial.

### 1.0.1

Fixed issue #.

### 1.1.0

Added features X, Y, and Z.

---

## For more information

* [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
* [Markdown Syntax Reference](https://help.github.com/articles/markdown-basics/)

**Enjoy!**
