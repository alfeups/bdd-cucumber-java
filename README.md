# spring profile arg
-Dspring.profiles.active=test

# Requisitos:
<li>MARIADB ou H2;
<li>Maven para gerenciar dependencias;
<li>Linguagem - Java;
<li>Para escrever doc. - BDD + Cucumber gerkhin;
<li>Automatizar test interface web - selenium
<li>Design patter - page-object


# MARIADB

## https://downloads.mariadb.com/MariaDB/

<p>rodar mariadb no windows (a partir da pasta bin do mariadb)</p>

</p>mysqld.exe --console</p>

# para se conectar com mariadb (a partir da pasta bin do mariadb)
<p>mysql -u root</p>

<p>create database leilao;</p>


# MAVEN
## https://maven.apache.org/download.cgi

<p>Rodando testes com maven na linha de comando (default profile é test) apenas testes de unidade</p>

<p>mvn test</p>

## Testes de integracao
mvn test-integration

## Para alterar o profile
mvn test -Pprod

## Para usar chrome driver (firefox é padrao)

mvn integration-test -Ddriver=chrome
mvn integration-test -Dcucumber.filter.tags="@login or @lance"



# DOCKER
# para subir mariadb com docker (a partir local do docker-compose.yml)
docker-compose up -d

#login e senha está no docker-compose.yml

#para terminar os services abaixo
docker-compose down 

http://localhost:8081

 
