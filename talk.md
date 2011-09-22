!SLIDE

# ¿Quiénes somos?

!SLIDE

## Ruby Argentina
## Asociación Civil

!SLIDE

## Hoy vamos a contarles acerca de:

!SLIDE

# ルビ   (Ruby)

!SLIDE

##Agenda
<br/>
* Características de Ruby<br/>
* Instalar Ruby<br/>
* Web Frameworks<br/>
* Ruby Ecosystem<br/>
* Recursos<br/>
* Eventos locales<br/>

!SLIDE

##Características de Ruby

!SLIDE

## Multiplataforma
<br>
### *Windows*
<br>
### *Linux*
<br>
### *Mac OS*

!SLIDE

## Múltiples implementaciones
<br>
### MRI: C
<br>
### JRuby: Java
<br>
### IronRuby: .NET
<br>
### Rubinius: Ruby

!SLIDE

# *Interpretado*

!SLIDE

# *Dinámico*
<br>
@@@ ruby
    value = 42
    puts value # => 42
    value = "Hello, UP!"
    puts value # => Hello, UP!
@@@
<br>
<br>
#####(Las variables son objetos y al definirse no se especifica el tipo)

!SLIDE

# *Orientado a Objetos*

!SLIDE

### En Ruby todo es un objeto
<br>
@@@ ruby

    >> "fnoCybuR".reverse
    => "RubyConf"

@@@

!SLIDE

# Todo es *Abierto*

!SLIDE

(No sólo el código fuente es abierto: [https://github.com/ruby/ruby](https://github.com/ruby/ruby))
<br>
@@@ ruby

    class String
      def greet
        "Hola #{self}!"
      end
    end

    >> "UP".greet
    => "Hola UP!"

@@@

!SLIDE

# Es muy *Expresivo*

!SLIDE code

@@@ ruby

    10.times do
      puts "<3"
    end

    puts "Hello, UP!" if Time.now.friday?

    (1..5).each do |i|
      puts "El cuadrado de #{i} es #{i * i}"
    end

@@@

!SLIDE

# "Ruby is designed for programmer happiness"
<br>
matz

!SLIDE

## *Interacciones ágiles con bases de datos*

!SLIDE

@@@ ruby

    University.find_by_name("UP")

@@@

!SLIDE

## *Closure*
<br>
@@@ ruby

    user = "Foo Bar"
    10.times do
      puts user
    end

    # Donde *user* es una variable que fue creada 
    # fuera del bloque y el bloque puede acceder a ella
@@@
<br>

!SLIDE

## *Lambda*
<br>
@@@ ruby

    reverse_string_order = -> x, y { y.to_s <=> x.to_s }
    [1, 20, 3].sort &reverse_string_order

    square = -> n { n * n }
    [1, 2, 3, 4, 5].map &square

@@@

!SLIDE

## Instalar Ruby

!SLIDE

## Ruby.install!

<ul><li>Mac OS: Ya viene instalado<li></ul>
<ul><li>Linux: Ya instalado, o "apt-get install ruby ..." <li></ul>
<ul><li>Windows: rubyinstaller.org</li></ul>

!SLIDE

## Ruby.installed?


conf$ ruby -v<br/>
=> ruby 1.9..... <br>

<br/><br/>

## Interactive Ruby
conf$ irb<br/>

@@@ ruby

	"hola mundo".split
	=> ["hola", "mundo"] 

@@@ 

!SLIDE

## Probar Ruby online

http://tryruby.org

!SLIDE

# Web Frameworks
<br>
### Objetivo principal: Más productividad

!SLIDE

# Ruby on Rails
#### ([http://rubyonrails.org/](http://rubyonrails.org/))

!SLIDE

## *MVC*
<br>
## "Convention Over Configuration"
<br>
## "Don’t Repeat Yourself" (DRY)
<br>
## ORM -> ActiveRecord
<br/>
## Database Migrations
<br/>
## *Generadores*
<br>

!SLIDE

<br>
##### (Ejemplo)

!SLIDE

#Sinatra
#### ([http://www.sinatrarb.com/](http://www.sinatrarb.com/))
<br>
## *Minimalista. Simple.*
<br>
@@@ ruby
    require 'sinatra'
    
    get '/hi' do
      "Hello World!"
    end
@@@
<br>

!SLIDE

# Ejemplo de Padrino.rb

!SLIDE

# Otros Frameworks
<br>
## Cuba
<br>
## Padrino
<br>
### Otros más... (Sobre Rack)

!SLIDE

# Ruby Ecosystem

!SLIDE

# Windows Friendly

## Ruby Installer

## Rails Installer

!SLIDE

# Ruby Version Management

## rvm (Mac/Linux)

## pik (Windows)

!SLIDE

# Rake: Ruby Make
<br>
## #Rakefile
@@@ ruby
    task :default => [:test]

    task :test do
      ruby "test/unittest.rb"
    end
@@@ 
<br>
## #Bash
@@@ bash

    rake test

@@@
<br>

!SLIDE

# RubyGems: Distribución de paquetes
<br>
##(Las cosas que no te da Ruby las podés obtener con RubyGems)

!SLIDE

# RubyGems: Ejemplo @Twitter
<br>
## #bash
@@@ bash
    gem install 'twitter'
    irb
@@@
<br>
## #irb
@@@ ruby

    > require 'twitter'
    => true
    > Twitter.user_timeline("_nesto").first.text
    => "cerrando detalles de la charla de #Ruby para la UP"
    
!SLIDE

# Git
<br>
## SCM (Como SVN, CVS pero mejor!)
<br>
### Proyectos en Git: Linux, Debian, Eclipse

!SLIDE

# GitHub
<br>
## Social Coding (Open Source Fun!)
<br>
### Proyectos en GitHub: jQuery, Symfony, DJAngo, Linux Kernel

!SLIDE

# Gems Más Usados
<br>
### Sass
<br>
### Capistrano
<br>
### Haml
<br>
### Capybara
<br>
### Cucumber
<br>
### Rails

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
### ruby-lang.org/es/ -> "Ruby en 20 minutos"
<br>
### Lista rubysur@googlegroups.com
<br>
### ruby.com.ar - @rubyargentina
<br/>
### Rails for Zombies -> http://railsforzombies.org

!SLIDE

# Eventos locales

!SLIDE

## Meetups (Mensuales)
<br>
Se anuncian en www.ruby.com.ar

!SLIDE

## RubyConf Argentina 2011 

# 8 y 9 de Noviembre
Ciudad Cultural Konex
<br/>
<br/>
Parte del <i>"Tour Ruby Sur"</i>

!SLIDE

## Speakers
<br/><br/>

## Shugo Maeda
## Aaron Patterson
## Konstantin Haase
## Scott Chacon
## Tom Preston-Werner
## Luis Lavena
<br/>
### Y muchos más.

!SLIDE

## http://rubyconfargentina.org
### @rubyconfar
<br>

!SLIDE

Martin Aceto (@maceto)<br/>
Ernesto Tagwerker (@_nesto)<br/>
Leandro Lopez (@inkel)<br/>
Matias Owsianik (@matiasow)<br/>
Sebastian Rabuini (@sebasr)<br/>
Michel Martens (@soveran)<br/>
Lucas Florio (@lucasefe)<br/>
Chad DePue<br/>
Tom Henrik Aadland (@tomhenrik)<br/>
Nicolás Cerrini (@ceneon)<br/>

!SLIDE

## ¿Preguntas?


!SLIDE

## Gracias por venir

<br/><br/>

## http://ruby.com.ar
## http://rubyconfargentina.org
### @rubyconfar




