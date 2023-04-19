# Análise de Requisitos de Software com Histórias de Usuários

## 1. Introdução


Example Mapping : é uma técnica de refinamento de lista de pendências que ajuda a estruturar a conversa de sua equipe em torno de um item de lista de pendências. 
A conversa se concentra em extrair todos os critérios de aceitação relevantes (ou regras), cenários relacionados e questões pertinentes associadas ao item de backlog que você está discutindo.

Com o processo de Example Mapping as suas Histórias podem ser usadas para você pode criar testes automatizados, mas não é obrigatório.

## 2.  O que são Histórias de Usuário

O que é uma história de Usuário?
é uma descrição resumida da feature que você vai implementar para o seu cliente, cada história de usuário precisa ser independente, não pode usar uma história de usuário para complementar outra,essa história precisa ser alto contida , ou seja tudo que você precisa para implementar aquela feature tem que estar dentro da história de ususários, ela precisa ser mensurável para que consigamos mensurar de uma forma eficiente uma história de usuário, você precisa saber todas os detalhes que estão escondidos dentro dessa história é aqui que entra o example mapping, ele que vai facilitar descobrirmos  os detalhes ocultos em cada uma das histórias de usuários que iremos implementar. Além disso uma história de usuário tem que ser testável, testável não tem nada a ver com teste automatizados, uma história testável quer dizer que você tem que definir os critérios de aceitação e os testes que vão exemplificar se os critérios estão sendo atendidos. Ex: se o usuário fizer uma ação "X" no sistema , o sistema responde com um resultado "Y", esses testes podem ser feitos de forma manual , quanto automatizados. Para podermos identificar os critérios de aceitação que são as regras e os exemplos que devem ser testados para verificar se aquele critério foi atendido ou não, agente vai usar o example mapping

O que seria uma História de Usuário Mensurável?

