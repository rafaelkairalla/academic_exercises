# academic_exercises
Exercícios académicos em linguagem C.

/*#include<stdio.h>
#include<math.h>

int main()
{
int numero1, numero2, numero3, numero4, soma;

scanf("%d",&numero1);
scanf("%d",&numero2);
scanf("%d",&numero3);
scanf("%d",&numero4);

if(numero1 > numero2 && numero1 > numero3 && numero1 > numero4)
{
soma = (numero2 + numero3 + numero4);
printf("%d\n",soma);
}

else if(numero2 > numero1 && numero2 > numero3 && numero2 > numero4)
{
soma = numero1 + numero3 + numero4;
printf("%d\n",soma);
}

else if(numero3 > numero1 && numero3 > numero2 && numero3 > numero4)
{
soma = numero1 + numero2 + numero4;
printf("%d\n",soma);
}

else if(numero4 > numero1 && numero4 > numero2 && numero4 > numero3)
{
soma = numero1 + numero2 + numero3;
printf("%d\n",soma);
}

return 0;

}

/*#include<stdio.h>
#include<math.h>

int main()
{
int numero;

scanf("%d",&numero);

if (((numero % 5)==0) && ((numero % 3)==0)){
printf("O NUMERO E DIVISIVEL\n");
}
else{
printf("O NUMERO NAO E DIVISIVEL\n");
}
return 0;
}


/*#include<stdio.h>
#include<math.h>

int main()
{
float a, b, c, delta, X1, X2;

scanf("%f",&a);
scanf("%f",&b);
scanf("%f",&c);

delta = (pow(b,2) - 4 * a * c);
X1 = (-b + sqrt(delta))/(2 * a);
X2 = (-b - sqrt(delta))/ (2 * a);

if (delta == 0)
{
printf("RAIZ UNICA\n");
printf("X1 = %.2f\n",X1);
}

else if (delta < 0 )
{
printf("RAIZES IMAGINARIAS\n");
}

else if (delta > 0 )
{
printf("RAIZES DISTINTAS\n");
printf("X1 = %.2f\n",X1);
printf("X2 = %.2f\n",X2);
}

return 0;

}


/*#include<stdio.h>
#include<math.h>

int main()
{
int x, y;

scanf("%d",&x);

if(x < 1)
{
y = x;
printf("Y = %d\n",y);
}	

else if(x == 1)
{
y = 0;
printf("Y = %d\n",y);
}

else if(x > 1)
{
y = pow(x,2);
printf("Y = %d\n",y);
}

return 0;
}


/*#include<stdio.h>
#include<math.h>
#include<string.h>
int main()
{
int ano, anobissexto, mesfevereirobissexto;
char mes[15];

scanf("%s",mes);
scanf("%d",&ano);

if (ano % 4==0 ) {
anobissexto = 366;
mesfevereirobissexto = 29;
}

else {
anobissexto = 365;
mesfevereirobissexto = 28;
}

if (strcmp(mes,"JANEIRO") == 0){
printf("DIAS = 31\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"FEVEREIRO") == 0){
printf("DIAS = %d\n",mesfevereirobissexto);
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"MARCO") == 0){
printf("DIAS = 31\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"ABRIL") == 0){
printf("DIAS = 30\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"MAIO") == 0){
printf("DIAS = 31\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"JUNHO") == 0){
printf("DIAS = 30\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"JULHO") == 0){
printf("DIAS = 31\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"AGOSTO") == 0){
printf("DIAS = 31\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"SETEMBRO") == 0){
printf("DIAS = 30\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

else if (strcmp(mes,"OUTUBRO") == 0){
printf("DIAS = 31\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}
else if (strcmp(mes,"NOVEMBRO") == 0){
printf("DIAS = 30\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}
else if (strcmp(mes,"DEZEMBRO") == 0){
printf("DIAS = 31\n");
printf("DIAS NO ANO = %d\n",anobissexto);
}

return 0;	

}


/*#include<stdio.h>
#include<math.h>

int main()
{
int numerosala, capacidade, alunosmatriculados;

scanf("%d",&numerosala);
scanf("%d",&capacidade);
scanf("%d",&alunosmatriculados);

if (alunosmatriculados >= capacidade)
{
printf("SALA = %d\n",numerosala);
printf("CAPACIDADE = %d\n",capacidade);
printf("CADEIRAS OCUPADAS = %d\n",alunosmatriculados);
printf("SALA LOTADA\n");
}

else if (alunosmatriculados < capacidade)
{
printf("SALA = %d\n",numerosala);
printf("CAPACIDADE = %d\n",capacidade);
printf("CADEIRAS OCUPADAS = %d\n",alunosmatriculados);
printf("SALA NAO LOTADA\n");
}

return 0;
}


/*#include<stdio.h>
#include<math.h>
#include<string.h>

int main()
{
int numerodependentes;
float salariominimo, salariofunc, taxaimposto, taxaimpostosalario, impostoderenda, impostobruto, impostoliquido, salariomaximo12, salariomaximo5, calcdependentes; 

scanf("%f",&salariominimo);
scanf("%d",&numerodependentes);
scanf("%f",&salariofunc);
scanf("%f",&taxaimposto);

salariomaximo12 = salariominimo * 12;
salariomaximo5 = salariominimo * 5;
calcdependentes = numerodependentes * 300.00;
taxaimpostosalario = (taxaimposto / 100) * salariofunc;

if ( salariofunc > salariomaximo12){
impostobruto = 0.2 * salariofunc;
impostobruto = 0.04 * impostobruto + impostobruto;
} 

else if (salariofunc >  salariomaximo5){
impostobruto = 0.08 * salariofunc;
impostobruto = 0.04 * impostobruto + impostobruto;
}

else if (salariofunc <= salariomaximo5){
impostobruto = 0;
}

impostoliquido = impostobruto - calcdependentes ;
impostoderenda = impostoliquido - taxaimpostosalario;

if (impostoderenda == 0){
printf("IMPOSTO BRUTO = %.2f\n",impostobruto);
printf("IMPOSTO LIQUIDO = %.2f\n",impostoliquido);
printf("RESULTADO = %.2f\n",impostoderenda);
printf("IMPOSTO QUITADO\n");
}

else if (impostoderenda < 0){
printf("IMPOSTO BRUTO = %.2f\n",impostobruto);
printf("IMPOSTO LIQUIDO = %.2f\n",impostoliquido);
printf("RESULTADO = %.2f\n",impostoderenda);
printf("IMPOSTO A RECEBER\n");
}

else if (impostoderenda > 0){
printf("IMPOSTO BRUTO = %.2f\n",impostobruto);
printf("IMPOSTO LIQUIDO = %.2f\n",impostoliquido);
printf("RESULTADO = %.2f\n",impostoderenda);
printf("IMPOSTO A PAGAR\n");
}

return 0;
}


/*#include<stdio.h>
#include<math.h>
#include<string.h>

int main()
{
int contacliente, consumoagua;
float formula;
char tipoconsumidor[15];

scanf("%d",&contacliente);
scanf("%d",&consumoagua);
scanf("%s",tipoconsumidor);

if (strcmp(tipoconsumidor,"RESIDENCIAL") == 0){
formula = 5.00 + (0.05 * consumoagua);
printf("CONTA = %d\n",contacliente);
printf("VALOR DA CONTA = %.2f\n",formula);
}

if (strcmp(tipoconsumidor,"COMERCIAL") == 0 && consumoagua <= 80 ){
formula = 500.00;
printf("CONTA = %d\n",contacliente);
printf("VALOR DA CONTA = %.2f\n",formula);
}

else if (strcmp(tipoconsumidor,"COMERCIAL") == 0 && consumoagua > 80 ){
formula = 500.00 + ((consumoagua - 80) * 0.25);
printf("CONTA = %d\n",contacliente);
printf("VALOR DA CONTA = %.2f\n",formula);
}

if (strcmp(tipoconsumidor,"INDUSTRIAL") == 0 && consumoagua <= 100){
formula = 800.00;
printf("CONTA = %d\n",contacliente);
printf("VALOR DA CONTA = %.2f",formula);
}
else if (strcmp(tipoconsumidor,"INDUSTRIAL") == 0 && consumoagua > 100){
formula = 800.00 + ((consumoagua - 100 )* 0.04);
printf("CONTA = %d\n",contacliente);
printf("VALOR DA CONTA = %.2f\n",formula);
}

return 0;	

}


/*#include<stdio.h>
#include<math.h>
#include<string.h>
int main()
{
float preconormal, descontopromo, precototal;
char dia[15], categoria[15];

scanf("%f",&preconormal);
scanf("%s",dia);
scanf("%s",categoria);

if (strcmp(dia,"SEGUNDA") ==0 || strcmp(dia,"TERCA") ==0 || strcmp(dia,"QUINTA") == 0){
descontopromo = preconormal - (0.4 * preconormal) ;
}

else if (strcmp(dia,"QUARTA") == 0|| strcmp(dia,"SEXTA") == 0|| strcmp(dia,"SABADO") ==0|| strcmp(dia,"DOMINGO")==0){
descontopromo = 0;
}

if (strcmp(categoria,"LANCAMENTO") == 0){
preconormal = (preconormal * 0.15);	
}

else if (strcmp(categoria,"COMUM") == 0){
preconormal = preconormal;	
}

precototal = descontopromo + preconormal;
printf("PRECO FINAL = %.2f\n",precototal);

return 0;	

}


/*#include<stdio.h>
#include<math.h>
#include<string.h>
#define pi 3.1415

int main()
{

   float raio, altura, volume, area;
   char tipo[10];

   scanf("%f",&raio);
   scanf("%f",&altura);
   scanf("%s",tipo);

   if (strcmp(tipo,"CONE")==0){
       volume = ((pi * pow(raio,2)) * altura) / 3;
       area = (pi * raio) * sqrt(pow(raio,2) + pow(altura,2));
       printf("VOLUME = %.2f\n",volume);
       printf("AREA = %.2f\n",area);
   }

else if (strcmp(tipo,"CILINDRO")==0){
       volume = ((pi * pow(raio,2)) * altura);
       area = (2 * pi) * (raio * altura);
       printf("VOLUME = %.2f\n",volume);
       printf("AREA = %.2f\n",area);
   }

   else if (strcmp(tipo,"ESFERA")==0){
       volume = (pi * 4 * pow(raio,3)) / 3;
       area = (4 * (pi * pow(raio,2)));
       printf("VOLUME = %.2f\n",volume);
       printf("AREA = %.2f\n",area);
   }

return 0;
}
Exercício 10
Um certo aço é classificado de acordo com o resultado de três testes abaixo, que devem determinar se o mesmo satisfaz as especificações:
1. Conteúdo de Carbono abaixo de 7;
2. Dureza Rockwell maior do que 50;
3. Resistência á tração maior do que 80.000 psi;

/*#include<stdio.h>
#include<math.h>
#include<string.h>

int main()
{
int conteudo, dureza, resistencia;

scanf("%d",&conteudo);
scanf("%d",&dureza);
scanf("%d",&resistencia);    

if (conteudo < 7 && dureza > 50 && resistencia > 80000){
printf("ACO DE GRAU = 10\n");
}

else if (conteudo < 7 && dureza > 50 && resistencia <= 80000) {
printf("ACO DE GRAU = 9\n");
}

else if (conteudo < 7 && dureza <= 50 && resistencia <= 80000){
printf("ACO DE GRAU = 8\n");
}

else if (conteudo >= 7 && dureza <= 50 && resistencia <= 80000){
printf("ACO DE GRAU = 7\n");
}	

return 0;
}


/*#include<stdio.h>
#include<math.h>

int main()
{
int numero;

scanf("%d",&numero);

if (numero < 0)
{
printf("NEGATIVO\n");
}
else if (numero > 0)
{
printf("POSITIVO\n");
}

if (numero % 3 != 0)
{
printf("NAO MULTIPLO DE 3\n");
}

else if (numero % 3 == 0)
{
printf("MULTIPLO DE 3\n");
}
return 0;	
}


/*#include<stdio.h>
#include<math.h>

int main()
{
float salario, salarioreajustado;

scanf("%f",&salario);

if (salario <= 300.00){
salarioreajustado = (0.5 * salario) + salario;	
printf("SALARIO COM REAJUSTE = %.2f\n",salarioreajustado);
}

else if (salario > 300.00){
salarioreajustado = (0.3 * salario) + salario;	
printf("SALARIO COM REAJUSTE = %.2f\n",salarioreajustado);
}
return 0;	
}


/*#include<stdio.h>
#include<math.h>

int main()
{
float A, B, C;

scanf("%f",&A);
scanf("%f",&B);
scanf("%f",&C);

if (C > A + B  || A > B + C  || B > A + C ){
printf("NAO FORMAM UM TRIANGULO\n");
}

else if ( A != B && A != C &&  B != C ){
printf("TRIANGULO ESCALENO\n");
} 

else if ( A == B && A == C){
printf("TRIANGULO EQUILATERO\n");
}

else if (A == B || A == C || B == C){
printf("TRIANGULO ISOSCELES\n");
}

return 0;	
}


/*#include<stdio.h>
#include<math.h>

int main()
{
float A, B, C;

scanf("%f",&A);
scanf("%f",&B);
scanf("%f",&C);

if (pow(A,2) == pow(B,2) + pow(C,2)){
printf("TRIANGULO RETANGULO\n");
}

else if (pow(A,2) > pow(B,2) + pow(C,2)){
printf("TRIANGULO OBTUSANGULO\n");
}

else if (pow(A,2) < pow(B,2) + pow(C,2)){
printf("TRIANGULO ACUTANGULO\n");
}
return 0;	
}


/*#include<stdio.h>
#include<math.h>

int main()
{
float nota1, nota2, nota3, media;

scanf("%f",&nota1);
scanf("%f",&nota2);
scanf("%f",&nota3);

media = (nota1 + nota2 + nota3) / 3;

if (media >= 6.00){
printf("MEDIA = %.2f",media);
printf("APROVADO\n");
}

else if ( media < 6.00){
printf("MEDIA = %.2f\n",media);
printf("REPROVADO\n");
}	
return 0;	
}


/*#include<stdio.h>
#include<math.h>

int main()
{
int numero1, numero2, numero3;

scanf("%d",&numero1);
scanf("%d",&numero2);
scanf("%d",&numero3);

if (numero1 > numero2 && numero1 > numero3){
printf("MAIOR NUMERO = %d\n",numero1);
}

else if (numero2 > numero1 && numero2 > numero3){
printf("MAIOR NUMERO = %d\n",numero2);
}

else if (numero3 > numero1 && numero3 > numero2){
printf("MAIOR NUMERO = %d\n",numero3);
}

return 0;	
}


/*#include<stdio.h>
#include<math.h>

int main()
{
int cod_aluno;
float nota1, nota2, nota3, mediaponderada;

scanf("%d",&cod_aluno);
scanf("%f",&nota1);
scanf("%f",&nota2);
scanf("%f",&nota3);

if (nota1 > nota2 && nota1 > nota3){
mediaponderada = (( nota1 * 4 ) + (nota2 * 3) + (nota3 * 3)) /10;
}

else if (nota2 > nota1 && nota2 > nota3){
mediaponderada = (( nota2 * 4 ) + (nota1 * 3) + (nota3 * 3)) /10;
}

else if (nota3 > nota1 && nota3 > nota2){
mediaponderada = (( nota3 * 4 ) + (nota1 * 3) + (nota2 * 3.)) /10;
}

if (mediaponderada >= 5.00){
printf("CODIGO = %d\n",cod_aluno);
printf("NOTA 1 = %.2f\n",nota1);
printf("NOTA 2 = %.2f\n",nota2);
printf("NOTA 3 = %.2f\n",nota3);
printf("MEDIA = %.2f\n",mediaponderada);
printf("APROVADO\n");
}

else if (mediaponderada < 5.00){
printf("CODIGO = %d\n",cod_aluno);
printf("NOTA 1 = %.2f\n",nota1);
printf("NOTA 2 = %.2f\n",nota2);
printf("NOTA 3 = %.2f\n",nota3);
printf("MEDIA = %.2f\n",mediaponderada);
printf("REPROVADO\n");
}

return 0;	
}


/* 
* Author: Kelvin Santiago
* Create on: 07/06/2013
*/
#include<math.h>
#include<stdio.h>
#include<string.h>

