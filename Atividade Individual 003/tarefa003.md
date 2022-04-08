
## Tarefa 003 - 21/12/2021 - Definição de Classes de Equivalência.

**DEFINIÇÃO**:
1. Definir um conjunto de classes de Equivalência e um conjunto de casos de testes derivados, para testar a seguinte função de avaliação universitária.
2. A função avalicao, recebe como parâmtros os seguintes dados:
   2.1. **nota1** (numérico de ponto flutuante com duas casas decimais);
   2.2. **nota2**  (numérico de ponto flutuante com duas casas decimais);
   2.3. **cargaHoraria** (numérico inteiro, positivo);
   2.4. **faltas** (numérico inteiro, positivo).
3. A forma de calcular a avaliação é a seguinte:
  3.1. Se a quantidade de faltas for superior a 25% da carga horária, o aluno estará reprovado por falta. Neste caso a função retorna a seguinte mensagem **Reprovado por Falta**;
  3.2. Estando o aluno reprovado por falta, não haverá a necessidade de se avaliar as notas;
  3.2. Se a média entre nota1 e nota2 for menor que 3.0, o aluno estará reprovado por média.  Neste caso a função retorna a seguinte mensagem **Reprovado por Média**;
  3.3. Se a média entre nota1 e nota2 for >= 3.0 e < 6.0, o aluno estará em recuperação.  Neste caso a função retorna a seguinte mensagem **Recuperação**;
  3.4 Em qualquer outra situação o aluno estará  aprovado. Então a função retornará a mensagem: **Aprovado**.
4. O Conjunto de classes de Equivalência deverá ser definido seguindo o seguinte padrão:

**Classes de Equivalência**

|id|descrição|V/I|E/S|

|CE01|informar menos que 4 parâmetros |I|E|
|CE02|informar 4 parâmetros |V|E|
|CE03|informar mais que 4 parâmetros |I|E|
|CE04|nota1 inserida|V|E|
|CE05|nota1 não inserida|I|E|
|CE06|nota1 < 0.00|I|E|
|CE07|0.00 <= nota1 <= 10.00|V|E|
|CE08|nota1 > 10.00|I|E|

**cdm** - casas decimais
|CE09|cdm < 2|I|E|
|CE10|cdm = 2|V|E|
|CE11|cdm > 2|I|E|

**tvn1** - tipo da variavel nota 1 
|CE12|tvn1 <> double|I|E|
|CE13|tvn1 = double|V|E|
|CE14|nota2 inserida|V|E|
|CE15|nota2 não inserida|I|E|
|CE16|nota2 < 0.00|I|E|
|CE17|0.00 <= nota2 <= 10.00|V|E|
|CE18|nota2 > 10.00|I|E|

**cdm** - casas decimais
|CE19|cdm < 2|I|E|
|CE20|cdm = 2|V|E|
|CE21|cdm > 2|I|E|

**tvn2** - tipo da variavel nota 2
|CE22|tvn2 <> double|I|E|
|CE23|tvn2 = double|V|E|
|CE24|cargaHoraria inserida|V|E|
|CE25|cargaHoraria não inserida|I|E|
|CE26|cargaHoraria = {32, 64, 96 e 128} |V|E|
|CE27|cargaHoraria <> {32, 64, 96 e 128}|I|E|

**tvch** - tipo da variavel CargaHoraria
|CE28|tvch <> int|I|E|
|CE29|tvch = int|V|E|
|CE30|faltas inseridas|V|E|
|CE31|faltas não inseridas|I|E|
|CE32|faltas < 0|I|E|
|CE33|faltas <= 25% de cargaHoraria|V|E|
|CE34|faltas > 25% de cargaHoraria|V|E|
|CE35|faltas > cargaHoraria|I|E|
|CE36|faltas <> int|I|E|
|CE37|faltas = int|V|E|
|CE38|"Entrada Inválida"|V|S|
|CE39|"Reprovado por Falta"|V|S|
|CE40|"Reprovado por Média"|V|S|
|CE41|"Recuperação"|V|S|
|CE42|"Aprovado"|V|S|




**Casos de Teste**

|CT|Valor de Entrada|Resultado Esperado|Classe Equivalência|

|CT01|,7.00,32,8|"Inválido"|CE01,CE05,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT02|7.00,,32,8|"Inválido"|CE01,CE04,CE07,CE10,CE13,CE15,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT03|7.00,4.00,,8|"Inválido"|CE01,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE25,CE30,CE34,CE37,CE38|
|CT04|7.00,4.00,32,|"Inválido"|CE01,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE31,CE38|
|CT05|4.00,7.00,32,8,15|"Inválido"|CE03,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT06|-4.00,7.00,32,8|"Inválido"|CE02,CE04,CE06,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT07|4.00,-7.00,32,8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE16,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT08|4.00,7.00,-32,8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE26,CE29,CE30,CE33,CE37,CE38|
|CT09|4.00,7.00,32,-8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE32,CE37,CE38|
|CT10|4,7.00,32,8|"Inválido"|CE02,CE04,CE07,CE09,CE12,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT11|4.00,7,32,8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE19,CE22,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT12|4.00,7.00,32.00,8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE26,CE28,CE30,CE33,CE37,CE38|
|CT13|4.00,7.00,32,8.00|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE36,CE38|
|CT14|11.00,7.00,32,8|"Inválido"|CE02,CE04,CE08,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT15|4.00,15.00,32,8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE18,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT16|4.00,7.00,250,8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE26,CE28,CE30,CE33,CE37,CE38|
|CT17|4.00,7.00,32,35|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE34,CE35,CE36,CE38|
|CT18|4.0,7.00,32,8|"Inválido"|CE02,CE04,CE07,CE09,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT19|4.00,7.0,32,8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE19,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT20|4.000,7.00,32,8|"Inválido"|CE02,CE04,CE07,CE11,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT21|4.00,7.000,32,8|"Inválido"|CE02,CE04,CE07,CE10,CE13,CE14,CE17,CE21,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE38|
|CT22|4.00,7.00,32,10|"Reprovado por Faltas"|CE02,CE04,CE07,CE11,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE34,CE37,CE39|
|CT23|2.00,1.00,32,8|"Reprovado por Media"|CE02,CE04,CE07,CE11,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE40|
|CT24|4.00,5.00,32,8|"Recuperação"|CE02,CE04,CE07,CE11,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE41|
|CT24|6.00,8.00,32,8|"Aprovado"|CE02,CE04,CE07,CE11,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE42|

