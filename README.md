## Projeto de Certificação 1 - Trilha 1 - Lógica de Programação - DEVstart

Neste projeto avaliaremos as <b> notas dos atletas de uma competição escolar de Ginástica Artística.</b>

5 jurados avaliam os seguintes quesitos: 
<ol><li>Tempo de duração da apresentação.</li> <li> Originalidade da coreografia.</li> <li> Postura do atleta. </li> <li> Dificuldade das acrobacias. </li> <li> Sincronismo. </li> </ol>

Critérios de avaliação das notas:
1. Cada jurado pode fornecer uma nota entre 1 e 10
2. A média é calculada com base nas três notas do meio, desconsiderando a maior e menor nota.

------------
### Metodologia

Recebemos os dados da competição numa matriz de objetos contendo: nome do atleta e notas dos jurados.

Os resultados finais serão entregues neste formato:

Atleta:
<br>
Notas Obtidas:
<br>
Notas Válidas:
<br>
Média Notas:
<br></br>
Declaramos as seguintes variáveis: <b>nomesAtletas, notasObtidas, notasValidas</b>
<br>
Para acessar cada objeto da matriz, usaremos o laço for a seguir: <b> for (let i = 0; i < atletas.length; i++){ </b>
<br>
Pelo metodo <b>map</b> buscamos um novo resultado para cada elemento da matriz inicial dentro das variáveis declaradas.
<br>
Com o uso do <b>sort.()</b> ordenamos as notas dos jurados em ordem crescente, e pelo <b>slice.(1,4)</b> excluímos a maior e menor nota do atleta.
</br>

Na segunda etapa, para descobrirmos a <b>média das notas válidas</b>, novamente usaremos o mesmo laço for,
agora com a estrutura <b>condicional switch atrelando o contador [i] na cláusula case</b>.
Com o console.log printamos o resultado do nome Atleta e Notas Obtidas em conjunto com o contador [i].
Ao declarar a variável notasAtletas com o método slice() nas notasObtidas, obtemos apenas as 3 notas válidas, sem a maior e menor nota do atleta.
Para somar estas 3 notas, usamos o <b>reduce()</b>, e para encontrar a média dividimos a soma pelo número 3, e no resultado da média utilizamos o toFixed(2),
assim nosso resultado fica apenas com duas casas decimais depois da vírgula.

------------
### Resultado

Atleta: Cesar Abascal <br>
Notas Obtidas: 7.88,8.42,9.34,10,10 <br>
Notas Válidas: 8.42,9.34,10 <br>
Media Notas: 9.25 <br>

Atleta: Fernando Puntel <br>
Notas Obtidas: 7,8,9.33,10,10 <br>
Notas Válidas: 8,9.33,10 <br>
Media Notas: 9.11 <br>

Atleta: Daiane Jelinsky <br>
Notas Obtidas: 7,8,9.5,9.5,10 <br>
Notas Válidas: 8,9.5,9.5 <br>
Media Notas: 9.00 <br>

Atleta: Bruno Castro <br>
Notas Obtidas: 9,9.5,10,10,10 <br>
Notas Válidas: 9.5,10,10 <br>
Media Notas: 9.83 <br>

------------
### Classificação da Competição de Ginástica Olímpica:
🏆 [1] BRUNO CASTRO <br>
🥈 [2] CESAR ABASCAL <br>
🥉 [3] FERNANDO PUNTEL <br>
🏅 [4] DAIANE JELINSKY
