<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P2 - 12/04/2022</p>

Matrícula: 201808796

Nome: Gabriel Cândido Gomes Mendonça

<font color="green">Nota 6,58</font>

1. Quanto ao Processo de Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Defina os seguintes conceitos Processo de Teste de Software, Projeto de Teste de Software e Plano de Teste de Sofware.

   Plano de Teste de Software: Descrição detalhada dos objetivos do teste de software a serem alcançados e os meios e o  cronograma para alcança-los, organizando e coordenando atividades de teste para algum item de teste ou conjunto de itens de teste de software.

   Processo: Um processo é uma ação continua, continuada e prolongada de uma atividade, seguimento,curso ou decurso, possui uma sequencia contínua de fatos ou operações, reproduzindo com certa regularidade.

   Processo de Teste de Software: Já o processo de teste de software, compõem por uma série de atividades agrupadas em um ou mais subprocesssos de teste de software. Além de fornecer informações sobre a qualidade de um produto de software.

   Projeto de Teste de Software: É um documento que especifica os detalhes da abordagem de teste para um requisito de software ou combinação deles, além de identificar os casos de teste associados, descrevendo a estrutura dos elementos de testes e a realização dos casos de teste. Sendo também um esforço temporário que possui tempo de inicio e fim para essa abordagem de teste para os requisitos associados e os elementos. <font color="red">Nota 0,5</font>

   2. (**0,5 ponto**) Descreva o relacionamento existente entre estes conceitos.

   Inicialmente sendo um projeto de teste de software um esforço temporário, que possui inicio e fim, empreendido no intuito de detalhar e uma abordagem de teste para um requisito de software ou combinação deles, podemos dizer que para alcançar os objetivos definidos em questão , é necessário um processo de teste de software que compreende uma série de atividades agrupada e um ou mais subprocesso de teste, e dentro de um subprocesso(ou etapa), temos as fases mais comuns de um processo de teste e software, e dentro da fase de iniciação, temos como artefato de saída  o Plano de Teste que será usado como artefato de entrada na fase de planejamento. <font color="red">Nota 0,4</font>

2. (**1,0 pontos**) Descreva as vantagens para a equipe de desenvolvimento ao se adotar um processo de teste ágil.

Foco em várias tarefas simultaneamente , planejamento iterativo e incremental, alterações são sempre bem vindas.

Os testes são usados como complementos dos requisitos e da documentação, foco maior em testes exploratórios.

É realizado por meios de teste automatizados com mais frequência, é realizado por todos da equipe.

Ocorre durante todo o desenvolvimento em ciclos contínuos e frequentes. <font color="red">Nota 1,0</font>

3. (**1,0 ponto**) Cite pelo menos três características do Teste Exploratório.

Quando scripts são removidos e são menos rígidos ,permite aos testadores interagirem com a aplicação como desejarem e utilizar as informações obtidas para depois reagirem, alterar o curso , explorar as funcionalidades da aplicação sem repressão.

É muito poderosa para detectar defeitos quando dominada,além disso os resultados de teste, casos de teste e documentação de teste são gerados a medida que os teste são realizados.

Ferramentas de captura e registro de teclas são ideais a fim de armazenar os resultados do teste exploratório.

Ideal para teste de aplicações web modernas , e segue as ideias pregadas pela metodologia Agil.

Desenvolvimento em curtos ciclos e pouco tempo gasto para escrita de scripts e manutenção dos mesmos . <font color="red">Nota 1,0</font>

4. Considere os arquivos .java (Banco.java, Agencia.java, Conta.java e BankValidator.java). Nos próprios arquivos .java estão definidas as regras para cadastramento de cada um deles (Banco, Agencia e Conta). Desta forma, pede-se:
   1. (2.0 Pontos) Definir os cenários de teste suficientes para testar o cadastro e movimentações financeiras envolvendo bancos, agências e contas, conforme especificado. Para cada cenário definir os critérios de teste adequados à definição dos seus casos de teste.


   Testar o tamanho do numero do banco inserido que não pode ser igual a 3. <font color="red">O tamanho do numero do banco é exatamente = 3</font>

   **tnb** - Tamanho do Numero do banco.

   |id|descrição|V/I|E/S|
   |---|---|---|---|
   |CE01| td <> 3  |I|E|
   |CE02| td = 4  |V|E|

   Testar o número da agência que não pode ter tamanho menor que 3 ou maior que 5.

    **tna** - Tamanho do Numero da Agência.

   |id|descrição|V/I|E/S|
   |---|---|---|---|
   |CE03| tna < 3  |I|E|
   |CE04| tna > 5  |I|E|
   |CE05| tna = 4  |V|E|

   Testar o número da agência possui somente numeros.
    **agencia** - numero da agência.


   |id|descrição|V/I|E/S|
   |---|---|---|---|
   |CE06| agencia <> char  |I|E|
   |CE07| agencia = int  |V|E|


   Testar o nome da agência que deve ser formado por letras do alfabeto e que nao pode ter tamanho menor que 5 ou tamanho maior que 100.

   **nomea** - nome da agência.
   **tnome** - tamanho do nome da agencia

   |id|descrição|V/I|E/S|
   |---|---|---|---|
   |CE08| nomea = int  |I|E|
   |CE09| nomea = string  |V|E|
   |CE10| tnome < 5  |I|E|
   |CE11| tnome > 100   |I|E|


Testar o **tipo** de conta que não pode ser diferente de "Corrente" e "Poupanca".


   |id|descrição|V/I|E/S|
   |---|---|---|---|
   |CE13| tipo <> Corrente  |I|E|
   |CE14| tipo <> Poupanca  |I|E|
   |CE15| tipo = Corrente  |V|E|
   |CE16| tipo = Poupanca  |V|E|

