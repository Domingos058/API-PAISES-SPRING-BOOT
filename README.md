Esta e' uma API RESTful que nos permite gerenciar as informações das propriedades dos países (identificador – gerado automaticamente, nome, capital, região, sub-região, área).
Usando tecnologia java Maven-Spring boot 



1 edit o application.properties com a connection string com os dados que tem em seu mysql.
para garantir crie uma database no mysql e coloque o nome na connection String 
para testar a API use o Postman ou outro

POST localhost:8080/api/paises
JSON para a insercao dos dados
{
   "nome" : "",
   "capital" : "",
   "regiao" : "",
   "subRegiao" : "",
   "area" : ""
}


 Para fazer a listagem de todos os paises 
GET localhost:8080/api/paises

3. Para Actualizar os dados de um pais 
 A pesquisa do Pais e feita pelo nome.
 PUT localhost:8080/api/paises/nomeDoPais
{
   "nome" : "",
   "capital" : "",
   "regiao" : "",
   "subRegiao" : "",
   "area" : ""
}

4. Eliminar um Pais
DELETE PUT localhost:8080/api/paises/IdDoPais

5. Ordenar
GET localhost:8080/api/paises/ordenar
