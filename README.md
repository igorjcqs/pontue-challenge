## Sobre o desafio

O desafio é construir uma API simples em Laravel (PHP) que permite Criar, Ler, Atualizar e Deletar 2 entidades diferentes à sua escolha, ou seja, cria um lista de filmes, carros, games, etc.

Desafio bônus (opcional): Fazer com que a API funcione apenas para usuário logados (autenticados).

## Objetivos:
- Ter um ending point para cada operação (CRUD);
- Utilizar um banco de dados para armazenar os dados;
- Exibir dados retornados de forma organizada;
- Ter um README para explicar como rodar o projeto;
- Construir coleção do POSTMAN para testes;
- Funcionalidades de resetar senha e trocar senha;
- Fazer testes automatizados utilizando PHPUnit;
- Utilizar Docker para rodar o sistema;

Objetivos concluídos: todos.

## Sobre o desenvolvimento

Api desenvolvida em um ambiente Docker, através de um ambiente de desenvolvimento pré configurado chamado [Laradock](https://github.com/laradock/laradock)

## Como testar a api?

- 1 - Clone o repositório para um local de sua escolha, através do comando:
```git clone https://github.com/igorjcqs/pontue-challenge```

- 2 - Clone o repositório do laradock para dentro do projeto, através do comando:
```git clone https://github.com/laradock/laradock```

- 3 - Instale as dependências do composer, através do comando:
```composer install```

- 4 - Acesse o ambiente docker;
```cd laradock```

- 5 - Abra o arquivo ```laradock/.env.example``` e copie o conteúdo para seu arquivo ```laradock/.env``` (Caso não tenha, crie);

- 6 - Configure todas as portas que você irá usar.

- 7 - Configure o seu banco de dados.

- 8 - Volte ao diretório principal.

- 9 - Abra o arquivo ```.env.example``` e copie o conteúdo para seu arquivo ```.env```  (Caso não tenha, crie);

- 10 - Abra o seu arquivo ```.env``` e configure o banco de dados e o servidor de e-mail.

- 11 - Inicie o ambiente docker, através do comando:
```docker-compose up -d nginx mysql phpmyadmin```

- 12 - Realize as migrações do banco de dados, através do comando:
```php artisan migrate```

- 13 - Rode todas as seeds do banco de dados, através do comando:
```php artisan db:seed```

- 14 - Pronto! O projeto já está rodando em um ambiente docker e você poderá acessar pelo link: https://localhost:PORTA_CONFIGURADA_NO_ENV

- 15 - Baixe o Postman e importe a coleção (Pontue - Backend Requests..postman_collection.json) de requests presentes no projeto.

OBS¹: Para rodar corretamente é necessário ter o Docker Desktop instalado no computador.

OBS²: Caso queira, você pode optar por trocar as tecnologias utilizadas.

OBS³: A primeira vez que você rodar o comando "docker-compose", provavelmente irá levar um tempo, pois irá baixar todas as depedências necessárias.
