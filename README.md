# Gerador-de-relat-rios-t-cnicos-da-Manuten-o-Predial
Criei esse código no intuito de ajudar meu patrão à facilitar o preenchimento dos dados obtidos de oficinas da manutenção predial e no final gerar um relatório que tem como objetivo mostrar o percentual de satisfação da ofiina.



GERADOR DE PORCENTAGEM DE OFICINAS DE MANUTENÇÃO

#include<stdio.h>
#include<stdlib.h>
#include<locale.h>
main(){
	setlocale(LC_ALL, "Portuguese");
 float cgerada,pgerada,cex,pex,totge,totex;
 float perco,perprev, totperexe,totalpercent;
 char oficina;
 

printf("\nBEM-VINDO(A) A FERRAMENTA DE CÁLCULO PARA RELATÓRIO DE DESEMPENHO - CCO:\n\n");

 printf("PROJETO IDEALIZADO POR: Eduardo Cavalcante - VIVANTE\n\n");
  printf("****OBJETIVO: OTIMIZAR O PROCESSO DE PREENCHIMENTO DO RELATÓRIO TÉCNICO MENSAL****\n\n");
 printf("\OFICINA:\n");
 scanf("%s",&oficina);
 

 printf("Quantidade de OS corretivas geradas:\n");
 scanf("%f",&cgerada);
 printf("Quantidade de OS corretivas executadas:\n");
 scanf("%f",&cex);
  printf("Quantidade de OS preventivas geradas:\n");
 scanf("%f",&pgerada);
 printf("Quantidade de OS preventivas executadas:\n");
 scanf("%f",&pex);

totge = (cgerada+pgerada);
totex = (cex+pex);

perco = (cex*1/cgerada)*100;
perprev = (pex*1/pgerada)*100;
totalpercent=(totex*1/totge)*100;

printf("\n ==================================================================\n");


printf("\n\n RELATÓRIO - RESULTADO: \n\n");

printf("\n\n QUANTIDADE:\n\n");

printf("TOTAL DE CORRETIVAS GERADAS..................... %.f\n ",cgerada);
printf("TOTAL CORRETIVAS EXECUTADAS..................... %.f\n ",cex);
printf("PREVENTIVAS GERADAS............................. %.f\n ",pgerada);
printf("PREVENTIVAS EXECUTADAS.......................... %.f\n ",pex);
printf("TOTAL GERADAS................................... %.f\n ",totge);
printf("TOTAL EXECUTADAS................................ %.f\n ",totex);

printf("\n===================================================================\n");
printf("\n\n PORCENTAGEM:\n\n");
printf("PORCENTAGEM O.S CORRETIVAS (%%)....................... %.1f\n ",perco);
printf("PORCENTAGEM O.S PREVENTIVAS (%%)...................... %.1f\n ",perprev);
printf("PORCENTAGEM GERAL O.S (%%)............................ %.1f\n ",totalpercent);
printf("\n ==================================================================\n");





system("pause");




 
 
}
