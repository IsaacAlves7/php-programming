<a href="https://github.com/IsaacAlves7/php-programming"><img src="https://kinsta.com/pt/wp-content/uploads/sites/3/2019/05/o-que-php.png"></a>

# It's a repository of PHP language 🐘

> 🐘 **Preparação**: Para este conteúdo, o aluno deverá dispor de um computador com acesso à internet, um web browser com suporte a HTML 5 (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, Opera etc.), um editor de texto ou IDE (VSCode etc.) e o software PHP, com a versão mais recente, instalado na sua máquina local.

<!-- https://madewithlaravel.com/boilerplate -->

<div align="center"><img src="https://poster.keepcalmandposters.com/5502447.jpg" height="177"></div>

# 🐒 Paradigmas de desenvolvimento de software
<div align="center"><img src="https://user-images.githubusercontent.com/61624336/112900537-065ce480-90ba-11eb-86f7-f9006445876a.png"></div>

Hoje em dia, o desenvolvimento de sistemas se baseia em vários e diferentes paradigmas, tais como os listados a seguir:

- **Imperativo (Procedural)**: Segue sequências de comandos ordenados segundo uma lógica.
- **Funcional**: Trabalha com a divisão de problemas através de funções, que resolvem separadamente problemas menores e que, ao serem organizados, resolvem o problema como um todo.
- **Lógico**: Voltado ao desenvolvimento de problemas de lógica e usado em sistemas de inteligência computacional.
- **Orientado a Objetos (OO)**: Define um conjunto de classes para dividir o problema e realiza a interação entre as diferentes classes para também resolver o problema como um todo.

# 🐘 PHP - Hypertext Preprocessor 
<div align="center"><img src="https://upload.wikimedia.org/wikipedia/commons/2/27/PHP-logo.svg" height="207"><img src="https://d1zviajkun9gxg.cloudfront.net/user/prod/2020/01/05/fastpages-892f9602-fc52-42e6-9e81-2ea8f1477f89.png" height="207"></div><br \>

O **PHP** (**H**ypertext **P**reprocessor, originalmente **P**ersonal **H**ome **P**age) é uma linguagem de alto-nível de programação Web, criada por <a href="https://github.com/rlerdorf">Rasmus Lerdorf</a>, focada no desenvolvimento back-end para banco de dados.

# 🖥️ Servers
<div align="center"><img src="https://www.kalhost.com/images/php-icon.png" height="277"></div>

Como já aprendemos em sistemas distribuídos, um **servidor** é um software ou computador, com sistema de computação centralizada que fornece serviços a uma rede de computadores, chamada de **cliente** (não confunda com Client-Side). O principal papel de um servidor é fornecer algo de maneira centralizada, acabando com a necessidade de se ter um programa ou sistema instalado em cada equipamento de cada um dos usuários de uma empresa. Atualmente servidores são adotados para fornecer praticamente tudo que se consiga imaginar e esteja relacionado com computação.

# ⛵ phpMyAdmin
<div align="center"><img src="https://symbols.getvecta.com/stencil_91/64_phpmyadmin.7ca31c1e28.svg" height="207"></div><br \>

# ⬛ Bitnami
<div align="center"><img src="https://cdn.worldvectorlogo.com/logos/bitnami.svg" height="277"></div>

# ⓦ WordPress
<div align="center"><img src="https://cdn.worldvectorlogo.com/logos/wordpress-blue.svg" height="277"></div><br \>

# 📦 `composer`
<a href="https://getcomposer.org/doc/00-intro.md"><img src="https://cdn.worldvectorlogo.com/logos/composer.svg" height="77" align="right"></a>

O **Composer** é um gerenciador de dependências para a linguagem PHP. Ele permite que você declare as bibliotecas das quais o seu projeto depende e as gerencia (instala e atualiza) para você. Composer é amplamente utilizado na comunidade PHP para facilitar a inclusão e o gerenciamento de pacotes e bibliotecas de terceiros em projetos. Composer é uma ferramenta essencial para desenvolvedores PHP modernos, simplificando a gestão de dependências e promovendo melhores práticas de desenvolvimento. Ele facilita a integração de bibliotecas externas e ajuda a manter o projeto organizado e fácil de manter.

