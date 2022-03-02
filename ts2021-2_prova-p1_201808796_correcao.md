<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P1 - 16/02/2022</p>

Matrícula: 201808796
Nome:Gabriel Cândido Gomes Mendonça

<p><font color=red>Nota: 5,3.</font></p>

1. Quanto ao objetivo do Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Qual o objetivo primário da atividade de teste de software?
      O objetivo principal é revelar a presença de defeitos nos softwares. Reduzindo assim os riscos de falhas. <font color=green>Certo.</font>
   2. (**0,5 ponto**) O que acontece, quando não se atinge este objetivo primário?
      O software lançado em fase de implatação para o usuário poderá conter defeitos de execução, falhas nas entradas, valores fora do intervalo aceito para os dados.
      Além de funcionalidades executando ou realizando ações longe do que foi definido. <font color=red>Errado.</font>
2. (**1,0 ponto**) Explique o que é o teste exaustivo e porque sua execução não é possível.
      Teste exaustivel é a estratégia de testar todas as possibilidades possiveis dentro do software.
      Não é possivel pois existem diferentes cenários de aplicação e execução do software sendo impossivel mensurar de forma exata todos casos de execução.Levando a testar apenas os casos mais impactantes e importantes dentro do software. <font color=green>Certo.</font>
3. (**1,0 ponto**) Cite pelo menos duas limitações da Técnica de Teste Funcional e duas da Técnica de Teste Estrutural.

      Teste Funcional: Depende de uma boa especificação de requisitos, sendo geralmente nao executado corretamete.
      Não há garantia de execução de partes criticas e essenciais do software. <font color=green>Certo.</font>

      Teste Estrutural: Caminhos da especificação podem ser esquecidos na etapa de implementação.
      Um módulo do software pode falhar em alguns casos e ser executado  corretamente em outros. <font color=green>Certo.</font>

4. (**1,0 ponto**) Descreva pelo menos um dos quatro níveis de teste constantes da literatura especializada.
      Unidade
      Integração
      Sistema
      Aceitação
      <font color=orange>Parcialmente correto. Você identificou os níveis, mas não descreveu um deles. Nota 0,3.</font>
5. (**1.0 ponto**)Descreva qual o propósito do critério de teste funcional Particionamento por Classes de Equivlência.

      É um criterio de teste funcional, que busca reduzir o número de testes, além de procurar garantir uma boa cobertura de código.
      Usando um concepção de , que uma classe de equivalência revela um erro, e qualquer caso de teste dessa mesma classe tambem revelaria. <font color=green>Certo.</font>

6. (**1.00 ponto**) Existe algum tipo de hierarquia em relação aos critérios de teste estrutural, todos os nós, todos os arcos e todos os caminhos? Se sim, explique-a, considerando a perspectiva dos níveis de cobertura desejados.

      Deve se considerar o caminho, ou seja, a sequência de execução desde o ponto de entrada e termina com um ponto de saída.

      Sendo que um nó representa uma ou mais instruções que são executados em sequência, primeiro a instrução de um nó sendo executada, todas as demais intruções daquele nó serão executadas.

      O arco ou aresta, é o fluxo de controle entre os blocos de comandos ou nós.
<font color=red>Errado.</font>
7. Considere a especificação, a seguir, de um hipotético programa que objtiva a classificação de um triângulo, a partir dos valores informados para os seus três lados.

   a) Dado um triângulo cujos segmentos medem A, B e C, que são números inteiros positivos na faixa de 0 a 100. Esse triângulo somente existirá se: (A + B < C) ou (A + C < B) ou (B + C < A).



   b) Quanto às medidas dos seus lados o triângulo, poderá ser classicado em:
         • Isósceles = quando possui dois lados com a mesma medida;
         • Escaleno = quando todos os seus lados têm medidas diferentes;
         • Equilátero = quando todos os lados tem a mesma medida;
         • Acutângulo = quando o quadrado de um dos seus lados é menor que a soma do quadrado dois outros dois. (A<sup>2</sup> < B<sup>2</sup> + C<sup>2</sup>).
         • Retângulo: quando o quadrado de um dos seus lados é igual à soma do quadrado dois outros dois. (A<sup>2</sup> = B<sup>2</sup> + C<sup>2</sup>).
         • Obtusângulo: quando o quadrado de um dos seus lados é maior que a soma do quadrado dois outros dois. A<sup>2</sup> > B<sup>2</sup> + C<sup>2</sup>.

7.1 (**2.0 pontos**) Definir uma tabela de decisão para o teste tanto da existência do triângulo, quanto para a definição do seu tipo. Consulte exemplo de tabela de decisão na tarefa 005.
<div>
  <image src="tabelaf_decisao_P1.png">
</div>

<font color=red>Errado.</font>

7.2 (**2.0 pontos**) Criar os conjunto de casos de teste necessários para a cobertura das combinações constantes da tabela de decisão, seguindo o seguinte padrão:
|CT|Lado A|Lado B|Lado C|Resultado|
|---|---|---|---|---|
|CT01  | 25  | 25  | 30  | Isóceles  |
|CT02  | 25  | 30  | 35  | Escaleno  |
|CT03  | 25  | 25  | 25  | Equilátero |
|CT04  | 2  | 4  | 5  | Acutângulo |
|CT05  | 4  | 3  | 5  | Retângulo |
|CT06  | 2  | 3  | 9  | Obtusângulo |

<font color=orange>Parcialmente correto. Faltou o teste se é ou não um triângulo. Nota 1,5.</font>


INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing
3. Forma de Entrega: Entregar este arquivo, editado com suas respostas, no formato .md, nominado da seguinte forma: ts2021-2_prova-p1_mat.md, onde mat deverá ser substituído pelo número da sua matrícula.
4. **Entrega diferente da especificada não será avaliada.**
5. Data da Entrega: 22/02/2022, as 23h59min.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