Testar o **saldo** informado, que valida se o saldo é igual ou maior que o **valor** informado.

   |id|descrição|V/I|E/S|
   |---|---|---|---|
   |CE17| saldo < valor  |I|E|
   |CE18| saldo >= valor  |V|E|

Testar o nome da cidade informado como entrada, seguindo o mesmo raciociono do nome do banco.

   **nomec** - nome da cidade.
   **tnomec** - tamanho do nome da cidade

   |id|descrição|V/I|E/S|
   |---|---|---|---|
   |CE19| nomec = int  |I|E|
   |CE20| nomec = string  |V|E|
   |CE21| tnomec < 5  |I|E|
   |CE22| tnomec > 100   |I|E|
   |CE23| tnomec = 30   |V|E|

Testar se é valido **sacar** um valor em uma conta. Sendo que o **valor** do saque nao pode ser maior que o **saldo** da conta.

   |id|descrição|V/I|E/S|
   |---|---|---|---|
   |CE24| saldo < valor |I|E|
   |CE25| saldo >= valor |V|E|

   <font color="red">Nota 1,5</font>


   2. (2.0) Definir os casos de teste suficientes para a cobertura do teste de cada um dos cenários definidos. Documentar os casos de teste no seguinte padrão:

   Adicionei a Referencia de Classe de Equivalência para melhor relacionar entre o cenário definido e o caso de teste em questão.

   |CT|Valores de Entrada|Resultado esperado|
   |---|---|---|
   |CT03|9,99,7.00,64,15|"Aprovado"|CE02,CE04,CE06,CE10,CE13,CE14,CE17,CE20,CE23,CE24,CE27,CE29,CE30,CE33,CE37,CE42|

   Testando numero do banco.
   |CT|Valores de Entrada|Resultado esperado|Classe de Equivalência|
   |---|---|---|---|
   |CT01|5|"Valido"|CE01,CE02|
   |CT02|3|"Inválido"|CE01,CE02|


   Testando numero da agencia.
   |CT|Valores de Entrada|Resultado esperado|Classe de Equivalência|
   |---|---|---|---|
   |CT03|2|"Inválido"|CE03,CE04,CE05|
   |CT04|6|"Inválido"|CE03,CE04,CE05|
   |CT05|4|"Valido"|CE03,CE04,CE05|

   Testando numero da agencia.
   |CT|Valores de Entrada|Resultado esperado|Classe de Equivalência|
   |---|---|---|---|
   |CT06|"Universitario"|"Inválido"|CE06,C07|
   |CT07|3332|"Válido"|CE06,C07|

   Testando nome da agencia.
   |CT|Valores de Entrada|Resultado esperado|Classe de Equivalência|
   |---|---|---|---|
   |CT08|"Universitario"|"Valido"|CE08,CE09,CE10,CE11,CE12|
   |CT09|3332|"Inválido"|CE06,C07|CE08,CE09,CE10,CE11,CE12|
   |CT10|"ab"|"Inválido"|CE06,C07|CE08,CE09,CE10,CE11,CE12|

   Testando tipo de conta.
   |CT|Valores de Entrada|Resultado esperado|Classe de Equivalência|
   |---|---|---|---|
   |CT11|"ppp"|"Inválido"|CE13,CE14,CE15,CE16|
   |CT12|"Poupanca"|"Válido"|CE13,CE14,CE15,CE16|
   |CT13|"Corrente"|"Válido"|CE13,CE14,CE15,CE16|

   Testando o saldo informado.
   |CT|Valores de Entrada|Resultado esperado|Classe de Equivalência|
   |---|---|---|---|
   |CT14|25.00,25.00|"Válido"|CE17,CE18|
   |CT15|10.00,25.00|"Inválido"|CE17,CE18|

   Testando o nome da cidade.
   |CT|Valores de Entrada|Resultado esperado|Classe de Equivalência|
   |---|---|---|---|
   |CT16|"Goiânia"|"Valido"|CE08,CE09,CE10,CE11,CE12|
   |CT17|3332|"Inválido"|CE19,CE20|CE21,CE22,CE23|
   |CT18|"ab"|"Inválido"|CE19,CE20|CE21,CE22,CE23|


   Testando a movimentação **saque** .
   |CT|Valores de Entrada|Resultado esperado|Classe de Equivalência|
   |---|---|---|---|
   |CT19|40.00,50.00|"Inválido"|CE24,CE25|
   |CT20|45.00,5.00|"Válido"|CE24,CE25|

   <font color="red">Nota 1,0</font>

   3. (3.0 Pontos) Implementar (na linguagem de programação java) as classes para o teste da criação dos objetos e das movimentações financeiras envolvendo bancos e agências e contas.

 <font color="red">Nota 1,0</font>


INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing.
3. Forma de Entrega: arquivo compactado contendo:
   1. Este arquivo md, respondido.
   2. Classes de teste para (BancoTest, AgenciaTest e ContaTest);
   3. O arquivo compactado deverá ter o seguinte nome prova_p2<mat>.zip, onde mat é o número da matrícula do aluno(a).
5. Data da Entrega: 12/04/2022, as 22hs.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
7. Obs: segue no mesmo pacote o arquivo "org.apache.commons.lang.StringUtils", que é uma dependência do projeto. É deve ser inserida no _classpath_ do projeto de implementação da questão 4, caso não esteja utilizando o _maven_.