Principais Funcionalidades do Composer:

1. **Gerenciamento de Dependências**: Composer permite que você defina as dependências do seu projeto em um arquivo chamado `composer.json`. Ele resolve automaticamente as dependências, baixa e instala as bibliotecas necessárias.

2. **Autoloading**: Composer gera automaticamente um autoloader que permite carregar as classes das bibliotecas instaladas sem a necessidade de manualmente incluir os arquivos PHP, facilitando a organização e estruturação do código.

3. **Repositório Packagist**: Composer utiliza o Packagist, um repositório público onde desenvolvedores podem compartilhar e encontrar bibliotecas PHP. Você pode facilmente buscar e instalar pacotes do Packagist em seu projeto.

4. **Versões e Restrições de Versão**: Composer permite especificar versões específicas ou intervalos de versões para suas dependências, garantindo que o seu projeto use versões compatíveis e estáveis das bibliotecas.

5. **Scripts**: Composer permite definir scripts que podem ser executados em certos momentos do ciclo de vida do projeto, como antes ou depois da instalação de pacotes.

Como Usar o Composer:

Aqui está um guia básico sobre como instalar e usar o Composer em um projeto PHP.

Instalação do Composer:

Você pode instalar o <a href="https://youtu.be/XO5VFfiqOPI">Composer</a> globalmente no seu sistema ou localmente no seu projeto. Aqui está um exemplo de instalação global:

```sh
# Download e instalação do Composer
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php composer-setup.php
php -r "unlink('composer-setup.php');"

# Movendo o Composer para um diretório acessível globalmente
mv composer.phar /usr/local/bin/composer
```

Inicializando um Projeto com Composer:

1. **Criar um Arquivo `composer.json`**: Você pode criar este arquivo manualmente ou usando o comando `composer init`, que guia você na criação do arquivo.

```sh
composer init
```

2. **Adicionar Dependências**: Adicione dependências ao seu projeto. Por exemplo, para adicionar a biblioteca `monolog/monolog`:

```sh
composer require monolog/monolog
```

Este comando atualiza o arquivo `composer.json` e cria (ou atualiza) o arquivo `composer.lock`, além de baixar e instalar as bibliotecas necessárias na pasta `vendor`.

3. **Atualizar Dependências**: Para atualizar todas as dependências para as versões mais recentes permitidas pelo `composer.json`:

```sh
composer update
```

4. **Instalar Dependências**: Para instalar todas as dependências definidas no `composer.json` (útil quando você clona um projeto):

```sh
composer install
```

Exemplo de Arquivo `composer.json`:

Aqui está um exemplo simples de um arquivo `composer.json`:

```json
{
    "name": "meuprojeto/exemplo",
    "description": "Um projeto de exemplo usando Composer",
    "require": {
        "monolog/monolog": "^2.0"
    },
    "autoload": {
        "psr-4": {
            "MeuProjeto\\": "src/"
        }
    }
}
```

Usando o Autoload do Composer:

Para usar o autoloader gerado pelo Composer, inclua o seguinte em seu arquivo principal PHP:

```php
require 'vendor/autoload.php';
```

Isso permite que você utilize as classes das bibliotecas instaladas sem precisar manualmente incluir cada arquivo.

# 📦 Packagist
<div align="center"><img src="https://www.pngkey.com/png/full/178-1787579_in-this-section-we-will-create-a-php.png" height="277"></div>

# 🔋 Web Stacks

# 🪟 WAMP stack
<div align="center"><img src="https://upload.wikimedia.org/wikipedia/commons/f/f4/WampServer-logo.svg" height="277"></div>

# 💡 LAMP stack
<div align="center"><img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/apple/285/light-bulb_1f4a1.png" height="177"></div><br \>

