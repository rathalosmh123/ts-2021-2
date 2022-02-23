## Tarefa 006 - 15/02/2022 - Grafo de Fluxo de Controle

1. Considere o fragmento de código implementado na Linguagem de Programação Java.

~~~java

public class Avaliacao {


1    public String avalia(double nota1, double nota2, int faltas, int cargaHoraria) throws ValoresInvalidosException{
2        String result;
3        double percentualFaltas = (faltas*100/cargaHoraria);
4        double media = (nota1 + nota2)/2;
5        if((nota1 < 0.0 || nota1 > 10) || (nota2 < 0.0 || nota2 > 10) || (faltas < 0 || faltas > cargaHoraria) || cargaHoraria < 0){
6            throw new ValoresInvalidosException();//result = "Valores Inválidos.";
7        }else if(percentualFaltas > 25.0){
8            result = "Reprovado por Falta.";
9        }else if(media < 3.0){
10            result = "Reprovado por Média.";
11        }else if(media >= 3.0 && media < 6.0){
12            result = "Prova Extra.";
13        }else{
14            result = "Aprovado.";
15        }
16        return result;
17    }
18 }
~~~

2. Pede-se:
   1. Desenhar o **Grafo do Fluxo de Controle**. Pode-se anexar a imagem, aqui neste arquivo.



 

   2. Calcular a complexidade ciclomática do código. Exemplo de coo calcular pode ser obtido no [link]
(https://www.treinaweb.com.br/blog/complexidade-ciclomatica-analise-estatica-e-refatoracao)


F�rmula usada : V(G) = E � N + 2 - onde E � o n�mero de arestas (setas) e N � o n�mero de n�s do grafo G.

			V(G) = 14 arestas - 12 Arestas + 2
			V(G) = 2 + 2 
			V(G) = 4

			


   3. Definir quantos caminhos de execução existem;


Existem 4 caminhos possiveis para execu��o.


   4. Definir os casos de teste necessários para se percorrer todos estes caminhos. Cada caso de teste deve ter o valor correspondente para cada variável de entrada e o valor esperado.



|Nota1|Nota2|faltas|Carga Horaria|Valor Esperado

6.0|8.0|18|64|Reprovado por Falta
4.0|4.0|0|64|Reprovado por M�dia 
5.5|5.0|4|64|Prova Extra
9.0|10.0|6|64|Aprovado


INSTRUÇÕES:
1. Tipo: Tarefa Individual;
2. Local de Entrega: _branch main/master_ do repositório pessoal do aluno, criado para a manutenção do controle de versão dos artefatos da disciplina. O arquivo a ser entregue, pode ser este mesmo, editado com as respostas das questões solicitadas.
3. Data da Entrega: 21/02/2021, as 23h59min.
4. Critério de Aceitação: arquivo entregue, conforme solicitado.
