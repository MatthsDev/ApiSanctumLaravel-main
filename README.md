# Como Rodar a API

Siga os passos abaixo para rodar a API em sua máquina local.

### Passo 1: Clonar o Repositório

Primeiro, faça o **git clone** do repositório para o diretório desejado na sua máquina:

```bash
git clone https://github.com/MatthsDev/ApiSanctumLaravel-main
```
### Passo 2: Criar o Banco de Dados

Crie um banco de dados com o nome laraapisanctum no seu servidor MySQL ou no banco de dados de sua preferência.

```bash
CREATE DATABASE laraapisanctum;
```

### Passo 3: Configurar o Arquivo .env
No diretório raiz do projeto, copie o arquivo .env.example para .env:

```bash
cp .env.example .env
```
Em seguida, edite o arquivo .env e configure as credenciais do seu banco de dados. Abra o arquivo .env e modifique as seguintes linhas com suas credenciais do banco de dados:

```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laraapisanctum
DB_USERNAME=seu_usuario
DB_PASSWORD=sua_senha
```


```bash
bashcp .env.example .env
```

### Passo 4: Configurar o Arquivo .env

Instalar Dependências

Execute o seguinte comando para instalar as dependências do projeto:

```bash
composer install
```

### Passo 5: Rodar as Migrations e iniciar o servidor

```bash
php artisan migrate

php artisan serve
```