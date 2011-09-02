!SLIDE

# ¿Quiénes somos?

!SLIDE

## Ruby Argentina
## Asociación Civil

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
    value = "Hello, UTN!"
    puts value # => Hello, UTN!
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

    puts "Hello, UTN!" if Time.now.friday?

    (1..5).each do |i|
      puts "El cuadrado de #{i} es #{i * i}"
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
##### donde *user* es una variable que fue creada fuera del bloque y el bloque puede acceder a ella

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
#### ([http://www.sinatrarb.com/](http://www.sinatrarb.com/))
<br>
## *Minimalista y Simple*
<br>
@@@ ruby
    require 'sinatra'
    
    get '/hi' do
      "Hello World!"
    end
@@@
<br>

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
##(Las cosas que no te dá Ruby las podés obtener con RubyGems)

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
    => "cerrando detalles de la charla de #Ruby para la UTN"
    
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
### Proyectos en GitHub: jQuery, Symfony, DJAngo

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
### ruby-lang.org
<br>
### Lista rubysur@googlegroups.com
<br>
### ruby.com.ar - @rubyargentina

!SLIDE

# Eventos en Argentina
<br>
## Meetups (Mensuales)
<br>
## RubyConf Argentina 2011 (Noviembre)

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

