!SLIDE

# Padrino
<br/>
* Sinatra
<br/>
* Rápido
<br/>
* Agnóstico

<style>
  pre {
    font-family: monospace;
  }
</style>

!SLIDE

# Generators
<br/>
* project
<br/>
* mailer
<br/>
* controller
<br/>
* model
<br/>
* migration

!SLIDE

# Instalación

<br/>
@@@ bash

    gem install padrino
    
@@@

!SLIDE

# Generación

<br/>
@@@ bash

    padrino generate project blag -t shoulda -e haml -d activerecord
    
    cd blag
    
    bundle install
    
@@@

!SLIDE

# #app.rb
<br/>
@@@ ruby

    class Blag < Padrino::Application
      register Padrino::Rendering  
      register Padrino::Helpers
  
      # GET /
      get "/" do
        "Hello UP!"
      end

    end
    
@@@

!SLIDE

# Panel de Administración

<br/>
@@@ bash
    
    padrino generate admin

@@@

!SLIDE

# Migración de Base de Datos

<br/>
@@@ bash
    
    padrino rake ar:create
    
    padrino rake ar:migrate

@@@

!SLIDE

# Datos Iniciales

<br/>
@@@ bash

    padrino rake seed

@@@ 

!SLIDE

# Creación del Model Post

<br/>
@@@ bash

    padrino generate model post title:string body:text

@@@ 

!SLIDE

# Creación de Tabla de Posts

<br/>
@@@ bash

    padrino rake ar:migrate

@@@ 

!SLIDE

# Creación del Administrador

<br/>
@@@ bash

    padrino generate admin_page post

@@@ 

!SLIDE

# Listo!

<br/>
@@@ bash

    padrino start

@@@ 

!SLIDE

# Recursos: 
<br/>
* Ejemplo: [https://github.com/etagwerker/blag](https://github.com/etagwerker/blag)
<br/>
* Fuente: [http://www.padrinorb.com/guides/blog-tutorial](http://www.padrinorb.com/guides/blog-tutorial)
<br/>
* Padrino: [http://www.padrinorb.com/](http://www.padrinorb.com/)
<br/>
* Sinatra: [http://www.sinatrarb.com/](http://www.sinatrarb.com/)
