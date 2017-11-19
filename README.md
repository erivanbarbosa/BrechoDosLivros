# BrechoDosLivros

Projeto em construção que visa atender o nicho de venda e/ou doação de livros. 
Inicialmente foi pensado para atender aos Campus da Universidade Federal de Goiás, porém pode ser utilizado para qualquer área ou dimensão, desde que atente aos requisitos

## Estrutura do projeto
 - **APP**: Lado cliente, projeto para Android
 - **Backend**: Server side


### Pré-requisitos

**App:** Android Studio com API 24 ou superior
**Backend:** Servidor web (ex.: Nginx ou Apache2) com PHP 5.6 ou superior, atentando que a partir da versão 7.0 algumas funções foram modificadas, o que pode gerar alguma incompatibilidade. 
**SGBD:** MySQL 5.1+ ou MariaDB


### Como fazer?
1. Importe o arquivo Backend\database.sql para o seu SGDB. Será criado uma base de dados 'database_name'. Altere o nome, caso julgue necessário. 
2. Copie os arquivos da pasta Backend para o seu servidor
3. Altere conforme sua configuração o arquivo Backend/include/config.php
4. Altere a variável 'URL_BASE' no arquivo app/src/main/java/com/brecho/BrechoDosLivros/Globals.java
5. Abra o projeto App com o Android Studio e faça o deploy da aplicação

## Built With
* [Android Studio](https://developer.android.com/studio/index.html?hl=pt-br) - App
* [PHP](https://php.net/) - Backend
* [MySQL](https://www.mysql.com/) - Persistência de dados

## Crontribua!
Faça um fork do projeto, altere o que julgar necessário e faça um pull request


## License
Este projeto está licenciado sobre o MIT Licence - veja [LICENSE](LICENSE) para mais detalhes.
