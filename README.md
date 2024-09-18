# Pesquisa sobre conceitos em Python

MVC
Model: Giovanni Gustavo
**O que é: ** **Como funciona: **

View: Anna
**O que é: ** **Como funciona: **
Em Python, o termo "view" pode se referir a várias coisas, dependendo do contexto em que é usado.

1. **Views em Frameworks Web**: Em frameworks como Django ou Flask, uma "view" é uma função ou classe que processa uma requisição HTTP e retorna uma resposta. Ela define a lógica de apresentação e manipulação de dados para uma determinada rota.
2. **View em Bases de Dados**: Em bancos de dados SQL, uma "view" é uma tabela virtual que resulta de uma consulta. Você pode usá-la para simplificar consultas complexas, encapsular lógica e melhorar a segurança.
3. **View em Estruturas de Dados**: Em bibliotecas como NumPy, uma "view" é uma forma de acessar os dados de um array sem criar uma cópia. Isso permite manipulações eficientes da memória.

### Views em Python

1. **Views em Frameworks Web (Django e Flask)**:
   - **Django**:
     - As views são definidas em um arquivo `views.py`.
     - Elas processam requisições HTTP e retornam respostas.
     - Exemplo básico:

       ```python
       from django.http import HttpResponse

       def minha_view(request):
           return HttpResponse("Olá, mundo!")
       ```

     - As views podem acessar modelos (models) para manipular dados do banco de dados e renderizar templates.

   - **Flask**:
     - As views são funções decoradas com `@app.route()`.
     - Exemplo:

       ```python
       from flask import Flask

       app = Flask(__name__)

       @app.route('/')
       def minha_view():
           return "Olá, mundo!"
       ```

2. **Views em Estruturas de Dados (NumPy)**:
   - Em NumPy, uma "view" é uma maneira de acessar e modificar dados de um array sem criar uma cópia.
   - Exemplo:

     ```python
     import numpy as np

     array_original = np.array([1, 2, 3, 4])
     view_array = array_original[1:3]  # Cria uma view

     view_array[0] = 99  # Modifica o valor na view
     print(array_original)  # Saída: [ 1 99 3 4]
     ```
	 
### Resumo
- **Views em Web**: Funções que lidam com requisições e respostas.
- **Views em NumPy**: Referências a arrays que permitem manipulação eficiente de dados.

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
