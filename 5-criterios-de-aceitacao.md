# Criterios de aceitação

Critério de aceitação ou critério de aceite, é um grupo de condições ou regras de negócio que têm que ser atendidas para que a história do usuário possa ser aceita pelo dono do produto. Elas devem ser passíveis de serem testadas ou seja elas devem possuir instruções claras e objetivas para evitar qualquer ambiguidade. 

Elas também agregam mais informações às Histórias de usuário e definem como uma determinada funcionalidade será utilizada sob o ponto de vista do usuário final.
Um fato interessante é que essa regra, ou o conjunto de regras que elas ajudam o time a entender o que de fato será feito, para que aquela história do usuário seja considerada completa, que seria a definição de pronto (DEFINITION OF DONE DOD).
Como elas adicionam mais informações às Histórias, elas acabam melhorando a estimativa de esforço feita pelo time e também ajudam na hora de quebrar as histórias em partes menores quebrar em tarefas.

Obviamente, nos times que possuem essa prática de quebrar histórias em tarefas, e por fim elas ajudam também a alinhar as expectativas do PO sobre o que será entregue, bem como o que está incluído e excluído no escopo de uma determinada história, e há diversas maneiras de se definir um critério de aceitação.

![image](https://user-images.githubusercontent.com/52088444/233513006-fd801903-6a4c-47b2-bb78-152790c1942d.png)

**3 Modelos/formatos de se criar critéios de aceitação

![image](https://user-images.githubusercontent.com/52088444/233513155-24fc5c39-7457-41f0-8f70-31d4d8ebac56.png)


![image](https://user-images.githubusercontent.com/52088444/233513170-2bf3c67b-2c75-46ef-8d04-6786d8eb6987.png)

Nesse exemplo nós conseguimos identificar um título que seria o seguinte: Sign in startr your session,dois campos, que seriam um campo para e-mail e o campo de senha, e um botão de Logar.

Nesse exemplo vamos ignorar os dois ícones que a gente consegue ver aqui na tela, que seria o ícone de carta e o ícone de cadeado como se eles não fizessem parte do escopo dessa história.

Como escreveria essa funcionalidade de login  ou esse componente em forma de História de usuário?

como o titular da conta.
Eu quero poder acessar o portal de maneira segura 
para que eu possa consultar minha conta e verificar meu fundo de investimento

![image](https://user-images.githubusercontent.com/52088444/233513551-d0fb91da-aed4-4f62-a4b5-5ff1072a96e6.png)

## Checklist

Checklist como o nome diz, identifica os critérios de aceitação como se fossem parte de uma lista, passível de alguém olhar o item por item, linha por linha e conferir se aquilo foi atendido ou não.

como seria o critério de aceitação para a história do usuário acessar o sistema na parte de login?

![image](https://user-images.githubusercontent.com/52088444/233513851-21913af0-b07e-457b-8488-a9f4b9351bfd.png)

Perceba que em critérios de aceitação nós podemos utilizar os operadores lógicos "E" e o "OU"  para basicamente facilitar o entendimento de uma ação.

Nesse caso o segundo item do checklist só vai ser verdade e só vai passar no Teste se ambas condições forem corretas.

Por exemplo se o usuário inserir somente o usuário correto e conseguir acessar o sistema. Esse item está falho, ou se o usuário inserir somente a senha correta e também conseguir acessar o sistema, esse item também está falho, só vai passar se o usuário inserir o nome de usuário e a senha correta.

Outro ponto que é interessante notar é que cada item é bastante claro e objetivo o que facilita o entendimento do time do time e obviamente do PO.
E eles são similares a uma lista de compras.

## Modelo de  Perguntas fechadas (Closed-questions)

Esse modelo de perguntas fechadas ao invés de uma simples lista de itens, você terá uma lista de perguntas bem claras e objetivas, para evitar qualquer ambiguidade que funcionam como uma forma de teste, possuindo instruções que serão facilmente verificadas pelo time.

poderia ser algo como:

![image](https://user-images.githubusercontent.com/52088444/233514408-21793431-5f6c-4457-9019-eeb534fb55b9.png)

Se por algum motivo a resposta para qualquer um dos itens acima for não, isso significa que o que foi acordado entre o time e o PO não foi atendido. Logo essa história teria que voltar para o time para que ela seja finalizada.

## Desenvolvimento Orientado a Comportamento (BDD - Behaviour Driven Development)

O BDD é o modelo mais indicado , porque ela encoraja os donos do produto a pensarem nos diferentes possíveis cenários utilizando as palavras em inglês:

![image](https://user-images.githubusercontent.com/52088444/233514718-b40b1238-fe9c-4a80-9888-5d750f8e5b7c.png)

- O given/dado : foca no cenário que será descrito no estado antes do usuário executar uma determinada ação;
- when/quando: que seriam quando descreve a ação que aquele tipo de usuário fará.
- then/então:  descreve o resultado que o usuário terá após ele executar uma determinada ação e executar aquela ação.


Eu gostaria de salientar de ressaltar alguns pontos que são bastante importantes sobre usar BDD para identificar critérios de aceitação. O primeiro deles é que todo o cenário deve ser descrito usando a linguagem de negócio, nunca use linguagem técnica. Todo o cenário deve ser descrito sob o ponto de vista do usuário final ou seja todos eles devem respeitar o tipo de usuário que foi definido na história do usuário.

Os engenheiros podem teoricamente copiar os cenários identificados em uma história de usuário e colar dentro dos casos de teste.

![image](https://user-images.githubusercontent.com/52088444/233515262-8cb4bdb3-5b38-49f1-a263-90dad35f8761.png)

![image](https://user-images.githubusercontent.com/52088444/233515294-d3362117-d11a-4447-a886-0d141314c77b.png)

## O que considerar para definir bons critérios de aceitação

Primeiramente toda e qualquer interação do sistema com o usuário como um mouse, ou clique no botão descobrir, também a jornada do usuário, Considerando todos os cenários do início ao fim de um determinado usuário precisa seguir para poder completar uma determinada jornada e uma jornada específica no sistema rápido .
![image](https://user-images.githubusercontent.com/52088444/233515534-0f37e60b-9323-489e-84c8-c3c4077d66ba.png)

## Aula Prática: Definindo critérios de aceitação (Exemplo#1)

Wireframe de uma tela de news
![image](https://user-images.githubusercontent.com/52088444/233696298-02a2a66e-d9b3-47bd-a5ba-9cf91c8e359d.png)

Os 4 blocos representando os posts de noticias com imagem e descrição, os 3 pontinhos representam o carrosel. Temos um filtro. Abaixo as notícias mais antigas , e a paginação se as listas forem maiores.

![image](https://user-images.githubusercontent.com/52088444/233696794-e72ee27f-61e1-4ca5-b26d-842a9008436b.png)
Essa história de usuário está cobrindo essa parte.

![image](https://user-images.githubusercontent.com/52088444/233696869-61c42326-ed9c-41cf-bad5-e4775ba08450.png)


**Criar critérios de aCeitação usando BDD:

nós temos uma história de usuário e através dela criamsos os critérios de aceitação com todos os cenários que quisermos. Ou seja criamos uma jornada pois a experiência de usuário é diferente em cada dispositivo
![image](https://user-images.githubusercontent.com/52088444/233698099-464fbcc7-99d2-4758-b76a-7c5c30b74470.png)
![image](https://user-images.githubusercontent.com/52088444/233698485-37a6fc97-af5b-4ad7-a81f-bb046a365669.png)

**VERIFICAR SE EXISTE DIFERENÇA ENTRE OS COMPORTAMENTOS ENTRE MOBILLE E DESSKTOP, 


## Aula Prática: Definindo critérios de aceitação (Exemplo#2)
![image](https://user-images.githubusercontent.com/52088444/233698756-5c7e9bd5-d642-469a-bf94-ba74cce545cb.png)

Ficaram separadas por que senão a User Storie fica muito grande.Eu estou repetindo as frases por que as histórias precisam ser independentes, mesmo sendo a mesma página, só que seções diferentes.

![image](https://user-images.githubusercontent.com/52088444/233699362-41cdc514-a492-4826-b5f8-cc02bf8f164f.png)
![image](https://user-images.githubusercontent.com/52088444/233699604-bfac3e6f-f132-4bee-a471-029d3514a1e4.png)

## Aula Prática: Definindo critérios de aceitação (Exemplo#3)

![image](https://user-images.githubusercontent.com/52088444/233699686-d14c9295-b27f-43d8-834a-8d841fc205df.png)
![image](https://user-images.githubusercontent.com/52088444/233699942-e65bcf93-8ad9-4faf-98d5-8e2ee13f25f9.png)

só estamos cobrindo a parte das estrelas/pontuaçãoes

## Aula Prática: Definindo critérios de aceitação (Exemplo#4)

![image](https://user-images.githubusercontent.com/52088444/233700104-394b3ce0-8a7f-456b-9cbd-2f69f0c598c5.png)
Um banner e um botão, como é um wireframe vamos escrever no BDD

![image](https://user-images.githubusercontent.com/52088444/233700421-a6adf729-25d9-4d58-ba5b-311b9f23621d.png)

## Aula Prática: Definindo critérios de aceitação (Exemplo#5)

![image](https://user-images.githubusercontent.com/52088444/233700487-2372fa45-cd83-4e65-beee-d99388136b5c.png)

![image](https://user-images.githubusercontent.com/52088444/233700946-d8d3a3e0-90b7-46cb-902f-1646c172c8e5.png)

Ele só está analisando o review

## Dicas para definição de critérios de aceitação

![image](https://user-images.githubusercontent.com/52088444/233701268-b9c5fceb-0d89-4603-ba8c-7677ed61ca20.png)

No BDD (Behaviour Driven Development ou Desenvolvimento Orientado a Comportamento), o que “Dado/Quando/Então” quer dizer respectivamente?
![image](https://user-images.githubusercontent.com/52088444/233701501-58cd4944-7929-4cd2-9dc4-4e3a5671a560.png)

