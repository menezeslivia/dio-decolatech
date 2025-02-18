# dio-decolatech
Repositório de projetos do bootcamp Decola Tech da Avanade

VISÃO GERAL 
Spring Framewok

AULA 1: Fundamentos

- Oque é spring framework

* Framework open source (codigo aberto) desenvolvido pera plataforma java baseado nos padrões de projetos inversão de controle (atribuir responsabilide a um container) e injeção de dependencia. 

Composta por modulos, para simplificar o desenvolvimento.


-Spring Versus JAVA EE

* java ee era muito complicado, usar o sping era um caminho mais simples  facil d evoluir, mas chegou a versão  5 do java ee e a discussão voltou a ficar mais quente. 

- Conceito de inversão de controle

Trata-se do redirecionamento do fluxo de execução de um código retirando parcialmente o controle sobre ele e delegando-o para um container. O principal proposito é minimizar o acoplamento do código.

sem IoC: Antes era necessário criar o objeto para depois utilizar

Com Ioc 

Aplicação inciializada, container configurado, os objetos que precisam existir ja estarão previamete no container, quando precisar usar o objeto pede ao container

- Injeção de dependencias

Parão de desenvolvimento com a finalizade de manter o baixo nivel de acoplamento entre modulos de um sistema 


- Beans / autowired / scopes

BEANS: Objeto que é criado (instanciado), montado e gerenciado pelo container

SCOPES: 

Singleton: um unico objeto sendo compartilhado por toda a aplicação quando for solicitado

Prototype: criado uma nova instancia a cada requisição de um objeto ao container.

HTTP 
Um bean será criado para cada requisição http.

Requisições, sessões e global

Request

Um bean será criado para cada requisição http (os objetos existirão enquanto a requisição estiver em execução)

Session

Um ben será criado para cada sessão e usuário (precisamos acessar a mesma solicitação duas vezes para testar os escopos específicos da web)

Global

Cria um bean para o ciclo de vida do contexto da aplicação (Objetos compartilhados por toda a aplicação)

AUTOWIRED

Anotação onde deverá ocorrer uma injeção automatica de dependencia.

* byName: É buscado um método set que corresponde ao nome do Bean

* byType: É considerado o tipo da classe para inclusão do Bean.

* byCOnstrutor: Usamos o construtor para incluir a dependência.

--------------------------
Spring (boot) Framework

- Oque é springboot?

Foca na consfiguração automatica
padrões de estruturação de projeto
