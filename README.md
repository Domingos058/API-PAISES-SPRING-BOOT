Esta e' uma API RESTful que nos permite gerenciar as informações das propriedades dos países (identificador – gerado automaticamente, nome, capital, região, sub-região, área).
Usando tecnologia java Maven-Spring boot Com os seguintes requisitos funcionais:
-criar um novo país a partir da API criada com todas as suas propriedades;
-listar todos os países anteriormente criados;
-modificar os dados de um país anteriormente criado;
-eliminar um país anteriormente criado;
-ordenar a lista dos países por qualquer uma das suas propriedades.




1 A base de dados em  Mysql  contem 6
para criar um novo Pais apartir da API com todas as propriedades[Postman]

POST localhost:8080/api/paises
JSON para a insercao dos dados
{
   "nome" : "",
   "capital" : "",
   "regiao" : "",
   "subRegiao" : "",
   "area" : ""
}


2. Para fazer a listagem de todos os paises anteriormente criados

GET localhost:8080/api/paises

3. Para Actualizar os dados de um pais 
 A pesquisa do Pais e feita pelo nome.
 PUT localhost:8080/api/paises/nomeDoPais
Inserindo os novos dados em Json nos devidos campos
{
   "nome" : "",
   "capital" : "",
   "regiao" : "",
   "subRegiao" : "",
   "area" : ""
}

4. Eliminar um Pais
A eliminacao do Pais e feita atraves do id(findById) disponibilizado pelo JpaRepository

DELETE PUT localhost:8080/api/paises/IdDoPais

5. Ordenar
E possivel ordenar a lista dos paises atraves da propriedade nome em ordem Alfabetica

GET localhost:8080/api/paises/ordenar
