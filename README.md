# Pesquisa sobre conceitos em Python

MVC
Model: Giovanni Gustavo
**O que é: ** **Como funciona: **

View: Anna
**O que é: ** **Como funciona: **

Controller:
O Controller (Controlador) é uma parte fundamental do padrão MVC (Model-View-Controller) em aplicações web e é responsável por gerenciar a lógica de interação entre o usuário,
a visão e o modelo. Aqui está uma explicação detalhada sobre o Controller em Python, com ênfase em frameworks populares como Flask e Django.

Funções do Controller

Receber Entradas do Usuário:
O controlador captura as ações do usuário, como cliques em botões ou envios de formulários. Em aplicações web, isso geralmente ocorre por meio de requisições HTTP.

Processar Lógica:
Após capturar a entrada, o controlador executa a lógica necessária. Isso pode incluir validação de dados, processamento de informações ou decisões sobre o fluxo da aplicação.

Interagir com o Modelo:
O controlador chama métodos do modelo para recuperar ou modificar dados. Isso pode envolver consultas a bancos de dados ou manipulações de dados existentes.

Selecionar a Visão:
Depois de processar a entrada e interagir com o modelo, o controlador determina qual visão deve ser renderizada e retorna essa visão ao usuário.

Exemplo em Flask:
Rota /:
O método index() é um controlador que renderiza a visão com a lista de tarefas. Ele utiliza a função render_template() para enviar os dados da lista de tarefas para o template HTML.

Rota /add:
O método add_task() é um controlador que processa o envio do formulário para adicionar uma nova tarefa, ele:
Captura o nome da tarefa do request.form.
Cria uma nova instância do modelo Task.
Adiciona a tarefa à lista de tarefas.
Redireciona o usuário de volta para a visão principal.

-   Recursos: Tudo o que pode ser manipulado pela API é um recurso. Por exemplo, em um e-commerce, os produtos são recursos.<br>
-   Verbos HTTP: A API usa verbos como GET (pegar), POST (criar), PUT (atualizar) e DELETE (deletar) para realizar ações nesses recursos.<br>
-   Endpoints: Cada recurso tem um endereço único (endpoint). Para buscar um produto específico, você faz uma requisição GET para o endpoint desse produto.<br>
-   Formato de dados: A informação é trocada em um formato padrão, como JSON ou XML.<br>
-   Stateless: Cada requisição é independente, a API não "lembra" o que aconteceu antes.<br>

# **REST:** (Gabriel)<br>
***O que é:***<br>
&nbsp;&nbsp;&nbsp;A API RESTful é uma interface que dois sistemas de computador usam para trocar<br>
&nbsp;&nbsp;&nbsp;informações de forma segura pela internet. A maioria das aplicações de negócios<br>
&nbsp;&nbsp;&nbsp;precisa se comunicar com outras aplicações internas e de terceiros para executar<br>
&nbsp;&nbsp;&nbsp;várias tarefas. Por exemplo, para gerar contracheques mensais, seu sistema interno<br>
&nbsp;&nbsp;&nbsp;de contas precisa compartilhar dados com o sistema bancário de seu cliente a fim de<br>
&nbsp;&nbsp;&nbsp;automatizar o faturamento e se comunicar com uma aplicação interna de planilha de horas.<br>
&nbsp;&nbsp;&nbsp;As APIs RESTful suportam essa troca de informações porque seguem padrões de comunicação<br>
&nbsp;&nbsp;&nbsp;de software seguros, confiáveis e eficientes.<br>
    <br>
<<<<<<< HEAD
***Como funciona:***<br>
&nbsp;&nbsp;&nbsp;A função básica de uma API RESTful é a mesma de navegar na internet. O cliente entra em<br>
&nbsp;&nbsp;&nbsp;contato com o servidor usando a API quando requer um recurso. Os desenvolvedores de API<br>
&nbsp;&nbsp;&nbsp;explicam como o cliente deve usar API REST na documentação da API da aplicação do servidor.<br>
&nbsp;&nbsp;&nbsp;Estas são as etapas gerais para qualquer chamada de API REST:<br>
    <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. O cliente envia uma solicitação ao servidor.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;O cliente segue a documentação da API para formatar<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a solicitação de modo que o servidor entenda.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. O servidor autentica o cliente e confirma que o cliente
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tem o direito de fazer essa solicitação.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. O servidor recebe a solicitação e a processa internamente.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4. O servidor retorna uma resposta ao cliente. A resposta contém<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;informações que indicam ao cliente se a solicitação foi bem-sucedida.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A resposta também inclui informações solicitadas pelo cliente.<br>
    <br>
&nbsp;&nbsp;&nbsp;Os detalhes de solicitação e resposta da API REST variam um pouco, dependendo de como os desenvolvedores da API projetam a API.
=======
**Como funciona:**<br>
    Uma API REST é como uma ponte que conecta diferentes sistemas, permitindo<br>
    que eles se comuniquem e troquem informações. Imagine como se fosse um menu<br>
    de um restaurante: você escolhe o que quer (um recurso), e o restaurante (a API)<br>
    prepara e entrega o pedido (a resposta).<br>
>>>>>>> 3ad589919b3c2332c7fba43da93c80a043128d15
    <br>
***APIs REST para Python:***<br>
&nbsp;&nbsp;&nbsp;1. Flask<br>
&nbsp;&nbsp;&nbsp;2. FastAPI<br>
&nbsp;&nbsp;&nbsp;3. Django Rest Framework<br>
&nbsp;&nbsp;&nbsp;4. Tornado<br>
&nbsp;&nbsp;&nbsp;5. Bottle<br>
&nbsp;&nbsp;&nbsp;6. Falcon<br>
&nbsp;&nbsp;&nbsp;7. Pyramid<br>
&nbsp;&nbsp;&nbsp;8. Sanic

CORS: Thiago
**O que é: ** **Como funciona: **
