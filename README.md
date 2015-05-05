# FileManager

FileManager é um baseado na Web PHP Laravel o gerenciador de arquivos que suporta operações de arquivo básicas.
![image](https://s3-us-west-2.amazonaws.com/assets.cdn.univerch.com/filemanager.png)

## Requisitos do Servidor

 * PHP >= 5.4
 * composer
 * npm

## Funções básicas

 * Autenticação Básica de Usuários
 * Sistema de arquivos personalizado caminho físico
 * Arquivo ( pasta) para criar , fazer upload, download, renomear, apagar ,
 * Suporte a AJAX

## Live Demo

 * Endereço teste: http: //filemanager.michaelzlies.com
 * Teste do Usuário : test@test.local
 * Senha: 123456

## Instalação

 1. clonagem repositório Git


     ```
     git clone https://github.com/lzhang43/FileManager.git
     ```

 2. As bibliotecas dependentes

     ```
     composer install
     npm install
     ```

 3. Compilar CSS, JS arquivos

    ```
    gulp
    ```

## configuração

  1. No diretório raiz , copie o arquivo de configuração variável de ambiente

     ```
     cp .env.example .env
     ```

  2. Modificar variáveis ​​de ambiente

 ```
     Disk_name = default // local " disco " nome para o local,
     DISK_DRIVER = defaults // locais para o sistema de arquivos local , mas também através Laravel suporta Amazon S3 e RackSpace
     DISK_ROOT = / var / disk // customizável "Disk " (Root) , o diretório de armazenamento padrão / app ao usar o diretório de programas como o diretório raiz

     DB_HOST = localhost // endereço banco de dados
     DB_DATABASE = herdade // nome do banco de dados
     DB_USERNAME = hoemstead // nome de usuário de banco de dados
     DB_PASSWORD = secret // senha de banco de dados
     ```

  3. Instale banco de dados

     ```
     php artisan migrate
     ```

  4. Você pode ser acessado usando um navegador da Web após a instalação
