Esta é uma API simples para gerenciar pessoas. Esta API está hospedada em: https://avaliacao.onrender.com.

Por se tratar de um serviço gratuito, ele leva algum tempo para carregar.



Cadastrar, editar, consultar e deletar pessoas. 

Para cadastrar a pessoa é necessário que você faça um POST na aplicação através do seguinte endpoint:

**/pessoas/cadastrar**

E insira os dados no seguinte formato:

<img src="https://i.imgur.com/fNlBmNK.png">



Para editar você pode fazer um PUT através do seguinte endpoint:

**/pessoas/atualizar**



E para deletar você pode fazer um DELETE através de **/pessoas/deletar/{id}**



A classe Pessoa tem os seguintes atributos:

- Nome
-  Data de nascimento
- Endereço



Já a classe Endereco tem os seguintes atributos: 

-  Logradouro
-  CEP
-  Número
- Cidade
- Pessoa



Segue o diagrama das classes:

<img src="https://i.imgur.com/wxSXnT5.png" style="zoom:50%" />





Também foram criadas algumas formas de busca, são elas: pelo nome, pelo endereço, ou pelo cep, ou pelo id.

Essas buscas podem ser feitas dando um GET através dos seguintes endpoints:



**/pessoas/all**

Retorna todas as pessoas cadastradas no banco de dados



**/pessoas/{id}**

Retorna uma pessoa com o id específico



**/pessoas/nome/{nome}**

Retorna uma pessoa com nome específico



**/endereco/cep/{cep}**

Retorna um endereço de uma pessoa, e a pessoa relacionada a esse endereço.



**/endereco/{id}**

Retorna um endereço através de um id específico.





Esta API está disponível em: http://avaliacao.onrender.com/



