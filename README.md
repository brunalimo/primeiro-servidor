# primeiro-servidor
Primeiro servidor npm - teste para as aulas da Cubos academy.

Passo 1 - Configuração inicial 
- Iniciei o projeto com a instalação do NPM (Node Package Manager) com o comando:
-- npm init y //para criar o pacote com o package.json;
-- npm install express //instalar um pacote localmente;
-- npm intall -D nodemon // para restartar o servidor automaticamente;
- Criei a "const express = require('express'); e a const app = express(); para importar o express no código.

Passo 2 - Lista de jogadores
- Defini a lista de jogadores criando um array "const jogadores";
- Com a variável "let jogadorDaVez" estabeleci como valor de 0 para controlar qual jogador estará jogando.

  Passo 3 - Rota
  - Configurei a rota usando app.get e uma função callback de requisição (req) e resposta (res);

  Passo 4 - Lógica
  - Adicionei a lógica dentro da rota/função callback.
  - Criei uma constante que terá o papel de armazenar o nome do jogador da vez: "const nomeJogador = jogadores[jogadorDaVez];"
  - Com o incremento ++, a lista deve rodar, passando a vez para um próximo jogador; "jogadorDaVez++;"
  - Adicionei condicional if ("se o jogador da vez for menor ou igual ao array (jogadores).length") para garantir que o
    índice do jogador da vez não ultrapasse o tamanho da lista de jogadores.
  - Por fim, com o "return res.send" espera-se retornar o nome do jogador que deve jogar no momento.
