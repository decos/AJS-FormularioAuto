# MANEJO DE FORMULARIOS

## Auto validar formularios

    Recursos:
        - http://jonsamwell.github.io/angular-auto-validate/

1. Descargar el proyecto de la seccion

2. Descargar el proyecto del  primer recurso
    - Ingresar al directorio `dist` y  copiar el archivo `jcs-auto-validate.js`
    - Pegar el archivo dentro del proyecto `js/lib`
    - Añadir la referencia en el fichero `index.html`
    - Inyectar la dependencia en el controlador principal `app.js`

3. Añadir la clase `control-label` en cada label del `index`

4. Añadir `required` en cada `input` del formulario

5. Traducir a Español los mensajes de validación modificando el siguiente archivo:
    - js/lib/jcs-auto-validate.js

~~~
Error Message Resolver (Mensajes Personzalizados)
~~~

6. Añadir mensajes Personzalizados
    - En el controlador principal añadir al modulo los mensajes Personzalizados
    - Añadir a los `inputs` los mensajes personalizados usando las directivas `ng-min-err-type` y `ng-max-err-type`

## Cambiando la cultura del autovalidado

1. Añadir el fichero dentro del directorio `js/lib`
    - js/lib/jcs-auto-validate_es-co.json

2. Añadir las siguientes lineas dentro del manejador de errores:
    - defaultErrorMessageResolver.setI18nFileRootPath('js/lib');
    - defaultErrorMessageResolver.setCulture('es-CO');
