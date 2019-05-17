# Ayudantia 6

## Bootstrap ##
Bootstrap es una biblioteca multiplataforma o conjunto de herramientas de código abierto para diseño de sitios y aplicaciones web.

Instalación Bootstrap 4 en el proyecto:

- Instalar siguientes gemas en el Gemfile:
~~~~
gem 'bootstrap'
gem 'jquery-rails'
gem 'simple_form'
gem 'popper_js'
gem 'tether-rails'
~~~~
- Correr ``` docker-compose build ``` para instalr gemas o hacer bundle install

- Editar archivo ``` /app/assets/javascripts/application.js ```
Borrar línea ``` //= require rails-ujs``` reemplazar por  ``` //= require jquery3 ```
Agregar las siguientes líneas:
```
//= require jquery_ujs
//= require popper
//= require tether
//= require bootstrap
```
- Instalar simpleform para que los siguientes scaffolds que tengamos se crean con formularios bootstrap. Correr en consola:

``` docker-compose exec web rails g simple_form:install -bootstrap ```

- Ir al archivo ``` app/assets/stylesheets/application.css ``` renombrarlo para que quede como ```application.css ```

- Editar ese archivo borrando todo lo que aparece comentado y reemplazarlo por 
~~~
@import "/*";
@import "bootstrap";
@import "tether";
~~~


 - Estas listo para usar Bootstrap

Recomiendo revisar la documentación de bootstrap para ver como se usan los distintos componentes que provee la librería.
https://getbootstrap.com

    
