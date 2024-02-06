# Projeto MySQL Docker

Este repositório contém um projeto Docker para criar uma imagem do [MySQL](https://www.mysql.com/) na versão "8.0.36-debian". Utilizamos um Dockerfile para construir a imagem e um docker-compose para facilitar a execução do contêiner.

## Pré-requisitos

Certifique-se de ter o Docker instalado em sua máquina antes de começar.

- Docker: [Instalação do Docker](https://docs.docker.com/get-docker/)

## Como usar

1. Clone este repositório em sua máquina local:

```bash
git clone https://github.com/JoaoPedroLott/mysql_docker.git
```

2. Crie um arquivo .env com as variáveis de ambiente necessárias para seu projeto:

```bash
MYSQL_ROOT_PASSWORD=senha_root
MYSQL_DATABASE=nome_banco
MYSQL_USER=nome_usuario
MYSQL_PASSWORD=senha_usuario
```

3. Inicie o contêiner usando o docker-compose:

```bash
docker-compose up
```

O MySql estará acessível na porta 3306 do seu localhost.

## Configuração Adicional
- O diretório ./data é usado para persistir os dados do banco de dados. Você pode alterar isso no arquivo docker-compose.yml se necessário.
- Certifique-se de revisar e personalizar o docker-compose.yml para atender aos requisitos específicos do seu projeto.

## Contribuindo
Sinta-se à vontade para contribuir com melhorias, correções de bugs ou novos recursos. Abra uma issue ou envie um pull request!