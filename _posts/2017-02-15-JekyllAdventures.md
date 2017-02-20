---
layout: post_page
title: Jekyll Adventures
---


Gracias a un curso que tome en CodeAcademy habia creado con anterioridad un sitio en Github Pages sin embargo no fue hasta el dia de hoy que me decidi por incorporar la tecnologia por completo en mi sistema.

Jekyll es un generador de sitios estaticos, esto quiere decir que podemos incluir archivos en Markdown y estos seran trandormados en HTML. Podemos ademas generar el Layout del sitio incluyendo multiples archivos HTML con el renderizador Liquid.

De las multiples plantillas y estilos existentes busque uno que fuera minimalista y enfocado a un blog, principalmente de texto. Entre ellos encontre [Vanilla Bean Creme Theme](http://richbray.me/frap/) el cual parece servir mis necesidades sin embargo carece de un menu por categorias.

Para iniciar mi desarrollo en Jekyll tuve que installar Chocolatey, Ruby, RubyGems y [RubyDevKit](http://rubyinstaller.org/downloads/). La mayoria de las installaciones y compilaciones se realizaron desde PowerShell:

~~~ powershell
PowerShell.exe -ExecutionPolicy Undefined
iwr https://chocolatey.org/install.ps1 -UseBasicParsing | iex
choco install ruby -y
ruby dk.rb init
ruby dk.rb review
ruby dk.rb install
gem install jekyll bundler
gem install jekyll-paginate-v2
gem install jekyll-feed
gem install jekyll-gist
gem install rouge
gem install wdm
cinst -Source "https://go.microsoft.com/fwlink/?LinkID=230477" libxml2
cinst -Source "https://go.microsoft.com/fwlink/?LinkID=230477" libxslt
cinst -Source "https://go.microsoft.com/fwlink/?LinkID=230477" libiconv
gem install nokogiri
jekyll new blogname
*Enter blogname directory*
bundle exec jekyll serve
~~~
