# Pesquisa sobre conceitos em Python

<h1>MVC</h1>
Model: Giovanni Gustavo
**O que é: ** **Como funciona: **
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
 
<h2>como Funciona<h2>
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
   A API RESTful é uma interface que dois sistemas de computador usam para trocar<br>
   informações de forma segura pela internet. A maioria das aplicações de negócios<br>
   precisa se comunicar com outras aplicações internas e de terceiros para executar<br>
   várias tarefas. Por exemplo, para gerar contracheques mensais, seu sistema interno<br>
   de contas precisa compartilhar dados com o sistema bancário de seu cliente a fim de<br>
   automatizar o faturamento e se comunicar com uma aplicação interna de planilha de horas.<br>
   As APIs RESTful suportam essa troca de informações porque seguem padrões de comunicação<br>
   de software seguros, confiáveis e eficientes.<br>
    <br>
***APIs REST para Python:***<br>
   1. Flask<br>
   2. FastAPI<br>
   3. Django Rest Framework<br>
   4. Tornado<br>
   5. Bottle<br>
   6. Falcon<br>
   7. Pyramid<br>
   8. Sanic

CORS: Thiago
**O que é: ** **Como funciona: **