# 🕯️ LEMP stack
<div align="center"><img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/apple/285/candle_1f56f-fe0f.png" height="177"></div><br \>

# 🦴 XAMPP stack
<div align="center"><img src="https://cdn.worldvectorlogo.com/logos/xampp.svg" height="277"></div>

# 🧨 LNPP stack
<div align="center"><img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/120/apple/285/firecracker_1f9e8.png" height="177"></div>

# 💓 PHP Frameworks
<div align="center"><img src="https://programadoresbrasil.com.br/wp-content/uploads/2020/06/phplinguagem1.png" height="377"></div><br \>

# 🍰 CakePHP
<div align="center"><img src="https://cdn.worldvectorlogo.com/logos/cakephp-1.svg" height="277"></div>

# 🟧 Laravel
<div align="center"><img src="https://cdn.worldvectorlogo.com/logos/laravel-2.svg" height="277"></div>

# 🔥 CodeIgniter
<img src="https://cdn.worldvectorlogo.com/logos/codeigniter.svg" height="77" align="right">

# 🟩 Zend
<img src="https://cdn.worldvectorlogo.com/logos/zend-framework.svg" height="77">

# ⚫ Symfony
<img src="" height="77">

# 💧 Drupal
<img src="https://cdn.worldvectorlogo.com/logos/drupal.svg" height="77">

# 🌱 Yii Framework
<div align="center"><img src="https://www.yiiframework.com/image/design/logo/yii3_sign.svg" height="277"></div>

# Linguagem Hack
<img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/Hack_%28programming_language%29_logo.svg" height="77" align="right">

A linguagem Hack é uma linguagem de programação desenvolvida pela equipe do Facebook como uma extensão do PHP. Ela foi criada para melhorar a performance, a segurança e a produtividade do desenvolvimento em PHP, mantendo uma sintaxe familiar para os desenvolvedores PHP. Hack introduz várias características modernas e eficientes que não são nativas do PHP, oferecendo uma experiência de desenvolvimento mais robusta. Hack é uma linguagem poderosa que traz muitas melhorias em relação ao PHP tradicional, oferecendo um ambiente de desenvolvimento mais seguro e eficiente.

Aqui estão algumas das principais características da linguagem Hack:

1. **Tipagem Estática**: Hack suporta tipagem estática opcional, permitindo que os desenvolvedores definam explicitamente os tipos de variáveis, parâmetros de funções e retornos de funções. Isso ajuda a detectar erros em tempo de compilação em vez de tempo de execução.

2. **Inferência de Tipos**: Mesmo que a tipagem estática seja opcional, Hack pode inferir os tipos de muitas expressões automaticamente, reduzindo a necessidade de anotações explícitas.

3. **Coleções**: Hack introduz coleções modernas (como `Vector`, `Map` e `Set`) que são mais consistentes e eficientes do que as arrays tradicionais do PHP.

4. **Generics**: A linguagem suporta tipos genéricos, permitindo que as coleções e funções sejam definidas de maneira a trabalhar com qualquer tipo de dado, aumentando a reutilização de código e a segurança de tipos.

5. **Async/Await**: Hack possui suporte nativo para programação assíncrona com `async` e `await`, facilitando a escrita de código assíncrono de maneira mais clara e menos propensa a erros.

6. **Shapes**: Shapes são uma estrutura de dados flexível que permite definir e usar arrays associativos com uma verificação de tipos mais rigorosa.

7. **Lambda Expressions**: Hack suporta funções anônimas (lambdas) que podem capturar variáveis do escopo externo, oferecendo uma maneira concisa de definir funções de curto prazo.

8. **Modo Estrito**: O modo estrito (`strict mode`) do Hack exige que todas as variáveis e funções sejam anotadas com tipos, proporcionando um nível adicional de segurança e rigor na verificação de tipos.

Exemplo de Código em Hack: Aqui está um exemplo simples de um script escrito em Hack:

