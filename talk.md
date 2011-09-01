!SLIDE

# Quiénes somos ?

!SLIDE

## Ruby Argentina
## Asociación Civil sin fines de lucro

!SLIDE

## Hoy vamos a contarles acerca de :

!SLIDE

# ルビ   (Ruby)

!SLIDE

## Multiplataforma
<br>
### *Windows*
<br>
### *Linux*
<br>
### *Mac OS*

!SLIDE

## Multiples implementaciones
<br>
### MRI: C
<br>
### Jruby: Java
<br>
### IronRuby: .NET
<br>
### Rubinius: Ruby

!SLIDE

# *Interpretado*

!SLIDE

# *Dinámico*
<br>
###(Las variables son objetos y al definirse no se especifica el tipo)

!SLIDE

# *Orientado a Objetos*

!SLIDE

### en Ruby todo es un objeto
<br>
@@@ ruby

    >> "fnoCybuR".reverse
    => "RubyConf"

@@@

!SLIDE

# todo es *Abierto*

!SLIDE

(Donde no sólo el código fuente es abierto: [https://github.com/ruby/ruby](https://github.com/ruby/ruby))
<br>
@@@ ruby

    class String
      def greet
        "Hola #{self}!"
      end
    end

    >> "UTN".greet
    => "Hola UTN!"

@@@

!SLIDE

# es muy *Expresivo*

!SLIDE code

@@@ ruby

    10.times do
      puts "<3"
    end

@@@

!SLIDE

# Programmer Happiness Oriented

!SLIDE

## *interacciones con bases de datos ágil*

!SLIDE

@@@ ruby

    University.find_by_name("UTN")

@@@

!SLIDE

## *Closure*
<br>
@@@ ruby

    user = "Foo Bar"
    10.times do
      puts user
    end

@@@
<br>
<br>
##### donde *user* es una variable que fue creada fuera del bloque y el bloque la encapsula

!SLIDE

## *Lambda*
<br>
@@@ ruby

    reverse_string_order = -> x, y { y.to_s <=> x.to_s }
    [1, 20, 3].sort &reverse_string_order

@@@

!SLIDE

# Web Frameworks
<br>
### objetivo principal es la productividad

!SLIDE

# Ruby on Rails 
#### ([http://rubyonrails.org/](http://rubyonrails.org/))
<br>
## *MVC*
<br>
## *Generadores*
<br>
<br>
##### (Ejemplo)

!SLIDE

#Sinatra 
#### ([https://github.com/sinatra/sinatra](https://github.com/sinatra/sinatra))
<br>
## *Simplicidad*
<br>
<br>
##### (Ejemplo)

!SLIDE

# Otros FrameWorks
<br>
## CUBA
<br>
## Padrino
<br>
### otros mas..

!SLIDE

# Ruby Ecosystem

!SLIDE

# RubyGems: Distribución de paquetes
<br>
####(las cosas que no te da ruby las podes obtener con rubygems)

!SLIDE

# Bibliotecas.
<br>
### God
<br>
### Capistrano
<br>
### Vagrant
<br>
### Capybara
<br>
### Cucumber
<br>
### RSpec

!SLIDE

# Desktop Frameworks
<br>
### Shoes
<br>
### FX Ruby
<br>
### Ruby QT

!SLIDE

# Recursos
<br>
### ruby-lang.org
<br>
### Lista rubysur@googlegroups.com
<br>
### ruby.com.ar - @rubyargentina

!SLIDE

# Eventos en Argentina
<br>
## Meet ups (Todos los meses)
<br>
## RubyConf Argentina 2011

!SLIDE

## Shugo Maeda
Uno de los responsables de que Ruby exista.

!SLIDE

## Aaron Patterson
Integrante del core de Ruby y de Rails.

!SLIDE

## Konstantin Haase
Responsable del web framework Sinatra.

!SLIDE

## Scott Chacon
Git core contributor y CIO de GitHub

!SLIDE

## Tom Preston-Werner
CTO de GitHub

!SLIDE

## Luis Lavena
Integrante del core de Ruby

!SLIDE

### Y muchos más.

!SLIDE

# 8 y 9 de Noviembre
Ciudad Cultural Konex

!SLIDE

## http://rubyconfargentina.com
### @rubyconfar
<br>
### Martin Aceto (@maceto) 
<br>
### Ernesto Tagwerker (@_nesto) 
<br>
### Leandro Lopez (@inkel) 
<br>
### Matias Owsianik (@matiasow) 
<br>
### Sebastian Rabuini (@sebasr) 

