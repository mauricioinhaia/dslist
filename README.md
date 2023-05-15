# DS List Back End
# Sobre o Projeto

DS List trata-se de uma aplicação Back End com padrao API REST e Banco de Dados Relacional, foi desenvolvida durante o evento organizado pela [DevSuperior](https://devsuperior.com "Site da DevSuperior").

Nesta aplicação temos uma coleção de Games ordenadas por categorias, como aventura e rpg por exemplo. Podemos também visualizar informações mais completas sobre estes games e ainda ordena-los em posições a nossa escolha.

# Tecnologias Utilizadas
- Java (JDK 17)
- Spring Boot
- JPA / Hibernate
- Maven
- PostgreSQL

# Implantação em Produção
- BackEnd e Banco de Dados: [RailWay](https://railway.app/ "Site Railway")
## Testes em Produção

Podem ser efetuados testes até o dia 01/06/2023 (tempo que a plataforma disponibiliza gratuitamente 500 horas) alterando os endpoints para o endereço abaixo:
```
https://dslist-production-4aed.up.railway.app
```
# EndPoints
Podem ser importados no Postman através do arquivo DSList.postman_collection.json disponibilizado nesse projeto. 
#### Buscar Jogos
```
http://localhost:8080/games
```
#### Buscar Jogo pelo ID
```
http://localhost:8080/games/10
```
#### Buscar Categorias
```
http://localhost:8080/lists
```
#### Buscar Jogos por Categoria
```
http://localhost:8080/lists/2/games
```
#### Atualizar Posição dos Jogos na Lista
```
http://localhost:8080/lists/2/replacement

Body:
{
    "sourceIndex": 3,
    "destinationIndex": 1
}
```
# Como executar o Projeto
```
# Criar uma pasta para salvar o projeto
mkdir /home/seunomeusuario/git

# Acessar a pasta para salvar
cd /home/seunomeusuario/git

# Clonar repositório
git clone https://github.com/mauricioinhaia/dslist.git

# Acessar pasta para executar
cd dslist

# Executar o Projeto
./mvnw spring-boot:run
```
# Autor
[Mauricio Inhaia](https://www.linkedin.com/feed/ "LinkedIn")