![image](https://user-images.githubusercontent.com/52088444/232067416-100ee22b-6934-4048-b3ac-807d9aab69f8.png)

O que seria uma história de usuário Testável?

![image](https://user-images.githubusercontent.com/52088444/232067544-fd4b36b6-aea9-4b90-a10c-e2557f430087.png)


## 3. O que é Example Mapping (Mapeamento de Exemplos)

Example Mapping é uma técnica que usamos para identificar as coisas que estão ocultas numa história de usuários, que vão nos ajudar a mensurar uma história e saber quais são os passos que devem ser implementados para que aquela história seja atendida. 

Para isso usamos os conceitos dos 3 amigos. 

3 amigos representam os 3 aspectos diferentes na hora que você está desenvolvendo um sistema. 3 visões que serão trabalhadas em conjunto :

- O aspecto do Cliente que é o Product Owner. (ou contratante da empresa para mostrar os requisitos do sistema);
- A visão do desenvolvedor que vai realmente implementar o sistema;
- E a visão do testador;

ou pode ser você e o cliente , mas precisa ter essas funções envolvidas

Quais papéis são representados pelos 3 amigos, numa reunião de Example Mapping?
Cliente, desenvolvedor e testador;

## 7. Como funciona o Example Mapping

Você deve escolher uma história que deve ser trabalhada naquela reunião. Lembrando que as histórias de usuários não tem nenhum detalhamento até esse momento. 
Envolve o Cliente, desenvolvedor e testador nessa reunião, onde limita o cronometro em 30 minutos, todos focados para desmembrar a história.

Para cada história de usuário usaremos um quadro com cartões coloridos, para poder desmembrar a história de usuário, para que os envolvidos na reunião possam expressar suas opiniões, soluções, questionamentos...

Exemplo de um quadro:

![image](https://user-images.githubusercontent.com/52088444/233070292-c8e0a923-9260-42ab-8094-583181d6e6f6.png)

O cartão amarelo você vai colocar a História que vai ser trabalhada. Uma breve descrição do que vai ser implementado,  e no decorrer da reunião que você vai ter com cliente você vai encontrar:

- Cartão azul(REGRA):as regras ou seja os critérios de aceitação que precisam ser implementados. Então, cada critério de aceitação "REGRA" precisa estar num cartão azul, cada uma dessas regras você tem exemplos.
- Cartão Verde(EXEMPLO): contém exemplos concretos que descrevem como é que essa regra tem que ser implementada.
- Cartão Rosa(QUESTIONAMENTO):no decorrer da reunião vai surgir questionamentos, e esse questionamento pode ser associado à história que está sendo implementada, ele pode ser associado à regra de negócio

Outro detalhe importante é o seguinte,um EXEMPLO tem que ter um contexto, uma ação que o usuário vai executar. E para fechar você coloca o resultado esperado quando o usuário executar essa ação baseada nesse contexto. Cada teste o ideal é que você divida dessa forma, e vocês vão ver que isso vai ajudar na hora que você vai implementar nos testes automatizados então você vai ter o contexto daquele teste a ação que o usuário vai executar e o resultado que você espera que seja devolvido para o usuário. No caso não precisa ser uma ação do usuário, pode ser uma ação do sistema que você vai atender.
Outro detalhe importante é que você não precisa seguir exatamente essa regra de cores.

O intuito dessa técnica é trazer à tona tudo que está obscuro, ou seja todos que estão presentes na reunião vão ter uma visão concisa a respeito do que está sendo desenvolvido. Isso vai evitar ambiguidades que normalmente só são percebidas no meio ou no final do projeto.

Quais os tipos de cartões utilizados num Example Mapping?
![image](https://user-images.githubusercontent.com/52088444/233068074-3e17331f-9c8f-4b70-8ace-5503d908eb09.png)

Idealmente, um cartão de exemplo deve conter a seguinte ordem:
![image](https://user-images.githubusercontent.com/52088444/233068238-567a6074-e695-4589-a374-db9e47cc1dd7.png)


## Visão Geral do Projeto Prático (Apontamentos de requisitos de um sistema de Anuncios Online)

**Sistema  de Anuncios Online

Iniciaria uma entrevista com o cliente(descrição exemplo do cliente do que ele precisa):

- quem faz anúncio gratuito vai ter um destaque X e quem vai fazer anúncios pagos vão ter um destaque diferenciado.

Nessa reunião com o cliente será levantado todos os pontos chave, por exemplo você pode perguntar:
- o usuário que vai fazer o anúncio tem que ter uma conta pelo site para poder se autenticadas antes de fazer o anúncio? Se ele responder que sim, isso já se torna uma história de usuário.

Exemplo História1: Como usuário devo me cadastrar no site para poder criar um anúncio.

A partir da história acima vem outras histórias:

- Exemplo história2: Sendo um usuário cadastrado eu quero me autenticar no sistema/site
- Exemplo história3: Como um usuario autenticado eu quero criar um anuncio gratuito para vender o meu produto
- Exemplo história4: Como um usuario autenticado eu quero criar um anuncio pago para vender o meu produto mais rapidamente.

Esse padrão nos ajuda a enxergar a motivação por trás de cada uma dessas features,.

Na parte acima estamos montando um product Backlog , que é uma lista de funcionalidades que vão ser desenvolvidas.

## Mapeando História de Usuário 1: Cadastro de Usuário

Como fazer o Exemplo Mapping da História 1: Como usuário devo me cadastrar no site para poder criar um anúncio.

Nesse caso você começa a reunião com o cliente delimitando 30 minutos, para extrair as informações.

Primeiro iniciamos pela "REGRA":
- Dados obrigatórios deverão ser informados
- O campo(dado) que você vai utilizar como autenticação ele deve ser único no sistema para evitar que usuários diferentes se logen com o mesmo dado de autenticação, que no caso é o e-mail.
- A senha do usuário deve ter no mínimo 8 caracteres

Questionamento:
- O usuário tem que validar o e-mail ?

Exemplo:
- Quando o usuário preencher todos os dados e submeter o formulário a resposta vai ser um "OK".(Criado com Sucesso)
- Quando o usuário deixar algum campo obrigatório vazio e submeter o form, retorna "ERRO"
...
<img width="517" alt="image" src="https://user-images.githubusercontent.com/52088444/233094658-20d6c80e-0dae-4f9b-b8a5-9b891da0907d.png">

Podemos realizar os testes automatizados através dos exemplos. Ou seja podemos usar os exemplos para testar suas regras.

## Mapeando História de Usuário 2: Autenticação de Usuário

Exemplo história2: Sendo um usuário cadastrado eu quero me autenticar no sistema/site

Nesse caso você começa a reunião com o cliente delimitando 30 minutos, para extrair as informações.

<img width="406" alt="image" src="https://user-images.githubusercontent.com/52088444/233096104-a0143506-66e8-44a9-92b3-819e5ed17c67.png">

Através dessa história foi gerado uma segunda história de usuário, deixamos ela de lado, e continuamos a dar foco na nossa história2.

##  Mapeando História de Usuário 3: Publicando Anúncio Gratuito

Exemplo história3: Como um usuario autenticado eu quero criar um anuncio gratuito para vender o meu produto

Nesse caso você começa a reunião com o cliente delimitando 30 minutos, para extrair as informações.

![image](https://user-images.githubusercontent.com/52088444/233097570-30f64960-f121-4a4b-a9b3-dc5e760d6ecb.png)

## Mapeando História de Usuário 4: Publicando Anúncio Pago

 Exemplo história4: Como um usuario autenticado eu quero criar um anuncio pago para vender o meu produto mais rapidamente.
 
 ![image](https://user-images.githubusercontent.com/52088444/233099169-baad7ee4-55dc-4aa5-b38b-11744ae9fdab.png)

O que é um critério de aceitação?
![image](https://user-images.githubusercontent.com/52088444/233099472-9ed07b52-ade1-4d15-828e-c56802d0494c.png)

Qual a função dos cartões de exemplos?
![image](https://user-images.githubusercontent.com/52088444/233099604-baa45fe8-7385-4fe3-85f4-b69ca59c0716.png)

Durante uma reunião, se surgir uma nova história de usuário, o que deve ser feito?
![image](https://user-images.githubusercontent.com/52088444/233099722-950201a7-681b-4202-b879-878db9ba488a.png)

Sobre os participantes da reunião, escolha a afirmativa correta:
![image](https://user-images.githubusercontent.com/52088444/233099823-f96c19f5-5c0f-4f93-9ac9-5a727364b697.png)

## Aulão - Respondendo Dúvidas e Resolvendo a Última Questão (parte 1)

1. Existe alguma ferramenta online para fazer Example Mapping? miro.com
2. Quanto tempo deve demorar uma reunião de example mapping? como definir isso? Isso é relativo depende da história, mas o ideal é que seja de 25 a 30 minutos
3. Quantas histórias devem ser abordadas num reunião? apenas uma história de usuário
4. Definição de prioridades, como fazer? Isso tem a ver com a definição de requisitos, e adefinição de backlog, tem sprint que demora uma semana, 1 mês, depende do projeto que vocês está trabalhando
Exemplo: faz de conta que você tem 6 histórias de usuários, e você precisa definir a finalidade, as vezes o cliente não sabe qual é a prioridade, e você precisa perguntar para ele, e além de perguntar questionar os motivos daquelas histórias serem prioridade, geralmente é através dessa pergunta que saberemos se realmente é prioridade. por exemplo ele responde que a prioridade é o carrinho de compras por que eu tenho alguns clientes que estão vendendo um produto dentro do sistema, ou seja comprar online como se fosse o mercado livre, ele quer que o cliente coloque os produtos no carrinho e calcule o frete e tudo mais, aí você pergunta para o cliente você sabe se existe essa necessidade no momento, você já tem usuários que usam o sistema como é hoje, de onde tirou esses dados? ele pode informar que fez uma pesquisa de mercado, que alguns usuários informaram que seria interessante que pudesse fazer um anuncio como se fosse uma loja virtual. Se ele demonstrar a necessidade, perfeito, mas se o cliente não souber o motivo pelo o qual está selecionando essa história, é interessante você indicar uma outra história, e mostrar os motivos pelo o qual está segurindo a história.  
5. Quem deve participar da reunião de Example Mapping? Conceito dos 3 amigos: PO (Dono do negócio/PO/Cliente quem conhece do negócio), Desenvolvedor(pessoa responsavel para desenvolver o sistema, a solução do sistema), tester(reponsável por testar o sistema - problemas, visão mais negativa para evitar que o cliente final descubra os problemas). Na maioria das vezes não temos essas funcionalidades infelizmente. Nessa reunião podemos ter o designer, Ux, UI...
6. Devo fazer example mapping incremental ou em cascata? 
No incremental nós temos a flexibilidade de fazer de forma iterativa as entregas, 
![image](https://user-images.githubusercontent.com/52088444/233109688-bce52596-6e38-4786-949d-a074adfb167e.png)
já no cascata nós precisamos fazer toda a análise requisito no início.
![image](https://user-images.githubusercontent.com/52088444/233108985-b5d6d445-7d13-45e2-b220-7d7a21cca506.png)
7. Cobrar por hora ou por projeto? como sabr a duração do projeto? é possivel? não é possivel definir o tempo, é possivel fazer estimativa e mesmo assim elas na maioria das vezes são maiores, por que os clientes geralmente não sabem o que querem no início do projeto.
8. Qual nivel de detalhamento deve ter uma feature (como saber se estou testando uma regra de negócio corretamente?)? não detalhar exageradamente os campos o cliente não precisa saber o detalhe , apenas ter os dados essenciais para poder criar, montar um cenário específico para a regra.
9.Como adicionar os exemplos ao documento de requisitos? Você pode usar modelos prontos do word
![image](https://user-images.githubusercontent.com/52088444/233117552-5feefbc0-0464-4786-85a4-318e053fa16c.png)
![image](https://user-images.githubusercontent.com/52088444/233118591-4b71224f-0284-4f90-be1c-6e42c4be6767.png)

10. Como transformar os exemplos em testes automatizados?cumcumber rails, (BDD - dESENVOLVER DE ACORDO DOM O COMPORTAMENTO), Rspec

**Exercicio 

![image](https://user-images.githubusercontent.com/52088444/233105945-b2d28270-4cf1-4dcb-975b-91b7d7e77e5b.png)
![image](https://user-images.githubusercontent.com/52088444/233106335-538d2419-ce27-4ac2-9a1f-e5bf03b26774.png)
![image](https://user-images.githubusercontent.com/52088444/233106736-187e805a-1df4-45a0-85eb-f6413cf4996b.png)

REGRAS PARA SEREM ENTREGUES

![image](https://user-images.githubusercontent.com/52088444/233110620-80b71e07-b096-46c4-a269-f2c6ba629d72.png)
![image](https://user-images.githubusercontent.com/52088444/233110677-8e7be6ea-1c0e-459d-856d-ac9e321abc12.png)

![image](https://user-images.githubusercontent.com/52088444/233112481-7fae0ad1-2d9f-403f-93fe-eb25b66e0082.png)
como podemos ver acima no cartão verde(exemplo) é dessa forma que devemos estruturá-lo. Para poder exemplificar a regra (cartão azul).
Ou seja perguntar ao cliente o que ele considera um caminho feliz(um cenário onde tudo ocorreu bem), um contexto para que o usuário faça uma ação no sistema.
![image](https://user-images.githubusercontent.com/52088444/233114116-c650e672-bf55-476e-9df2-31908b23708b.png)
Todo esse cartão verde é um teste/ou pode ser um teste. 

![image](https://user-images.githubusercontent.com/52088444/233116064-dcb9b63a-4346-4443-9f18-40ba86ef70b6.png)


Gherkin
- Given -> Dado que (contexto)
- when -> quando (ação testada)
- Then -> então ...(resultaad)
- and-> E
- But-> mas
- ... dado...
- ...e
- ...quando..
- então...

![image](https://user-images.githubusercontent.com/52088444/233117894-89be9a19-8c6e-4571-9412-8c4c88736b8a.png)

![image](https://user-images.githubusercontent.com/52088444/233117974-4d21a824-cf7b-40dc-8b18-db46b3039cbf.png)

No caso de microsserviço e mensageria :
![image](https://user-images.githubusercontent.com/52088444/233119817-a1f8f97d-98d9-4f6b-a33f-0510c410d667.png)

Podemos enxergar uma regra e transformá-la em uma história de usuário.

![image](https://user-images.githubusercontent.com/52088444/233120472-a0be507c-e5b7-4e8d-a88e-826f01678f56.png)

## Referencias

- https://insideproduct.co/example-mapping/
