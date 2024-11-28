# Pesquisa sobre conceitos em Python

<h1>MVC</h1>
<h1>View: Giovanni Gustavo</h1>

<h3>Definição:</h3> Um modelo de aprendizado de máquina é uma representação matemática 
que captura padrões em um conjunto de dados. 
Ele é treinado usando dados de entrada (features) e suas saídas correspondentes
(target) para fazer previsões ou classificações
em novos dados.<br>

Resumo
resumo
Em resumo, um "modelo" em Python pode significar um modelo de aprendizado de máquina, um modelo de dados em um framework web,
 ou um modelo de software, dependendo do contexto em que está sendo usado. 
 Se você tiver um contexto específico em mente, posso fornecer mais detalhes!
 
<h2>como Funciona</h2>
Resumo dos Modelos
Modelo em Aprendizado de Máquina:

- Coleta de Dados: Reúne dados relevantes.
- Pré-processamento: Limpa e prepara os dados (ex: remoção de valores ausentes).
- Divisão dos Dados: Separa em conjuntos de treinamento e teste.
- Escolha do Algoritmo: Seleciona o método apropriado para o problema.
- Treinamento: O modelo aprende padrões ajustando parâmetros com base nos dados de treinamento.
- Avaliação: Mede o desempenho usando métricas (ex: acurácia, MSE).
- Ajuste: Melhora o modelo através de ajustes e validação cruzada.
- Implantação: O modelo é colocado em produção para fazer previsões em novos dados.
- Modelo de Dados:

 Define a estrutura e a organização dos dados em um banco de dados.
Contém atributos que representam características dos dados e relacionamentos entre entidades.
Modelo em Engenharia de Software:

Representa a estrutura e interações de um sistema através de diagramas, como diagramas de classe e casos de uso.
<hr>
<h1>View: Anna</h1>

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

<h1> Controller : (Erica) </h1>
O Controller (Controlador) é uma parte fundamental do padrão MVC (Model-View-Controller) em aplicações web e é responsável por gerenciar a lógica de interação entre o usuário,
a visão e o modelo. Aqui está uma explicação detalhada sobre o Controller em Python, com ênfase em frameworks populares como Flask e Django.

<h2> Funções do Controller </h2>

Receber Entradas do Usuário:
O controlador captura as ações do usuário, como cliques em botões ou envios de formulários. Em aplicações web, isso geralmente ocorre por meio de requisições HTTP.

Processar Lógica:
Após capturar a entrada, o controlador executa a lógica necessária. Isso pode incluir validação de dados, processamento de informações ou decisões sobre o fluxo da aplicação.

Interagir com o Modelo:
O controlador chama métodos do modelo para recuperar ou modificar dados. Isso pode envolver consultas a bancos de dados ou manipulações de dados existentes.

Selecionar a Visão:
Depois de processar a entrada e interagir com o modelo, o controlador determina qual visão deve ser renderizada e retorna essa visão ao usuário.

<h2> Exemplo em Flask </h2>
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
   A API REST é uma interface que dois sistemas de computador usam para trocar<br>
   informações de forma segura pela internet. A maioria das aplicações de negócios<br>
   precisa se comunicar com outras aplicações internas e de terceiros para executar<br>
   várias tarefas. Por exemplo, para gerar contracheques mensais, seu sistema interno<br>
   de contas precisa compartilhar dados com o sistema bancário de seu cliente a fim de<br>
   automatizar o faturamento e se comunicar com uma aplicação interna de planilha de horas.<br>
   As APIs REST suportam essa troca de informações porque seguem padrões de comunicação<br>
   de software seguros, confiáveis e eficientes.<br>
    <br>
    ***Como funciona:***<br>
   A função básica de uma API REST é a mesma de navegar na internet. O cliente entra em<br>
   contato com o servidor usando a API quando requer um recurso. Os desenvolvedores de API<br>
   explicam como o cliente deve usar API REST na documentação da API da aplicação do servidor.<br>
   Estas são as etapas gerais para qualquer chamada de API REST:<br>
    <br>
      1. O cliente envia uma solicitação ao servidor. O cliente segue a documentação da API para formatar a solicitação de modo que o servidor entenda.<br>
      2. O servidor autentica o cliente e confirma que o cliente tem o direito de fazer essa solicitação.<br>
      3. O servidor recebe a solicitação e a processa internamente.<br>
      4. O servidor retorna uma resposta ao cliente. A resposta contém informações que indicam ao cliente se a solicitação foi bem-sucedida. A resposta também inclui informações solicitadas pelo cliente.<br>
    <br>
   Os detalhes de solicitação e resposta da API REST variam um pouco, dependendo de como os desenvolvedores da API projetam a API.<br>
   <br>
***APIs REST para Python:***
   1. Flask<br>
   2. FastAPI<br>
   3. Django Rest Framework<br>
   4. Tornado<br>
   5. Bottle<br>
   6. Falcon<br>
   7. Pyramid<br>
   8. Sanic

<h1>CORS: Thiago </h1><p>

<h2>Oque é o Cors:</h2> <p> CORS (Cross-Origin Resource Sharing) é um mecanismo que permite que recursos de uma origem (domínio) sejam acessados por outra origem. Por padrão, navegadores bloqueiam essas requisições por motivos de segurança.  <br>

<h2>Com funciona o CORS:</h2> Quando uma página tenta acessar um recurso em outra origem, o navegador pode enviar uma requisição "preflight" usando o método OPTIONS. Essa requisição verifica se a origem é permitida pelo servidor. O servidor, então, responde com cabeçalhos CORS, como Access-Control-Allow-Origin, que especificam quais origens podem acessar os recursos.

Se a origem for permitida, o navegador prossegue com a requisição real. Se não, a requisição é bloqueada. Em resumo, o CORS controla o acesso a recursos entre diferentes origens, git equilibrando segurança e funcionalidade.</p>

