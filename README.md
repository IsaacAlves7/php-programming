# <img src="https://cdn.worldvectorlogo.com/logos/php-1.svg" height="30"> It's a repository of PHP programming 🐘🔢
<!--
[![PHP](https://img.shields.io/badge/-index.php-000000?style=social&logo=PHP&logoColor=777BB4)](#)
[![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-fff?style=social&logo=Postgresql&logoColor=336791)](#)
[![SQL](https://img.shields.io/badge/-db.sql-fff?style=social&logo=MySQL&logoColor=336791)](#)
-->
<p>I created this repository for my PHP language learning.</p>

<a href="https://github.com/IsaacAlves7/php-programming"><img src="https://kinsta.com/pt/wp-content/uploads/sites/3/2019/05/o-que-php.png" width="1070"/></a>

## 🎒 Prerequisites and repositories 📚:
<ul>
  <li>Good domains in English;</li>
  <li>HTML5 and CSS3;</li>
  <li>Programming logic;</li>
  <li>Desire to learn.</li>
</ul>
<blockquote>⚠️ <b>Warning:</b> It's very important to install each one of components shown and to execute the codes on your own machine. Besides that, please note that repository is only focused in PHP development, if you want to learn about HTML5, CSS3, JS or PHP Frameworks i recommend to access another repositories, click on links bellow!</blockquote>

[![Web](https://img.shields.io/badge/-HTML5‍‍and‍‍css3‍‍development-8B89CC?style=for-the-badge&logo=HTML5&logoColor=white)](https://github.com/IsaacAlves7/html5-and-css3-development)
[![JS](https://img.shields.io/badge/-JavaScript-8B89CC?style=for-the-badge&logo=JavaScript&logoColor=white)](https://github.com/IsaacAlves7/javascript-programming)
[![SQL](https://img.shields.io/badge/-SQL‍‍language-777BB4?style=for-the-badge&logo=PostgreSQL&logoColor=white)](https://github.com/IsaacAlves7/sql-language)
[![React.js](https://img.shields.io/badge/-React.js-6264A7?style=for-the-badge&logo=React&logoColor=white)](https://github.com/IsaacAlves7/react.js-programming)
[![Vue.js](https://img.shields.io/badge/-Vue.js-665CAC?style=for-the-badge&logo=Vue.js&logoColor=white)](https://github.com/IsaacAlves7/vue.js-programming)

<hr>

# Cap 01: 🐘 O que é PHP? 🐘
<div align="center"><img src="https://d1zviajkun9gxg.cloudfront.net/user/prod/2020/01/05/fastpages-892f9602-fc52-42e6-9e81-2ea8f1477f89.png" height="170"></div>

O **PHP** (**H**ypertext **P**reprocessor, originalmente **P**ersonal **H**ome **P**age) é uma linguagem de alto-nível de programação Web, criada por <a href="https://github.com/rlerdorf">Rasmus Lerdorf</a>, focada no desenvolvimento back-end para banco de dados.

## 🐘 PHP na atualidade 📅
<div align="justify"><img src="https://programadoresbrasil.com.br/wp-content/uploads/2020/06/phplinguagem1.png" height="107"><img src="https://www.webgeometrics.com/wp-content/uploads/2014/04/banner-php.jpg"/></div>
<p>Muito se discute a respeito do PHP acabar em 2020 ou a partir dos anos futuros. E a resposta correta, para essa pergunta, é que não irá! Pois o PHP ainda é amplamente usado por empresas, seus frameworks e bibliotecas são amplamente utilizadas para páginas dinâmicas, templates Web e E-commerce. Além disso, sua versão chegou a 8° em 2020.</p>

## 🐘 Web Dev Stacks 🔋
Iremos utilizar o **LAMP** e o **LEMP** mais pra frente.

![36ed3e0f-5344-4a7e-b807-e6104c6d63be](https://user-images.githubusercontent.com/61624336/117226732-ad384d00-adeb-11eb-8d91-e3ea47b6050b.jpg)

## 🐘 Guia de instalação ⬇️
<div align="center"><img src="https://cdn.worldvectorlogo.com/logos/apache-13.svg" height="170"> <img src="https://cdn.worldvectorlogo.com/logos/xampp.svg" height="170"></div><br />

Instale o **servidor Apache** e um programa que rode o código, no caso utilizarei o **XAMPP**, mas você pode usar qualquer outro de acordo com a sua preferência. Após a instalação recomendo você não alterar as portas do localhost e nem colocar o mesmo endereço da porta em outro programa, muitos bancos de dados já possuem o padrão do <code>localhost:8080</code>, caso isso ocorra, altere do outro programa para evitar possíveis conflitos futuros.

### Versão do PHP pelo terminal
<pre>php -v</pre>

## 🐘 Problema de UAC ⚠️
Caso você antes tenha instalado o Xampp e desinstalou incorretamente, gerou um problema no UAC, portanto recomendo seguir os passos de instalação desse vídeo:

- https://youtu.be/EPsmGZYBDEA
- https://youtu.be/AporimmfqMk

## 🐘 Erro no XAMPP devido outro programa usar a mesma porta ❌
<img src="https://www.ybierling.com/images/large/web/apachecannotstart/apachecannotstart2.png" height="400">
Recomendo seguir os passos desse vídeo: https://youtu.be/4dK3rQiXsls

## 🐘 403 Forbidden ❌🚫
Recomendo seguir os passos desse vídeo: https://youtu.be/GqzhXCKP3iQ

## 🐘 DocumentRoot 🌳
Abrir o diretório do Apache na Área de Trabalho!

<pre>DocumentRoot "C:/Users/user/Área de trabalho"
&lt;Directory "C:/Users/user/Área de trabalho"&gt;</pre>

## 🐘 Servidor Apache XAMPP 🪶 🦴

<div align="center"><img src="https://cdn.worldvectorlogo.com/logos/xampp.svg" height="247">&nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/61624336/114465502-94a68f80-9bbd-11eb-9599-19fa00b1ec75.png" height="257"></div><br />

Após a instalação, você deve iniciar apertando o botão <code>Apache</code>, a luz verde indica que o servidor reconheceu tudo e foi executado com sucesso. Em seguida, aperte o botão <code>Admin</code> que o endereço do localhost será aberto no browser e você poderá acessar a pasta do <a href="https://github.com/IsaacAlves7/php-programming#-documentroot-">DocumentRoot</a> onde ficarão os seus projetos e arquivos do PHP. E dai você pode ter um preview da sua aplicação.

![localhost](https://user-images.githubusercontent.com/61624336/114467960-1946dd00-9bc1-11eb-93e1-63b600bc67be.png)

Agora que você já conhece a parte do servidor, vamos programar!

## 🐘 PHP: - Hello, world! (Olá, Mundo!) 🐘

[![PHP](https://img.shields.io/badge/-index.php-000000?style=social&logo=PHP&logoColor=777BB4)](#)

Primeiro, crie uma pasta para o documento e depois crie um arquivo, normalmente usamos o nome "<code>index</code>" como o arquivo principal e a extensão <code><b>.php</b></code>.

![diferentes maneiras de inserir o código php](https://user-images.githubusercontent.com/61624336/114467359-30d19600-9bc0-11eb-801c-762734774eef.jpg)

A primeira coisa que iremos fazer no arquivo é escrever a estrutura do HTML para o **Front-end** reconhecer a página, logo, podemos criar o código do php em qualquer parte do documento livremente, pois o código não será acessado pelo **front-end**, mas sim pelo **back-end** (servidor).

O código do php é bem característico da linguagem, possui a inicialização <code>&lt;?php ?&gt;</code>, e ele é um pouco similar as tags do HTML, por isso facilita o entendimento. Além disso, dentro da "tag" e no meio desses sinais de interrogação ficará o nosso código.

O comando <code>echo</code> exibe uma mensagem na tela. Pode ser inserido entre <code>()</code> ou sem, com <code>;</code> no final ou sem.

![Sem título](https://user-images.githubusercontent.com/61624336/114469393-717ede80-9bc3-11eb-827c-01e8f01bffe0.png)

Perceba que não aparece o código do php pelo código-fonte do front-end, pois, como havia dito anteriormente, somente o servidor acessou e interpretou o código.

## 🐘 Comentário no PHP 📝

# Banco de Dados

## Banco de Dados Relacionais
## MySQL

### 🪶 🦴 Inicializando o Apache e o MySQL no XAMPP 🐬

<img width="688" alt="2249" src="https://user-images.githubusercontent.com/61624336/115929405-2637bc00-a45e-11eb-97b6-7a954b2b49b6.png">


## PhpMyAdmin


<hr>

# Cap 02: 🐘 

<hr>

# 🐘 Dia do programador 🎂
![php](https://user-images.githubusercontent.com/61624336/112904846-f21be600-90bf-11eb-9641-59fd388e42e8.jpg)

