//Incluir as bibliotecas
#include <stdio.h>
#include <stdlib.h>

//Criar a função principal da linguagem C
main()

//Abrir o código com chave
{
int num_projeto;
float valor;
char operacao;
//Criar uma estrutura struct
struct projeto
{
int numero_projeto;
float recursos;
};
printf("\n----- Cadastro dos Valores Iniciais dos Projetos -------\n\n\n");
struct projeto lista_projetos[10];
for (int i = 0; i<=9; i++)
{

lista_projetos[i].numero_projeto=i;

printf("Entre com o valor do recurso incial do projeto %d: \n", i);
scanf("%f.2", &lista_projetos[i].recursos);
 }
 printf("\n----- Movimentacao financeira dos Projetos -------\n\n\n");
 
 
 while (true){ // esse codigo faz com que tudo que esteja dentro deste bloco seja repatido indefinidamente. A forma de sair desse while está dentro do próprio bloco (break).
 	
 	puts("########### NOVA MOVIMENTACAO DE RECURSOS ###############");
 	
 	printf("Entre com o numero do projeto que voce quer movimentar(0 a 9): \n(Obs: digite -1 para encerrar programa) \n");
	scanf("%d", &num_projeto);
	
	if (num_projeto == -1){ // resquisito para sair do while e ir direto para impressão dos saldos
		break;
	}
	
	if (num_projeto < 0 && num_projeto > 9){ // qualquer numero de projeto digitado que nao esteja entre 0 e 9, será invalido e o sistema pedirá outro numero.
		puts("Numero de projeto invalido. Tente novamente. \n");
		continue;
	}
	
	printf("Entre com um valor: \n");
	scanf("%f.2", &valor);
	 
	printf("Entre com o tipo de recurso para receita r para despesa d: \n");
	scanf(" %c", &operacao);
	 
	if (operacao == 'r')
	{
		lista_projetos[num_projeto].recursos=lista_projetos[num_projeto].recursos+valor;
	}
	else if (operacao == 'd')
	{
		lista_projetos[num_projeto].recursos=lista_projetos[num_projeto].recursos-valor;
	}
	else
	{
		printf("Este tipo de operacao nao existe. Recursos nao alterados. Operacao cancelada! \n\n");
		continue; // volta pro inicio do while, pedindo novamente um novo numero de projeto.
	}
	 
	printf("O novo saldo do recurso do projeto %d eh: %.2f \n\n", num_projeto, lista_projetos[num_projeto].recursos);
 }
 
puts("\n\n ############# SALDO DAS CONTAS DOS PROJETOS ################ \n\n");

// usando o for para mostrar os recursos atuais de todos os projetos.
for (int i = 0; i<=9; i++)
{
	printf("Saldo do projeto %d: R$ %.2f\n", i, lista_projetos[i].recursos);
}
 
}