int main(){

int n1,n2,n3,n4,n5,numero,aux, inverter;

scanf("%d",&numero);

n1 = numero / 10000;
aux = numero % 10000;
n2 = aux / 1000;
aux = aux % 1000;
n3 = aux / 100;
aux = aux % 100;
n4 = aux / 10;
n5 = aux % 10;

inverter = (n5 * 10000) + (n4 * 1000) + (n3 * 100) + (n2 * 10) + n1;

if (numero == inverter){
printf("O NUMERO E PALINDROMO\n");
}

else {
printf("O NUMERO NAO E PALINDROMO\n");
}

return 0;
}


#include <stdio.h>

#define TAM 2 //define constante

int main() {
    int vet1[TAM], vet2[TAM], vet3[TAM*2], i;

    //ler valores para o primeiro vetor
    for (i = 0; i < TAM; i++) {
        scanf("%i", &vet1[i]);
    }

    //ler valores para o segundo vetor
    for (i = 0; i < TAM; i++) {
        scanf("%i", &vet2[i]);
    }

    //preencher o terceiro vetor
    for (i = 0; i < TAM; i++) {
        vet3[i*2] = vet1[i];
    }
    for (i = 0; i < TAM; i++) {
        vet3[i*2+1] = vet2[i];
    }

    //mostra valores para o segundo vetor
    printf("Vetor 1: ");
    for (i = 0; i < TAM; i++) {
        printf("%i ", vet1[i]);
    }
    printf("\n");

    //mostra valores para o segundo vetor
    printf("Vetor 2: ");
    for (i = 0; i < TAM; i++) {
        printf("%i ", vet2[i]);
    }
    printf("\n");

    //mostra valores para o terceiro vetor
    printf("Vetor 3: ");
    for (i = 0; i < TAM*2; i++) {
        printf("%i ", vet3[i]);
    }

    return 0;
}


