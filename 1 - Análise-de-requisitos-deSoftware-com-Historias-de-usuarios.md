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

<img width="406" alt="image" src="https://user-images.githubusercontent.com/52088444/233096104-a0143506-66e8-44a9-92b3-819e5ed17c67.png">

Através dessa história foi gerado uma segunda história de usuário, deixamos ela de lado, e continuamos a dar foco na nossa história2.

##  Mapeando História de Usuário 3: Publicando Anúncio Gratuito

Exemplo história3: Como um usuario autenticado eu quero criar um anuncio gratuito para vender o meu produto




5m
Reproduzir
10. Mapeando História de Usuário 4: Publicando Anúncio Pago
8m
Iniciar
11. Exercício para Fixação: Faça o Mapeamento de uma História de Usuário
1m
Iniciar
Teste 4: Fixação dos Conceitos
Reproduzir
12. Encerramento do Curso
1m
Reproduzir
13. Aulão - Respondendo Dúvidas e Resolvendo a Última Questão (parte 1)
44m
Reproduzir
14. Aulão - Respondendo Dúvidas e Resolvendo a Última Questão (parte 2)
39m
Reproduzir
15. Aulão - Respondendo Dúvidas e Resolvendo a Última Questão (parte 3)
49m


## Referencias

- https://insideproduct.co/example-mapping/