```hack
<?hh // strict

// Função que soma dois inteiros
function soma(int $a, int $b): int {
    return $a + $b;
}

// Função que retorna uma mensagem de saudação
function saudacao(string $nome): string {
    return "Olá, " . $nome;
}

// Exemplo de uso de coleções
function exemploColecao(): void {
    $vec = Vector {1, 2, 3};
    foreach ($vec as $valor) {
        echo $valor . "\n";
    }
}

// Chamada das funções
<<__EntryPoint>>
function main(): void {
    echo soma(5, 10) . "\n";
    echo saudacao("Mundo") . "\n";
    exemploColecao();
}
```

Neste exemplo:
- A função `soma` aceita dois inteiros e retorna um inteiro.
- A função `saudacao` aceita uma string e retorna uma string.
- A função `exemploColecao` demonstra o uso de uma coleção `Vector`.
- A anotação `<<__EntryPoint>>` define o ponto de entrada do script.

# PDO - PHP Data Objects
O **PDO** (PHP Data Objects) é uma extensão da linguagem PHP que fornece uma interface para acessar bancos de dados. A principal vantagem do PDO é sua capacidade de trabalhar com múltiplos sistemas de gerenciamento de banco de dados (SGBD) de forma consistente e segura, sem que o desenvolvedor precise modificar o código de sua aplicação ao trocar de SGBD. PDO é uma ferramenta poderosa para desenvolvedores PHP que precisam de flexibilidade e segurança ao interagir com bancos de dados.

Aqui estão algumas características importantes do PDO:

1. **Abstração de Banco de Dados**: PDO permite que você use a mesma interface para interagir com diferentes bancos de dados, como MySQL, PostgreSQL, SQLite, entre outros. Isso facilita a portabilidade da aplicação.

2. **Preparação e Execução de Declarações**: PDO suporta declarações preparadas, que são úteis para proteger contra ataques de injeção SQL. Você pode preparar uma declaração com marcadores de posição e executá-la várias vezes com diferentes valores.

3. **Segurança**: Com declarações preparadas, PDO ajuda a evitar injeções de SQL. Os parâmetros são vinculados à declaração preparada de forma segura, o que reduz significativamente os riscos.

4. **Manejo de Erros**: PDO oferece uma forma elegante de lidar com erros através de exceções. Isso facilita a depuração e a manipulação de falhas na execução de consultas.

5. **Transações**: PDO fornece suporte a transações, permitindo que você execute múltiplas operações de banco de dados como uma única unidade de trabalho. Isso é essencial para garantir a consistência dos dados.

Exemplo de Uso: Aqui está um exemplo básico de como usar PDO para conectar-se a um banco de dados MySQL e realizar uma consulta:

```php
<?php
// Configuração da conexão
$dsn = 'mysql:host=localhost;dbname=teste';
$usuario = 'root';
$senha = '';

// Criando uma nova instância de PDO
try {
    $pdo = new PDO($dsn, $usuario, $senha);
    // Configurando o modo de erro do PDO para exceções
    $pdo->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);
    
    // Preparando uma declaração SQL
    $stmt = $pdo->prepare('SELECT * FROM usuarios WHERE id = :id');
    $stmt->execute(['id' => 1]);
    
    // Obtendo os resultados
    $usuario = $stmt->fetch(PDO::FETCH_ASSOC);
    print_r($usuario);
} catch (PDOException $e) {
    echo 'Erro: ' . $e->getMessage();
}
?>
```

Neste exemplo, a conexão com o banco de dados é estabelecida usando o Data Source Name (DSN), o nome de usuário e a senha. Uma consulta SQL é preparada com um marcador de posição (`:id`), que é seguro contra injeções de SQL. A consulta é executada e os resultados são obtidos.

# Design Patterns

# XHP
<div align="center"><img src="https://camo.githubusercontent.com/b788fc3cc9e4d36a567f8c218e099f6e89a7840348f5d7755b51639081f222a8/68747470733a2f2f6868766d2e6769746875622e696f2f7868702d6c69622f696d616765732f7868705f6c6f676f2e706e67" height="177"></div>
