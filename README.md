<h1 align="center">🎲 AluGames</h1>

<p align="center">
  Uma plataforma web para gerenciar o aluguel de boardgames, permitindo marcar jogos como
  alugados ou devolvidos de forma simples e visual.
</p>

<hr>

<h2>📌 Sobre o projeto</h2>

<p>
  Este projeto foi desenvolvido durante um curso da <strong>Alura</strong>. O HTML e o CSS foram fornecidos como base do curso,
  enquanto a lógica em <strong>JavaScript</strong> foi implementada por mim.
</p>

<h2>🖥️ Sobre a interface</h2>

<p>
  A aplicação exibe um catálogo de boardgames disponíveis para aluguel. Cada jogo possui:
</p>

<ul>
  <li>Uma imagem de capa;</li>
  <li>O nome do jogo;</li>
  <li>Um botão que alterna entre <strong>"Alugar"</strong> e <strong>"Devolver"</strong>;</li>
</ul>

<p>
  Ao clicar no botão, o status do jogo é alternado: quando alugado, a capa recebe um efeito visual
  de escurecimento (overlay) indicando indisponibilidade, e o botão muda de cor e texto para "Devolver".
</p>

<h2>⚙️ Funcionalidades</h2>

<ul>
  <li>✅ Alternância de status entre "Alugar" e "Devolver"</li>
  <li>✅ Feedback visual (overlay escurecido) para jogos alugados</li>
  <li>✅ Atualização dinâmica do texto e estilo do botão</li>
  <li>✅ Estrutura reutilizável para múltiplos jogos via <code>id</code></li>
</ul>

<h2>🧠 Como funciona o JavaScript</h2>

<h3>Função <code>alterarStatus(id)</code></h3>
<p>
  Recebe o <code>id</code> do jogo clicado e localiza o elemento correspondente na página
  (<code>#game-${id}</code>). A partir dele, seleciona a imagem e o botão internos usando <code>querySelector</code>.
</p>

<p>
  Em seguida, verifica se o jogo já está marcado como alugado através da classe
  <code>dashboard__item__img--rented</code>:
</p>

<ul>
  <li>
    <strong>Se estiver alugado</strong>: remove a classe de "alugado" da imagem e do botão,
    retornando o texto do botão para <code>"Alugar"</code>.
  </li>
  <li>
    <strong>Se não estiver alugado</strong>: adiciona a classe de "alugado" na imagem e no botão,
    alterando o texto para <code>"Devolver"</code>.
  </li>
</ul>

<p>
  Essa lógica é acionada pelo atributo <code>onclick</code> presente em cada botão do HTML,
  passando o número identificador do jogo correspondente.
</p>

<h2>🛠️ Tecnologias utilizadas</h2>

<table>
  <thead>
    <tr>
      <th>Tecnologia</th>
      <th>Uso</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>HTML5</td>
      <td>Estrutura da página</td>
    </tr>
    <tr>
      <td>CSS3</td>
      <td>Estilização, gradientes e responsividade</td>
    </tr>
    <tr>
      <td>JavaScript</td>
      <td>Lógica de aluguel/devolução (implementada por mim)</td>
    </tr>
    <tr>
      <td>Google Fonts</td>
      <td>Fontes Chakra Petch e Inter</td>
    </tr>
  </tbody>
</table>

<h2>📁 Estrutura do projeto</h2>

<pre>
📦 alugames
 ┣ 📂 css
 ┃ ┣ _reset.css
 ┃ ┗ main.css
 ┣ 📂 img
 ┃ ┣ logo.svg
 ┃ ┣ fade_bar.svg
 ┃ ┣ hachuras.svg
 ┃ ┣ monopoly.png
 ┃ ┣ ticket_to_ride.png
 ┃ ┗ takenoko.png
 ┣ 📂 js
 ┃ ┗ app.js
 ┣ 📜 index.html
 ┗ 📜 README.md
</pre>

<h2>🚀 Como executar</h2>

<ol>
  <li>Clone este repositório;</li>
  <li>Abra o arquivo <code>index.html</code> no navegador;</li>
  <li>Clique em "Alugar" ou "Devolver" para alternar o status de cada jogo!</li>
</ol>

<h2>🎓 Créditos</h2>

<p>
  Projeto base desenvolvido durante um curso da <a href="https://www.alura.com.br/" target="_blank">Alura</a>.
  A implementação da lógica em JavaScript foi feita por mim como parte do meu aprendizado.
</p>

<hr>

