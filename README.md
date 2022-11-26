
<h1>&#9917;&#127758;FLAI_Data-Science_COPA_DO_MUNDO_2022 &#127758;&#9917;</h1>
 
<h2>&#9917;Previsão de Partidas</h2>
<hr>
<div style='text-align:justify'>
<p>Modelar não é representar a realidade, mas transmitir uma equação útil, então tentamos quantificar as frações possíveis.
<p>É interessante quanta variação existe no futebol, e essa variação coloca os problemas do jogo nas minúcias. Se pudéssemos repetir o jogo algumas vezes, poderíamos ter vários jogos de diferentes valores.</p>
<p>Quando se trata de futebol, estamos quantificando todas as incertezas possíveis.</p>

<h2>&#9917;FLAI – Inteligência Artificial e Data Science</h2>
<hr>
<p>Sim, este mini curso foi disponibilizado pela FLAI, abaixo o link para as videos aulas:</p>
<a href="url">AULA 1 YOUTUBE</a><br>
<a href="url">AULA 2 YOUTUBE</a><br>
<a href="url">AULA 3 YOUTUBE</a><br><br>

<h2><i>&#9917;Questão 1: Como modelar a distribuição de gols das equipes em um jogo</i></h2> 
<hr>
<h3>Distribuição Poisson:</h3>

<p>Ajuda quando tentamos quantificar a probabilidade de marcar. É uma boa escolha para dados de futebol para contagem de gols em partidas, o que foi verificado por alguns pesquisadores.</p>

<img src="image\equacao.png" width="400px;">

Onde:<br>
k - número de ocorrências;<br>
e - número de Euler.<br>

<p>Com isso, podemos calcular a probabilidade de cada gol multiplicando a probabilidade de um determinado time marcar tantos gols pela probabilidade de outro time marcar tantos gols.</p>

<p>&#9917;A probabilidade de empate em uma partida é a soma das probabilidades de empate em cada resultado.</p>
<p>&#9917;A probabilidade de vitória da Argentina é a soma das probabilidades de suas combinações de pontos vencedores.</p>
<p>&#9917;A probabilidade do Vitória do Brasil é a soma das probabilidades de todas as combinações em que ele ganha.</p>
<p>Portanto, em um jogo, a distribuição de gols para o time 1 e time 2 é S¹ ~ Poisson(m1) s² ~ Poisson(m2) respectivamente onde:</p>
m - Alvo médio.<br>
Em que S¹ e S² são independentes.<br><br>

<h2><i>&#9917;Questão 2: Como calculo o número médio de golos por equipa por jogo</i></h2>
<hr>
<p>Partindo da média histórica de gols marcados na Copa do Mundo e considerando alguns fatores, podemos pensar que a média de gols esperados nesta Copa é de 2,75.</p>
m = m¹ + m²<br>
m = 2,75<br>

<p>Agora é só descobrir para cada equipe, quanto resta de cada equipe.</p>
<p>Para isso usaremos o fator de força de cada equipe</p>


m¹ = m . f¹ / (f¹ + f²) <br>
m² = m - m² <br>

<p>Onde:</p>
f¹ - força da Seleção 1 <br>
f² - força da Seleção 2 <br>


<p>O método de cálculo da força de cada seleção utilizará o ranking da FIFA. Convertemos os valores do ranking para um intervalo (a, 1), onde 1 é a escolha mais forte.</p>







