---
layout: post_page
title: Jekyll Adventures
---

Gracias a un curso que habia tomado en [CodeAcademy](https://www.codecademy.com/) aprendi a crear sitios en [Github Pages](https://pages.github.com/), sin embargo no fue hasta el dia de hoy que me he decidido por incorporar [Jekyll](https://jekyllrb.com/)(Generador de Sitios Estaticos) en mi sistema.

Con Jekyll podemos transformar documentos de texto en [Markdown](https://daringfireball.net/projects/markdown/) y transformarlos en HTML, es decir en un [sitio web estatico](https://techterms.com/definition/staticwebsite). Generando a su vez el layout del sitio con un renderizador [Liquid](https://shopify.github.io/liquid/).

De las multiples plantillas y estilos que existen me decidi por uno minimalista enfocado en texto. La decision final recayo en [Vanilla Bean Creme Theme](http://richbray.me/frap/), la cual es una buena plantilla, aunque en retrospectiva deberia de haber creado mi propia plantilla desde cero.

En Windows para desarrollar en Jekyll se tiene que instalar Chocolatey, Ruby, RubyGems y [RubyDevKit](http://rubyinstaller.org/downloads/), generalmente desde PowerShell:

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
*Enter (cd) the blogname directory*
bundle exec jekyll serve
~~~
