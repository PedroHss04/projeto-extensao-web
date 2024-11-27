# Projeto de Extensão - PHP e MySQL

Este projeto é um site desenvolvido em PHP e MySQL. Para rodá-lo em sua máquina local, siga os passos abaixo para configurar o ambiente de desenvolvimento usando o XAMPP.

## Requisitos

- **XAMPP**: Plataforma de desenvolvimento que inclui Apache (servidor web), MySQL (banco de dados) e PHP.
- **PHP**: A linguagem utilizada para o desenvolvimento do site.
- **MySQL**: Banco de dados utilizado para armazenar informações do site.

## Passos para Configuração

### 1. Instalar o XAMPP

Baixe e instale o XAMPP [aqui](https://www.apachefriends.org/index.html). O XAMPP inclui o Apache, o MySQL e o PHP, essenciais para o funcionamento do projeto.

### 2. Iniciar o XAMPP

Após a instalação do XAMPP, abra o painel de controle do XAMPP e siga os seguintes passos:

- **Iniciar o Apache**: Clique no botão **Start** ao lado de "Apache" para iniciar o servidor web.
- **Iniciar o MySQL**: Clique no botão **Start** ao lado de "MySQL" para iniciar o servidor de banco de dados.

### 3. Copiar o Projeto para o Diretório do XAMPP

1. Copie a pasta do seu projeto para a pasta `htdocs` do XAMPP. O caminho padrão da pasta `htdocs` é:

   - **Windows**: `C:\xampp\htdocs\`
   - **Linux/Mac**: `/opt/lampp/htdocs/`

2. Renomeie a pasta do projeto para o nome desejado. Exemplo: `projeto_de_extensao`.

## Requisitos

- **XAMPP**: Plataforma de desenvolvimento que inclui Apache (servidor web), MySQL (banco de dados) e PHP.
- **PHP**: A linguagem utilizada para o desenvolvimento do site.
- **MySQL**: Banco de dados utilizado para armazenar informações do site.

## Passos para Configuração

### 1. Instalar o XAMPP

Baixe e instale o XAMPP [aqui](https://www.apachefriends.org/index.html). O XAMPP inclui o Apache, o MySQL e o PHP, essenciais para o funcionamento do projeto.

### 2. Iniciar o XAMPP

Após a instalação do XAMPP, abra o painel de controle do XAMPP e siga os seguintes passos:

- **Iniciar o Apache**: Clique no botão **Start** ao lado de "Apache" para iniciar o servidor web.
- **Iniciar o MySQL**: Clique no botão **Start** ao lado de "MySQL" para iniciar o servidor de banco de dados.

### 3. Copiar o Projeto para o Diretório do XAMPP

1. Copie a pasta do seu projeto para a pasta `htdocs` do XAMPP. O caminho padrão da pasta `htdocs` é:

   - **Windows**: `C:\xampp\htdocs\`
   - **Linux/Mac**: `/opt/lampp/htdocs/`

2. Renomeie a pasta do projeto para o nome desejado. Exemplo: `projeto_de_extensao`.

### 4. Configurar o Banco de Dados MySQL

1. Abra o **phpMyAdmin** no seu navegador. Para isso, acesse a URL:

http://localhost/phpmyadmin/

2. Crie um novo banco de dados para o seu projeto. Clique em **Novo** e crie um banco de dados, por exemplo, `projeto_extensao`.

3. Se você tiver um arquivo `.sql` contendo a estrutura do banco de dados, clique em **Importar**, selecione o arquivo `.sql` e clique em **Executar** para importar as tabelas do banco de dados.

### 5. Configurar o Arquivo de Conexão (se necessário)

Caso o seu projeto utilize um arquivo de configuração para a conexão com o banco de dados (geralmente chamado de `config.php`, `db.php`, ou algo semelhante), verifique se as credenciais de conexão estão corretas. A configuração padrão do XAMPP para MySQL geralmente é:

```php
<?php
$host = "localhost";
$user = "root";
$pass = ""; // A senha padrão no XAMPP é vazia
$dbname = "projeto_extensao"; // Nome do banco de dados criado

// Conexão com o banco de dados
$conn = new mysqli($host, $user, $pass, $dbname);

if ($conn->connect_error) {
 die("Falha na conexão: " . $conn->connect_error);
}
?>
````


6. Acessar o Site
Agora que você copiou o projeto para a pasta htdocs e configurou o banco de dados, abra seu navegador e acesse o seguinte endereço:
  http://localhost/projeto_de_extensao