#include <stdio.h>
#include <stdlib.h>
#include <time.h>

#define TAM 7

int main() {
    int vet[TAM], i, acimaMedia = 0, soma = 0;
    float media;

    srand(time(NULL)); //planta uma nova semente

    //gera valores aleatorio para o vetor
    for (i = 0; i < TAM; i++) {
        vet[i] = rand()%51;
    }

    //determina a media
    for (i = 0; i < TAM; i++) {
        soma = soma + vet[i];
    }
    media = soma / (float)TAM;

    //determina quantos valores estao acima da media
    for (i = 0; i < TAM; i++) {
        if (vet[i] > media) {
            acimaMedia++;
        }
    }

    //mostrar valores do vetor
    printf("Vetor: ");
    for (i = 0; i < TAM; i++) {
        printf("%i ", vet[i]);
    }

    printf("\nMedia: %f", media);
    printf("\nAcima da media: %i", acimaMedia);

    return 0;
}


#include <stdio.h>
#include <stdlib.h>
int main(){
 char p1[30],p2[30];
 //captura palavras
 printf("Informe palavra 1: ");
 gets(p1);
 printf("Informe palavra 2: ");
 gets(p2);
 //verifica se sao iguais
 if(strcmp(p1,p2)==0)
 printf("\nPalavras sao iguais.");
 if(strcmp(p1,"papagaio")==0)
 printf("\nPalavra 1 igual papagaio.");
 if(strcmp(p2,"papagaio")==0)
 printf("\nPalavra 2 igual papagaio.");
 return 0;
}


