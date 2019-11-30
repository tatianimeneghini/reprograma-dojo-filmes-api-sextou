# DOJO: API de catálogo filmes da Netflix   :movie_camera:

## Passo a passo pra criar a API:
- README.md
- npm init
- npm install express mongoose
- npm install -D nodemon
- .gitignore com node_modules
- criar server.js rodando o app.js com a porta escolhida
- criar o app.js com o express, exportando o app

## Missão do DOJO: API de Catálogo Filmes da Netflix
Criar uma API de catálogo de filmes com Banco de Dados com uma lista de sugestões de pontuação dos filmes.
Pra isso, criamos um mecanismo de pontuação para os filmes, de forma que os filmes que possuírem maior pontuação, vão aparecer antes dos outros. 
O Dojo foi criado coletivamente com a turma N3 de Back-end da {reprograma}.

## Requisitos
- Cada filme deve possuir os seguintes campos: nome, ano, avaliações, quantidade de exibições
- Não podemos ter filmes diferentes com o mesmo nome.
- Avaliações é uma lista de números, em que cada número representa a avaliação da pessoa de 1 a 5 (estrelas). Exemplo: { avaliacoes: [2,3,1,4,5,5,1,2] }.
- A pontuação do filme é calculada multiplicando a média de avaliações com a quantidade de exibições.
- A rota GET /filmes/catalogo deve trazer os filmes ordenados por pontuação, exibindo a pontuação de cada filme.
- A rota POST /filmes/criar deve receber no body um novo filme pra ser adicionado no banco de dados, somente com nome e ano.
- A rota PATCH /filmes/exibicao/:id deve salvar a lista completa de avaliações e a quantidade de exibições.
- A rota DELETE /filmes/remover/:id deve remover o filme do catálogo pelo ID.