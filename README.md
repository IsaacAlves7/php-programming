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
<img src="https://upload.wikimedia.org/wikipedia/commons/2/27/PHP-logo.svg" height="77" align="right">

O **PHP** (**H**ypertext **P**reprocessor, originalmente **P**ersonal **H**ome **P**age) é uma linguagem de alto-nível de programação Web, criada por <a href="https://github.com/rlerdorf">Rasmus Lerdorf</a>, focada no desenvolvimento back-end para banco de dados.

<img src="https://d1zviajkun9gxg.cloudfront.net/user/prod/2020/01/05/fastpages-892f9602-fc52-42e6-9e81-2ea8f1477f89.png" height="77" align="right">

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

<img src="https://www.pngkey.com/png/full/178-1787579_in-this-section-we-will-create-a-php.png" height="77" align="right">

O **Packagist** é o principal repositório de pacotes para o gerenciador de dependências Composer, usado na linguagem PHP. Ele serve como um diretório central onde os desenvolvedores podem publicar, compartilhar e encontrar bibliotecas PHP que podem ser facilmente integradas em seus projetos através do Composer.

Principais Características do Packagist:

1. **Repositório Central**: Packagist é o repositório padrão que o Composer usa para buscar pacotes. Ele contém milhares de pacotes PHP disponíveis para uso.

2. **Busca e Descoberta**: Através do site do Packagist, os desenvolvedores podem procurar pacotes por nome, descrição ou outros critérios, facilitando a descoberta de bibliotecas úteis para seus projetos.

3. **Informações dos Pacotes**: Cada pacote no Packagist possui uma página dedicada com informações detalhadas, incluindo a descrição, versão, dependências, instruções de instalação e links para o código-fonte (geralmente hospedado no GitHub).

4. **Automação de Atualizações**: Quando um novo release de um pacote é publicado em seu repositório de origem, o Packagist é automaticamente atualizado, garantindo que os desenvolvedores tenham acesso às versões mais recentes.

5. **Integração com VCS**: Packagist se integra com sistemas de controle de versão (VCS) como GitHub, Bitbucket e GitLab, permitindo que os pacotes sejam atualizados automaticamente quando novas versões são lançadas.

Aqui está um guia básico sobre como usar o Packagist junto com o Composer:

1. **Buscar um Pacote no Packagist**:
   - Acesse o [site do Packagist](https://packagist.org/).
   - Use a barra de busca para encontrar pacotes por nome ou palavras-chave.

2. **Adicionar um Pacote ao seu Projeto**:
   - Após encontrar o pacote desejado, você verá instruções de instalação que podem ser usadas com Composer. Por exemplo, para instalar o pacote `monolog/monolog`:
     ```sh
     composer require monolog/monolog
     ```

3. **Configurar o Autoloading**:
   - Após a instalação, você deve incluir o autoloader do Composer no seu arquivo PHP principal:
     ```php
     require 'vendor/autoload.php';
     ```

Para publicar seu próprio pacote no Packagist, siga estes passos:

1. **Preparar o Projeto**:
   - Certifique-se de que seu projeto possui um arquivo `composer.json` devidamente configurado.
   - Empurre seu projeto para um repositório público no GitHub, GitLab, Bitbucket ou outro VCS suportado.

2. **Registrar o Pacote no Packagist**:
   - Acesse o [site do Packagist](https://packagist.org/).
   - Faça login (ou crie uma conta, se necessário).
   - Vá até a seção "Submit" e forneça a URL do repositório do seu projeto.
   - Packagist irá buscar seu `composer.json` e registrar o pacote.

3. **Manter o Pacote Atualizado**:
   - Sempre que você lançar uma nova versão do seu pacote, o Packagist será automaticamente atualizado se você configurar hooks do GitHub/GitLab/Bitbucket. Caso contrário, você pode atualizar manualmente através do Packagist.

Exemplo de um Arquivo `composer.json` para um Projeto:

```json
{
    "name": "meuusuario/meupacote",
    "description": "Um pacote de exemplo",
    "type": "library",
    "require": {
        "php": "^7.4 || ^8.0"
    },
    "autoload": {
        "psr-4": {
            "MeuNamespace\\": "src/"
        }
    },
    "authors": [
        {
            "name": "Seu Nome",
            "email": "seuemail@example.com"
        }
    ],
    "license": "MIT"
}
```

# [PHP] PDO - PHP Data Objects
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

# ◢◤ [PHP] Linguagem Hack
<img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/Hack_%28programming_language%29_logo.svg" height="77" align="right">

A linguagem **Hack** é uma linguagem de programação desenvolvida pela equipe do Facebook como uma extensão do PHP. Ela foi criada para melhorar a performance, a segurança e a produtividade do desenvolvimento em PHP, mantendo uma sintaxe familiar para os desenvolvedores PHP. Hack introduz várias características modernas e eficientes que não são nativas do PHP, oferecendo uma experiência de desenvolvimento mais robusta. Hack é uma linguagem poderosa que traz muitas melhorias em relação ao PHP tradicional, oferecendo um ambiente de desenvolvimento mais seguro e eficiente.

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

## [PHP] XHP
<img src="https://github.com/IsaacAlves7/php/assets/61624336/3fb6735f-42fc-4719-af56-cd762008d309" height="77" align="right">

O **XHP** é uma extensão da linguagem PHP desenvolvida originalmente pelo Facebook. Ela permite que os desenvolvedores escrevam interfaces de usuário usando uma sintaxe similar ao HTML diretamente no código PHP. Isso facilita a criação e a manutenção de componentes de UI, proporcionando uma maneira mais segura e eficiente de lidar com a manipulação de HTML. XHP é uma poderosa extensão que traz a sintaxe de componentes HTML para o PHP, melhorando a segurança e a organização do código. Embora a extensão original não seja mais mantida, a ideia por trás do XHP continua relevante e influente, especialmente em projetos que adotam Hack, a linguagem que continua a evoluir com essas capacidades integradas.

Principais Características do XHP:

1. **Sintaxe Similar ao HTML**: XHP permite que você escreva código HTML diretamente no PHP de uma maneira que parece natural. Isso ajuda a manter o código mais legível e organizado.

2. **Segurança Contra XSS**: XHP faz a sanitização automática do conteúdo, ajudando a prevenir ataques de Cross-Site Scripting (XSS). Isso significa que o conteúdo dinâmico é escapado de maneira segura antes de ser renderizado.

3. **Componentes Reutilizáveis**: XHP facilita a criação de componentes reutilizáveis de UI, permitindo que você crie elementos complexos de maneira modular e reutilize-os em diferentes partes da aplicação.

4. **Integração com PHP**: Como uma extensão do PHP, XHP se integra perfeitamente com o ecossistema do PHP, aproveitando todo o poder e as bibliotecas da linguagem.

Exemplo de Uso do XHP:

Aqui está um exemplo básico de como você pode usar XHP em um projeto PHP:

Instalação do XHP:

Antes de começar a usar XHP, é necessário instalar a extensão. No entanto, a extensão XHP original não é mais mantida. Para projetos novos, considere usar [Hack](https://hacklang.org/), uma linguagem desenvolvida pelo Facebook que incorpora XHP.

Se você ainda deseja usar XHP com PHP, você pode buscar por forks ou versões mantidas pela comunidade ou considerar o uso de [vários polyfills disponíveis](https://github.com/hhvm/xhp-lib).

Exemplo de Código:

1. **Definindo um Componente XHP**:

```php
<?php
require_once 'vendor/autoload.php';

class :my:button extends :x:element {
  attribute string type = "button", string label;

  protected function render(): XHPRoot {
    return
      <button type={$this->:type}>
        {$this->:label}
      </button>;
  }
}
```

2. **Usando o Componente no PHP**:

```php
<?php
require_once 'vendor/autoload.php';

echo
  <html>
    <body>
      <h1>Olá, Mundo!</h1>
      <my:button type="submit" label="Clique Aqui" />
    </body>
  </html>;
```

Benefícios do Uso do XHP:

1. **Maior Legibilidade**: O código que mistura HTML e PHP se torna mais legível e organizado.
2. **Reutilização de Componentes**: Componentes de UI podem ser definidos uma vez e reutilizados, promovendo a consistência e reduzindo a duplicação de código.
3. **Segurança**: A sanitização automática de conteúdo ajuda a prevenir vulnerabilidades de XSS, aumentando a segurança da aplicação.

Considerações:

- **Manutenção**: A extensão XHP original não é mais mantida. Para projetos novos, considere usar Hack ou procurar por versões mantidas pela comunidade.
- **Curva de Aprendizado**: Para desenvolvedores acostumados com a mistura tradicional de PHP e HTML, a adoção de XHP pode requerer uma curva de aprendizado inicial.

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

# 🍰 CakePHP
<img src="https://cdn.worldvectorlogo.com/logos/cakephp-1.svg" height="77" align="right">

**CakePHP** é um framework de desenvolvimento rápido (RAD) para a linguagem PHP, projetado para facilitar a criação de aplicativos web robustos e escaláveis. Ele segue o padrão de design Model-View-Controller (MVC), o que ajuda a separar a lógica da aplicação da apresentação e dos dados, tornando o desenvolvimento mais organizado e manutenível. CakePHP é um framework poderoso e estruturado que facilita o desenvolvimento de aplicações web em PHP. Ele oferece diversas funcionalidades out-of-the-box que ajudam a acelerar o desenvolvimento, mantendo o código organizado e seguro. É uma excelente escolha para desenvolvedores que buscam uma abordagem estruturada e eficiente para construir suas aplicações web.

Principais Características do CakePHP:

1. **MVC (Model-View-Controller)**: O CakePHP adota o padrão MVC, que separa a lógica da aplicação (Model), a apresentação (View) e a manipulação de dados e interações do usuário (Controller). Isso facilita a manutenção e a escalabilidade do código.

2. **Convention Over Configuration**: O CakePHP segue a filosofia de "Convenção sobre Configuração", o que significa que ele usa convenções sensatas para reduzir a necessidade de configuração explícita. Isso acelera o desenvolvimento, pois muitos aspectos do framework funcionam de forma padrão sem necessidade de configuração manual.

3. **ORM (Object-Relational Mapping)**: CakePHP inclui um poderoso ORM que facilita o trabalho com bancos de dados, permitindo que os desenvolvedores interajam com o banco de dados usando objetos PHP em vez de SQL puro.

4. **Templating**: O sistema de templates do CakePHP permite a criação de layouts reutilizáveis e views dinâmicas. Ele suporta a inclusão de elementos, helpers e layouts, tornando a construção da interface de usuário mais eficiente.

5. **Componentes e Helpers**: CakePHP fornece um conjunto de componentes e helpers que ajudam a gerenciar a lógica de negócios e a interface do usuário, como autenticação, manipulação de formulários, validação, etc.

6. **Segurança**: O CakePHP inclui várias funcionalidades de segurança, como proteção contra CSRF (Cross-Site Request Forgery), validação de dados, sanitização de entrada, proteção contra SQL Injection e mais.

7. **Ferramentas de Linha de Comando (Bake)**: O CakePHP inclui a ferramenta `bake`, que é uma linha de comando poderosa para gerar código automaticamente, como modelos, controladores, views e outros arquivos comuns.

Aqui está um exemplo básico de como começar com CakePHP, incluindo a criação de um projeto e a definição de um modelo simples:

Instalação do CakePHP

1. **Usando Composer**:
   ```sh
   composer create-project --prefer-dist cakephp/app meuprojeto
   ```

2. **Configuração do Banco de Dados**:
   Após criar o projeto, configure seu banco de dados no arquivo `config/app.php`:

   ```php
   'Datasources' => [
       'default' => [
           'host' => 'localhost',
           'username' => 'root',
           'password' => '',
           'database' => 'meubanco',
           'driver' => 'Cake\Database\Driver\Mysql',
           // Outros parâmetros de configuração...
       ],
   ],
   ```

Criando um Modelo, Controlador e View

1. **Gerando Código com Bake**:
   ```sh
   bin/cake bake model Usuarios
   bin/cake bake controller Usuarios
   bin/cake bake template Usuarios
   ```

2. **Definindo o Modelo** (`src/Model/Entity/Usuario.php` e `src/Model/Table/UsuariosTable.php`):

   ```php
   namespace App\Model\Entity;

   use Cake\ORM\Entity;

   class Usuario extends Entity {
       protected $_accessible = [
           '*' => true,
           'id' => false,
       ];
   }
   ```

   ```php
   namespace App\Model\Table;

   use Cake\ORM\Table;

   class UsuariosTable extends Table {
       public function initialize(array $config): void {
           parent::initialize($config);

           $this->setTable('usuarios');
           $this->setDisplayField('nome');
           $this->setPrimaryKey('id');

           $this->addBehavior('Timestamp');
       }
   }
   ```

3. **Criando o Controller** (`src/Controller/UsuariosController.php`):

   ```php
   namespace App\Controller;

   use App\Controller\AppController;

   class UsuariosController extends AppController {
       public function index() {
           $usuarios = $this->paginate($this->Usuarios);
           $this->set(compact('usuarios'));
       }

       public function view($id = null) {
           $usuario = $this->Usuarios->get($id);
           $this->set(compact('usuario'));
       }

       public function add() {
           $usuario = $this->Usuarios->newEmptyEntity();
           if ($this->request->is('post')) {
               $usuario = $this->Usuarios->patchEntity($usuario, $this->request->getData());
               if ($this->Usuarios->save($usuario)) {
                   $this->Flash->success(__('O usuário foi salvo.'));
                   return $this->redirect(['action' => 'index']);
               }
               $this->Flash->error(__('Não foi possível salvar o usuário.'));
           }
           $this->set(compact('usuario'));
       }
   }
   ```

4. **Criando Views** (`templates/Usuarios/index.php`, `view.php`, `add.php`):

   ```php
   <!-- templates/Usuarios/index.php -->
   <h1>Usuários</h1>
   <table>
       <tr>
           <th>ID</th>
           <th>Nome</th>
           <th>Ações</th>
       </tr>
       <?php foreach ($usuarios as $usuario): ?>
       <tr>
           <td><?= h($usuario->id) ?></td>
           <td><?= h($usuario->nome) ?></td>
           <td><?= $this->Html->link('Ver', ['action' => 'view', $usuario->id]) ?></td>
       </tr>
       <?php endforeach; ?>
   </table>
   ```

# 🟧 Laravel
<img src="https://cdn.worldvectorlogo.com/logos/laravel-2.svg" height="77" align="right">

O **Laravel** é um framework PHP de código aberto, elegante e expressivo, que oferece uma sintaxe simples e uma grande variedade de ferramentas poderosas para desenvolver aplicações web modernas e escaláveis. Ele foi criado por Taylor Otwell em 2011 e desde então tem ganhado popularidade rapidamente devido à sua facilidade de uso, documentação abrangente e robustez. O Laravel é um framework PHP moderno e robusto que oferece uma ampla gama de recursos e ferramentas poderosas para desenvolver aplicações web elegantes e escaláveis. Sua sintaxe expressiva, arquitetura MVC e ampla gama de funcionalidades integradas o tornam uma escolha popular para desenvolvedores de todos os níveis de habilidade.

Principais Características do Laravel:

1. **Expressivo e Elegante**: Laravel apresenta uma sintaxe limpa e expressiva que permite aos desenvolvedores escrever código de forma mais legível e produtiva.

2. **Arquitetura MVC**: Laravel segue o padrão de design Model-View-Controller (MVC), o que ajuda a organizar o código de forma clara e separar a lógica de negócios da apresentação.

3. **ORM Eloquent**: Laravel vem com Eloquent, um ORM (Object-Relational Mapping) intuitivo e fácil de usar, que simplifica a interação com o banco de dados, permitindo que os desenvolvedores trabalhem com bancos de dados usando objetos PHP.

4. **Sistema de Rotas Simples**: O sistema de roteamento do Laravel permite definir rotas de maneira simples e intuitiva, tornando fácil direcionar URLs para controladores e métodos específicos.

5. **Ferramentas de Migração de Banco de Dados**: Laravel oferece um sistema de migração de banco de dados que permite versionar facilmente o banco de dados da aplicação, permitindo que as alterações no esquema do banco de dados sejam controladas e compartilhadas com outros membros da equipe.

6. **Ferramenta de Paginação**: O Laravel inclui uma poderosa ferramenta de paginação que permite dividir grandes conjuntos de dados em várias páginas para facilitar a navegação e melhorar o desempenho da aplicação.

7. **Sistema de Cache**: Laravel oferece suporte a várias opções de cache, como cache de arquivo, cache de banco de dados, cache de memória e cache de Redis, o que pode ajudar a melhorar significativamente o desempenho da aplicação.

8. **Autenticação e Autorização**: Laravel simplifica a implementação de autenticação e autorização, fornecendo um sistema completo de autenticação com suporte a registro de usuários, login, recuperação de senha e muito mais.

9. **Notificações**: Laravel inclui um sistema de notificação flexível que permite enviar e-mails, SMS, notificações de push e outros tipos de notificações de forma fácil e intuitiva.

Exemplo de Uso do Laravel:

Instalação do Laravel:

Para criar um novo projeto Laravel, você pode usar o Composer. Execute o seguinte comando no terminal:

```bash
composer create-project --prefer-dist laravel/laravel nome-do-projeto
```

Criando uma Rota:

Defina uma rota no arquivo `routes/web.php`:

```php
Route::get('/', function () {
    return view('welcome');
});
```

Criando uma View:

Crie uma view em `resources/views/welcome.blade.php`:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Laravel</title>
</head>
<body>
    <h1>Bem-vindo ao Laravel!</h1>
</body>
</html>
```

Executando o Servidor de Desenvolvimento:

Execute o servidor de desenvolvimento embutido usando o comando Artisan:

```bash
php artisan serve
```

Acesse a aplicação no navegador em `http://localhost:8000`.

Benefícios do Uso do Laravel:

1. **Produtividade**: Laravel simplifica muitas tarefas comuns do desenvolvimento web, permitindo que os desenvolvedores sejam mais produtivos e eficientes.
2. **Comunidade Ativa**: Laravel tem uma grande comunidade de desenvolvedores ativos e uma vasta quantidade de recursos, incluindo documentação oficial, fóruns, pacotes de terceiros e muito mais.
3. **Segurança**: Laravel inclui várias funcionalidades de segurança, como proteção contra ataques CSRF, SQL injection, XSS e autenticação integrada.
4. **Manutenção Simples**: A estrutura organizada do Laravel e suas ferramentas integradas facilitam a manutenção e o crescimento contínuo da aplicação.

# 🔥 CodeIgniter
<img src="https://cdn.worldvectorlogo.com/logos/codeigniter.svg" height="77" align="right">

# 🟩 Zend
<img src="https://cdn.worldvectorlogo.com/logos/zend-framework.svg" height="77" align="right">

# ⚫ Symfony
<img src="https://github.com/IsaacAlves7/php/assets/61624336/c1fee442-cbf8-4b1a-a547-27610df659c1" height="77" align="right">

**Symfony** é um framework PHP de código aberto que segue os padrões de design e desenvolvimento web mais recentes. Lançado pela primeira vez em 2005, o Symfony se tornou uma das estruturas mais populares e amplamente adotadas para o desenvolvimento de aplicações web em PHP. Ele foi desenvolvido por Fabien Potencier e é mantido pela Symfony SAS, uma empresa francesa dedicada ao desenvolvimento e suporte do Symfony. Symfony é um framework PHP robusto e flexível, amplamente utilizado para o desenvolvimento de aplicações web modernas e escaláveis. Sua arquitetura modular, sua configuração flexível e sua vasta gama de funcionalidades integradas o tornam uma escolha popular entre os desenvolvedores que buscam criar aplicações web de alta qualidade.

Principais Características do Symfony:

1. **Componentes Reutilizáveis**: Symfony é construído com base em um conjunto de mais de 50 componentes PHP independentes, que podem ser usados de forma independente ou combinados para criar aplicações web complexas.

2. **Arquitetura MVC**: Symfony segue o padrão de design Model-View-Controller (MVC), que ajuda a organizar o código de maneira clara, separando a lógica de negócios (Model), a lógica de controle (Controller) e a apresentação (View).

3. **Configuração Flexível**: Symfony oferece uma configuração flexível e extensível que permite aos desenvolvedores adaptar a estrutura às necessidades específicas do projeto.

4. **Ferramentas de Linha de Comando**: Symfony inclui uma variedade de ferramentas de linha de comando (CLI) que ajudam os desenvolvedores a gerar código, executar tarefas comuns e realizar operações de manutenção de forma eficiente.

5. **Ferramentas de Teste**: Symfony oferece suporte integrado para testes automatizados, incluindo testes unitários, testes de integração e testes funcionais, facilitando a criação de código testável e a garantia da qualidade do software.

6. **Documentação Completa**: Symfony possui uma documentação abrangente e bem escrita, que cobre todos os aspectos do framework, desde a instalação e configuração até o desenvolvimento avançado e as melhores práticas.

7. **Segurança Integrada**: Symfony inclui várias funcionalidades de segurança integradas, como proteção contra ataques CSRF, XSS e SQL injection, ajudando a proteger as aplicações contra vulnerabilidades comuns.

Exemplo de Uso do Symfony:

Instalação do Symfony:

A maneira mais comum de instalar o Symfony é usando o Composer. Execute o seguinte comando no terminal:

```bash
composer create-project symfony/skeleton nome-do-projeto
```

Criando um Controlador:

Crie um controlador em `src/Controller/HelloController.php`:

```php
// src/Controller/HelloController.php

namespace App\Controller;

use Symfony\Component\HttpFoundation\Response;
use Symfony\Component\Routing\Annotation\Route;

class HelloController
{
    /**
     * @Route("/hello")
     */
    public function hello(): Response
    {
        return new Response('<html><body>Hello, World!</body></html>');
    }
}
```

Configurando as Rotas:

Defina uma rota no arquivo `config/routes.yaml`:

```yaml
# config/routes.yaml
hello:
    path: /hello
    controller: App\Controller\HelloController::hello
```

Executando o Servidor Web:

Execute o servidor web embutido usando o seguinte comando:

```bash
php -S localhost:8000 -t public
```

Acesse a aplicação no navegador em `http://localhost:8000/hello`.

Benefícios do Uso do Symfony:

1. **Flexibilidade e Escalabilidade**: Symfony oferece uma arquitetura flexível que pode ser adaptada a uma ampla gama de projetos, desde pequenos sites até grandes sistemas empresariais.

2. **Desenvolvimento Rápido**: Graças à sua configuração flexível e ao uso de componentes reutilizáveis, Symfony permite um desenvolvimento rápido e eficiente de aplicações web.

3. **Comunidade Ativa**: Symfony tem uma grande comunidade de desenvolvedores ativos e uma vasta quantidade de recursos, incluindo documentação oficial, fóruns, pacotes de terceiros e muito mais.

4. **Segurança e Confiabilidade**: Symfony é conhecido por sua segurança e confiabilidade, com funcionalidades integradas para proteger as aplicações contra vulnerabilidades comuns.

# 💧 Drupal
<img src="https://cdn.worldvectorlogo.com/logos/drupal.svg" height="77" align="right">

# 🌱 Yii Framework
<img src="https://www.yiiframework.com/image/design/logo/yii3_sign.svg" height="77" align="right">

O **Yii Framework** é um framework PHP de alto desempenho, componentizado e baseado no padrão Model-View-Controller (MVC). É conhecido por sua eficiência, flexibilidade e facilidade de uso, tornando-o uma escolha popular para desenvolvedores que buscam criar aplicações web robustas e escaláveis. O nome "Yii" significa "Yes It Is!", representando a simplicidade e facilidade de uso do framework.

Principais Características do Yii Framework:

1. **Alto Desempenho**: Yii é conhecido por ser um dos frameworks PHP mais rápidos disponíveis, otimizado para proporcionar um desempenho excelente.

2. **Componentização**: Yii é altamente componentizado, permitindo que os desenvolvedores usem apenas os componentes de que precisam e facilmente integrem novos componentes.

3. **Baseado em MVC**: Segue o padrão de design MVC, que ajuda a organizar o código de maneira clara, separando a lógica de negócios (Model), a lógica de controle (Controller) e a apresentação (View).

4. **Gii (Gerador de Código)**: Yii inclui uma poderosa ferramenta de geração de código chamada Gii, que pode gerar automaticamente o código para modelos, controladores, formulários, módulos, extensões e muito mais.

5. **Integração de Banco de Dados**: Yii suporta Active Record para interação com bancos de dados relacionais, facilitando o trabalho com dados sem escrever SQL manualmente.

6. **Segurança**: Oferece funcionalidades de segurança embutidas, como prevenção de SQL injection, XSS, CSRF, autenticação e autorização.

7. **Internacionalização (i18n)**: Suporte completo para internacionalização e localização, facilitando a criação de aplicações multilingues.

8. **Teste Automatizado**: Integrado com PHPUnit e Codeception, facilitando a criação de testes automatizados para garantir a qualidade do código.

Exemplo de Uso do Yii Framework:

Instalação do Yii:

A maneira mais comum de instalar o Yii é através do Composer. Aqui está como você pode criar um novo projeto Yii:

```sh
composer create-project --prefer-dist yiisoft/yii2-app-basic myproject
```

Estrutura Básica do Projeto:

A estrutura de diretórios de uma aplicação Yii típica inclui:

- `controllers/`: Contém os controladores.
- `models/`: Contém os modelos.
- `views/`: Contém as views.
- `config/`: Arquivos de configuração da aplicação.
- `web/`: Raiz do documento web, contendo o arquivo de entrada `index.php`.

Criando um Controlador:

```php
namespace app\controllers;

use yii\web\Controller;

class SiteController extends Controller
{
    public function actionIndex()
    {
        return $this->render('index');
    }
}
```

Criando uma View:

```php
// views/site/index.php

echo "Olá, Mundo!";
```

Criando um Modelo:

```php
namespace app\models;

use yii\db\ActiveRecord;

class User extends ActiveRecord
{
    public static function tableName()
    {
        return 'user';
    }
}
```

Configurando o Banco de Dados:

No arquivo `config/db.php`, configure a conexão com o banco de dados:

```php
return [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=localhost;dbname=mydatabase',
    'username' => 'root',
    'password' => '',
    'charset' => 'utf8',
];
```

Benefícios do Uso do Yii Framework:

1. **Rapidez no Desenvolvimento**: Ferramentas como o Gii ajudam a gerar código automaticamente, acelerando o desenvolvimento.
2. **Flexibilidade**: A arquitetura componentizada permite a fácil integração e personalização.
3. **Alta Performance**: Projetado para ser rápido, o Yii é uma excelente escolha para aplicações de alto desempenho.
4. **Segurança**: Funcionalidades embutidas de segurança ajudam a proteger a aplicação contra ameaças comuns.
