## Tarefa 005 - 08/02/2022 - Grafo de Causa e Efeito / Tabela de Decis�o.

1.Considere o seguinte cen�rio: Uma corretora de seguros concede desconto sobre o pr�mio anual de seguro de autom�vel, aos seus segurados conforme as regras a seguir:
|Sexo|Idade (anos)|Estado Civil|Desconto (%)|
|---|---|---|---|
|Masculino|< 25|Solteiro|0|
|Masculino|< 25|Casado|5|
|Masculino|> 25|Solteiro|10|
|Masculino|> 25|Casado|15|
|Feminino|< 25|Solteira|5|
|Feminino|< 25|Casada|10|
|Feminino|> 25|Solteira|15|
|Feminino|> 25|Casada|20|

2. Solicita-se:
   1. Gera��o do grafo de causa e efeito para representar este cen�rio.
      1. Anexar a este arquivo a imagem do grafo.
   2. Gera��o da tabela de decis�o para representar o cen�rio.
      1. Editar este arquivo e adicionar a tabela de decis�o.

 
	T1	T2	T3	T4	T5	T6	T7	T8	   
Condi��es									   
Masculino									   
Feminino									   
Idade<25									   
Idade>25									   
Solteiro									   
Casado									   
A��es									   
Desconto 0%									   
Desconto 5%									   
Desconto 10%									   
Desconto 15%									   
Desconto 20%									 


   3. Gera��o do conjunto de casos de teste suficientes para cobrir todos os cen�rios, constantes do grafo e da tabela de decis�o.
      1. Editar este arquivo e adicionar a tabela com os casos de teste, conforme exemplos disponibilizados em tarefas anteriores.

 
	T1	T2	T3	T4	T5	T6	T7	T8	   
Condi��es									   
Masculino	X	X	X	X					   
Feminino					X	X	X	X	   
Idade<25	X			X		X	X		   
Idade>25		X	X		X			X	   
Solteiro	X		X		X	X			   
Casado		X		X			X	X	   
A��es									   
Desconto 0%	X								   
Desconto 5%				X		X			   
Desconto 10%			X				X		   
Desconto 15%		X			X				   
Desconto 20%								X	 

   4. Em rela��o aos casos de teste, considere o valor do seguro de R$ 2.000,00 (Dois mil reais). Desta forma, o valor esperado, do resultado do caso de teste, deve ser o valor l�quido a ser pago. Ou seja, o pr�mio deduzido do valor correspondente ao percentual do desconto obtido pelo cliente.

Caso de Teste � Seguro R$ 2.000,00
 
	T1	T2	T3	T4	T5	T6	T7	T8	   
Condi��es									   
Masculino	X	X	X	X					   
Feminino					X	X	X	X	   
Idade<25	X			X		X	X		   
Idade>25		X	X		X			X	   
Solteiro	X		X		X	X			   
Casado		X		X			X	X	   
A��es									   
Desconto 0%	X								   
Desconto 5%				X		X			   
Desconto 10%			X				X		   
Desconto 15%		X			X				   
Desconto 20%								X	   
Valor L�quido
	2000,00	1700,00	1800,00	1900,00	1700,00	1900,00	1800,00	1600,00	 


INSTRU��ES:
1. Tipo: Tarefa Individual;
2. Local de Entrega: Reposit�rio pessoal, no github. O arquivo a ser entregue � este mesmo, editado com a inclus�o dos dados solicitados.
3. Data da Entrega: 14/02/2022, as 23h59min.
4. Crit�rio de Aceita��o: Arquivo entregue com os dados solicitados.

