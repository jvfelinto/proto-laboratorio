---
layout: post
title: Sobre o Jekyll
date: 2026-10-01 13:49 -0300
---

Dedico este post ao meu amigão Cira Lex, ele mostrou interesse em criar um site que usaria o Jekyll, mas achou complicado demais. Não irei tentar CONVECER-LO, mas acho que escrever sobre é interessante.

<hr>

## O Jekyll em si, e companhia

O Jekyll "transforma plain text em websites e blogs", eles mesmos falam isso <a href="https://jekyllrb.com/">aqui</a>. Começamos com os pré requisitos, que é a linguagem de programação Ruby; o RubyGems, o gerenciador de pacotes pro Ruby; e o GCC e Make, um compilador da linguagem C e um gerador de executáveis; eu não faço a menor ideia como que instala esses requisitos no Windows, mais informações <a href="https://jekyllrb.com/docs/installation/windows/">aqui</a>, no Fedora foi tranquilo, estava tudo no DNF. 

Após isso, você vai baixar o bundler e o jekyll, que são o FUNDAMENTAL para o esquema, para iniciar um blog básico de template você usa o comando 

<code>jekyll new meublog</code>

Isso vai criar uma pasta chamada <code>meublog</code> com os componentes básicos do blog, para rodar o site na SUA máquina você dentro da pasta do blog usa o comando 

<code>bundle exec jekyll serve</code>, que abre o site no <code>http://localhost:4000</code>

Ai você já tem tecnicamente um site com um blog pronto e pode começar a adicionar posts, o template inicial usa o estilo Minima, que você pode trocar para outro, ou criar seus próprios. Para postar você cria um novo arquivo markdown na pasta de posts, com a data e nome no formato certo, então você só começa a escrever. <a href="https://jekyllrb.com/docs/">Fonte 1</a>, <a href="https://jekyllrb.com/docs/themes/">fonte 2</a>.

<hr>

## Hostear

Há várias maneiras, eu usei o Github Pages, é fácil e gratuito. Funciona assim: você cria um repositório no Github, nesse repositório, deve haver um arquivo chamado <code>index.html</code> ou <code>index.md</code>, esse é o arquivo de entrada. Você vai em configurações, vai ter lá a seção Pages ou Páginas, escolhe o branch que no caso de um site vai ser o main, então o Github vai pegar o seu arquivo de entrada e publicar como um site, se seu arquivo de entrada linkar para outros arquivos, parabéns você publicou um site com mais de uma página, o potencial é infinito.

No caso de Jekyll especificamente, você vai criar um repositório e vai por todos os arquivos da pasta do blog nele, e então você só precisa configurar o Pages. <a href="https://docs.github.com/pt/pages/getting-started-with-github-pages/creating-a-github-pages-site"> Fonte</a>.

<hr>

## Um exemplo

Digamos que você quer fazer um site para ter o seu livro, então decide usar o Jekyll. Você cria a pasta do blog, escolhe/cria um estilo, cria uma homepage legal beleza, e põe no Github Pages. Já foi a parte difícil, para postar uma página ou capítulo do seu livro, você cria um novo post com o conteúdo, simples assim.

Há coisas que eu não mencionei, tem como customizar mais, domínio customizado, animações, etc, mas esse é o básico.
