# Projeto Laravel Migrate

Este repositório demonstra o processo de **criação de banco de dados utilizando migrations no Laravel**, apresentando diferentes métodos para criar tabelas, realizar alterações e aplicar as mudanças via `php artisan migrate`.

## Pré-requisitos

Antes de iniciar, é necessário ter instalado:

- [PHP](https://www.php.net/) >= 8.1
- [Composer](https://getcomposer.org/)
- [Laravel](https://laravel.com/docs)

Além disso, configure o banco de dados no arquivo `.env` de acordo com o arquivo `.env.example`.

## Instalação do Projeto

Para clonar e instalar as dependências do projeto:

``` bash
git clone https://github.com/caramelPopp/laravel-migrate.git  
cd laravel-migrate  
composer install
npm install
npm run build
php artisan key:generate  
```

## Criação do Banco de Dados com Migrations

O foco deste projeto está no uso de migrations para criação e alteração de tabelas dentro do banco de dados.

### Criação da tabela `cadastro`

<img width="606" height="63" alt="make-migration-cadastro" src="https://github.com/user-attachments/assets/fada5e7d-4e1e-4ebe-bb36-891d11cdef12" />


### Aplicando as migrations

Para aplicar as alterações feitas nos arquivos de migration:

``
php artisan migrate  
``

<img width="654" height="26" alt="comando" src="https://github.com/user-attachments/assets/a79d8e92-f515-41b0-80a7-bde354564bc3" />

<img width="654" height="59" alt="resultado" src="https://github.com/user-attachments/assets/e5eb6af0-0316-4c55-add9-774ed0716305" />


### Criação da tabela `estoque`

<img width="949" height="86" alt="create-migration-estoque" src="https://github.com/user-attachments/assets/4118d846-5e2d-44de-9129-f52fd77e9b4b" />


### Aplicando as migrations

``
php artisan migrate  
``

<img width="954" height="103" alt="migrate-estoque" src="https://github.com/user-attachments/assets/3b2fbca7-20c9-40f7-8d43-6a9722b9805f" />


### Alterando a tabela `cadastro` via migration de alteração

<img width="952" height="83" alt="alter-cadastro" src="https://github.com/user-attachments/assets/5951044f-a307-49f8-bd6a-c3410a6dfc4d" />


### Aplicando novamente as migrations

``
php artisan migrate  
``

<img width="950" height="106" alt="alter-migrate-cadastro" src="https://github.com/user-attachments/assets/c3113861-d14c-45d6-949c-28e7e8365b79" />

## Testando o projeto com as migration já criadas
Caso as migrations já tiverem sido criadas dentro do projeto, não há a necessidade de criá-las com os comandos, apenas importar o banco de dados presente em `database\bd_fornecedores.sql` para o phpMyAdmin e efetuar as migrations com o comando `php artisan migrate`

<img width="953" height="199" alt="migrations" src="https://github.com/user-attachments/assets/2b10101b-4559-4585-8b2c-14947383181a" />


----

## Sobre o Projeto

Este projeto foi desenvolvido para fins **educacionais**, demonstrando o uso prático de migrations no Laravel.

**Autoria:** [Bárbara Rampazi](https://github.com/caramelPopp)
