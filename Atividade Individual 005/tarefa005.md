## Tarefa 005 - 08/02/2022 - Grafo de Causa e Efeito / Tabela de Decisão.

1.Considere o seguinte cenário: Uma corretora de seguros concede desconto sobre o prêmio anual de seguro de automóvel, aos seus segurados conforme as regras a seguir:
|Sexo|Idade (anos)|Estado Civil|Desconto (%)|
|---|---|---|---|
|Masculino|< 25|Solteiro|0|
|Masculino|< 25|Casado|5|
|Masculino|>= 25|Solteiro|10|
|Masculino|>= 25|Casado|15|
|Feminino|< 25|Solteira|5|
|Feminino|< 25|Casada|10|
|Feminino|>= 25|Solteira|15|
|Feminino|>= 25|Casada|20|

  Grafo de causa e efeito:
   <div align=center>
     <img src="Grafo.png">
   </div>
   Tabela de decisão:
   <div align=center>
     <img src="TabeladeDecisão.png">
   </div>
   

|CT|Sexo|Estado Civil|Idade|Valor de Entrada|Valor Esperado|
|---|---|---|---|---|---|

|CT01|Masculino|Solteiro|15|R$ 2.000,00|R$ 2.000,00|
|CT02|Masculino|Solteiro|30|R$ 2.000,00|R$ 1.800,00|
|CT03|Masculino|Casado|23|R$ 2.000,00|R$ 1.900,00|
|CT04|Masculino|Casado|45|R$ 2.000,00|R$ 1.700,00|
|CT05|Feminino|Solteira|21|R$ 2.000,00|RS 1.900,00|
|CT06|Feminino|Solteira|32|R$ 2.000,00|R$ 1.700,00|
|CT07|Feminino|Casada|17|R$ 2.000,00|R$ 1.800,00|
|CT08|Feminino|Casada|54|R$ 2.000,00|R$ 1.600,00|

