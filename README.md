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

# **REST:** (Gabriel)<br>
***O que é:***<br>
&nbsp;&nbsp;&nbsp;Uma API REST (Representational State Transfer) é como uma interface<br>
&nbsp;&nbsp;&nbsp;que permite que diferentes sistemas se comuniquem entre si, trocando<br>
&nbsp;&nbsp;&nbsp;dados de forma organizada e eficiente. Imagine como se fosse um menu<br>
&nbsp;&nbsp;&nbsp;de um restaurante: você escolhe o que deseja (um recurso), e o restaurante<br>
&nbsp;&nbsp;&nbsp;(a API) prepara e entrega o pedido (a resposta).<br>
    <br>
**Como funciona:**<br>
    Uma API REST é como uma ponte que conecta diferentes sistemas, permitindo<br>
    que eles se comuniquem e troquem informações. Imagine como se fosse um menu<br>
    de um restaurante: você escolhe o que quer (um recurso), e o restaurante (a API)<br>
    prepara e entrega o pedido (a resposta).<br>
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
-   Recursos: Tudo o que pode ser manipulado pela API é um recurso. Por exemplo, em um e-commerce, os produtos são recursos.<br>
-   Verbos HTTP: A API usa verbos como GET (pegar), POST (criar), PUT (atualizar) e DELETE (deletar) para realizar ações nesses recursos.<br>
-   Endpoints: Cada recurso tem um endereço único (endpoint). Para buscar um produto específico, você faz uma requisição GET para o endpoint desse produto.<br>
-   Formato de dados: A informação é trocada em um formato padrão, como JSON ou XML.<br>
-   Stateless: Cada requisição é independente, a API não "lembra" o que aconteceu antes.<br>

CORS: Thiago
**O que é: ** **Como funciona: **
