<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

# Laravel API Restful com passport

Projeto api restful em Laravel 5.7 com passport

## Requisitos

-   [Git](https://git-scm.com/)
-   [Composer](http://getcomposer.org/doc/00-intro.md)
-   [Postman](https://www.getpostman.com/downloads/)

## Instalação

1. Efetuar a instalação clonando ou baixando do repositorio.
    ```bash
    git clone https://github.com/CodeSiteBr/laravel-passport.git
    ```

    ```bash
    git clone git@github.com:CodeSiteBr/laravel-passport.git
    ```

    OU Dowload [laravel-passport](https://github.com/CodeSiteBr/laravel-passport/archive/master.zip)

2. Entrar na pasta do projeto, execute:
    ```bash
    cd laravel-passport
    ```
3. Se composer está instalado, execute:
    ```bash
    composer install
    ```
4. Criar o arquivo .env, execute:
    ```bash
    cp .env.example .env
    ```
5. Gerar uma nova chave no arquivo .env, execute:
    ```bash
    php artisan key:generate
    ```
6. Criar o arquivo de banco de dados sqlite
    ```bash
    touch database/database.sqlite
    ```
7. Configurar no arquivo .env o acesso ao SQLite
    ```bash
    DB_CONNECTION=sqlite
    #DB_HOST=127.0.0.1
    #DB_PORT=3306
    #DB_DATABASE=homestead
    #DB_USERNAME=homestead
    #DB_PASSWORD=secret
    ```
8. Criar as tabelas e popular com o migrate
    ```bash
    php artisan migrate --seed
    ```

    Comando para criar novamente as tabelas e popular

    ```bash
    php artisan migrate:refresh --seed
    ```

9. Configurar o envio de e-mail no arquivo .env

    Se for em desenvolvimento crie uma conta no [mailtrap](https://mailtrap.io/) e configure as linhas.

    ```bash
    MAIL_USERNAME=null
    MAIL_PASSWORD=null
    ```

    Ou configuração completa de seu servidor de e-mail

    ```bash
    MAIL_DRIVER=smtp
    MAIL_HOST=smtp.mailtrap.io
    MAIL_PORT=2525
    MAIL_USERNAME=null
    MAIL_PASSWORD=null
    MAIL_ENCRYPTION=null
    ```

10. Para iniciar o servidor do laravel
    ```bash
    php artisan serve
    ```

    Ou em uma porta específica

    ```bash
    php artisan serve --port=300
    ```

11. Agora você deve ser capaz de visitar o caminho para onde você instalou o aplicativo e ver a página inicial padrão.

    [localhost:8000](http://localhost:8000)  
    [localhost:300](http://localhost:300/)

    > usuario: admin@admin.com  
    > senha: secret

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