#include <stdio.h>
#include <stdlib.h>
int main(){
 int i;
 char palavras[3][30];
 //captura palavras
 for(i=0;i<3;i++){
 printf("Informe palavra %d: ",i+1);
 gets(palavras[i]);
 }
 //EXIBE EM ORDEM INVERSA
 printf("\n::: Palavras em ordem inversa :::\n");
 for(i=2;i>=0;i--)
 printf("%s\n",palavras[i]);
 return 0;
}


#include <stdio.h>
#include <stdlib.h>
int main(){
 int i, j, m[3][3], v[3];
 //captura os elementos do vetor
 printf("::: Informe os elementos do vetor :::\n");
 for(i=0;i<3;i++){
 printf("Elemento[%d]= ",i);
 scanf("%d",&v[i]);
 }
 //captura os elementos da matriz
 printf("::: Informe os elementos da matriz :::\n");
 for(i=0;i<3;i++)
 for(j=0;j<3;j++){
 printf("Elemento[%d][%d]= ",i,j);
 scanf("%d",&m[i][j]);
 }
 //exibe valores originais
 printf("\n::: Valores Originais do Vetor :::\n");
 for(i=0;i<3;i++)
 printf("%d ",v[i]);
 printf("\n::: Valores Originais da Matriz :::\n");
 for(i=0;i<3;i++){
 for(j=0;j<3;j++)
 printf("%d ",m[i][j]);
 printf("\n");
 }
 //multiplica vetor pelas colunas da matriz
 for(i=0;i<3;i++)
 for(j=0;j<3;j++)
 m[i][j]=v[i]*m[i][j];
 //exibe valores multiplicados
 printf("\n::: Valores Multiplicados :::\n");
 for(i=0;i<3;i++){
 for(j=0;j<3;j++)
 printf("%d ",m[i][j]);
 printf("\n");
 }
 return 0;
}



