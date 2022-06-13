//Trabalho de Christian Kevelyn, João Guilherme, Matheus P. Mufato, e Yago Paronetto.
//Sistema Escolar.

#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include <locale.h>

#define MAX_ALUNOS 50
#define MAX_PROFESSORES 50
#define MAX_CURSOS 50
#define MAX_TURMAS 50
#define SYMB '#';
#define ANSI_COLOR_RED     "\x1b[31m"
#define ANSI_COLOR_GREEN   "\x1b[32m"
#define ANSI_COLOR_YELLOW  "\x1b[33m"
#define ANSI_COLOR_BLUE    "\x1b[34m"
#define ANSI_COLOR_MAGENTA "\x1b[35m"
#define ANSI_COLOR_CYAN    "\x1b[36m"
#define ANSI_COLOR_RESET   "\x1b[0m"

void Texto(char let[26], int num){
	/*Função para gerar os textos grandes recebe como parametro o texto + um integer, converte o integer para char e concatena com o			
	  texto original do parametro, apos isso roda um loop do tamanho do texto final e dentro do loop existe um switch case que diante de cada
	  letra ou numero do texto, escreve uma matriz de 5x5 utilizando um loop mais uma condição especifica
	  por fim transfere a matrix 5x5 para uma matrix de 5x100.
	*/
	char let2[26-strlen(let)];					
	char let3[strlen(let)+strlen(let2)];							
	char letra[5][5], palavra[5][100];		
	strcpy(let3,let);
	if(num>-1){
		itoa(num,let2,10);
		strcat(let3,let2);
	}
	int i, j, l, k=0;
	for(i = 0; i<5; i++){
		for(j=0;j<100;j++){
			palavra[i][j]=' ';
		}
	}
	void limparMatriz(){
		for(i = 0; i<5; i++){
			for(j=0;j<5;j++){
				letra[i][j]=' ';
			}
		}
	}
	void transferirMatriz(){
		for(i = 0; i<5; i++){
			for(j=0;j<5;j++){	
				palavra[i][j+(l*5)+k] = letra[i][j];
			}
		}
		k++;	
	}
	for(l =0;l<sizeof(let3);l++){
		switch(let3[l]){
			case('a'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i<5 && i >0 &&j==0) || (i<5&&i>0&&j==4) || (i==2&&j<5)|| (i==0&&j<4&&j!=0)) {
							letra[i][j]=SYMB;	
						}
					}
				}	
				transferirMatriz();
			break;
			case('b'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i<2&&j==4)|| (i>2&&j==4)|| (i==4&&j<4 )|| (i==2&&j<4 )|| (i==0&&j<5 )) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;	
			case('c'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i>0&&j==0&&i!=4) || (i==0&&j<5&&j>0 )|| (i==4&&j<5&&j!=0 )) {
							letra[i][j]=SYMB;	
						}
					}
				}	
				transferirMatriz();
			break;
			case('d'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || ((i<4&& i>0 &&j==4)&& (i>0&&j==4))|| (i==4&&j<4 )| (i==0&&j<4 )) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case ('e'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==0 && j<=3)||(i==2 && j<=2)||(i==4 && j<=3)||(i==1 && j==0)||(i==3 && j==0)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case ('f'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==0 && j<=3)||(i==2 && j<=2)||(i==4 && j==0)||(i==1 && j==0)||(i==3 && j==0)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('g'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>0&&j==0 || (i==3&&j==4) || (i==2&&j==3)|| (i==0&&j<5 )|| (i==4&&j<5 )) {
							letra[i][j]=SYMB;	
						}
					}
				}	
				transferirMatriz();
			break;
			case('h'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i>=0&&j==4)|| (i==2&&j<5 )) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('i'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i<5&&j==2) {
							letra[i][j]=SYMB;	
						}
					}	
				}
				transferirMatriz();	
			break;
			case('j'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i<5&&j==2) ||  (i==0&&j<5 )||(i==4 && j<3)) {
							letra[i][j]=SYMB;	
						}
					}	
				}
			transferirMatriz();	
			break;
			case('k'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i<5 &&j==0) || (i==2 &&j==1)|| (i==3 &&j==2)|| (i==4 &&j==3|| (i==1 &&j==2)|| (i==0 &&j==3))) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('l'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i==4&&j<5 )) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('m'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i>=0&&j==4) || (i==1 && j==1)|| (i==1 && j==3)|| (i==2 && j==2)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('n'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i>=0&&j==4) || (i==1 && j==1)|| (i==2 && j==2)|| (i==3 && j==3)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('o'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>0&&j==0&&i!=4 || (i>0&&j==4&&i!=4) || (i==0&&j<5&&j!=4&&j!=0 )|| (i==4&&j<5&&j!=4&&j!=0 )) {
							letra[i][j]=SYMB;	
						}
					}
				}	
				transferirMatriz();
			break;
			case('p'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i<2&&j==4)|| (i==2&&j<4 )|| (i==0&&j<5 )) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('q'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>0&&j==0 || (i>0&&j==4) || (i==0&&j<5 )|| (i==4&&j<5 ) ||(i==j && i>2)) {
							letra[i][j]=SYMB;	
						}
					}
				}	
				transferirMatriz();
			break;
			case('r'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i<2&&j==4)|| (i==2&&j<4 )|| (i==0&&j<5 ) || ((i==j)&&(i>2))) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('s'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==4&&j<4 ) || (i==0&&j<5&&j>0) ||(i==3&&j==4)||(i==2&&j<4&&j>0)||(i==1&&j==0)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('t'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i<5&&j==2) ||  (i==0&&j<5 )) {
							letra[i][j]=SYMB;	
						}
					}	
				}
				transferirMatriz();	
			break;
			case('u'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i>=0&&j==4)|| (i==4&&j<5 )) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('v'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==0&&j==0)||(i==0&&j==4)|| (i==1&&j==0)||(i==1&&j==4)||(i==2&&j==3)||(i==2&&j==1)||(i==3&&j==3)||(i==3&&j==1)||(i==4&&j==2)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('w'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>=0&&j==0 || (i>=0&&j==4) || (i==3 && j==1)|| (i==3 && j==3)|| (i==4 && j==2)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('x'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(((i==j)||(j==4-i))) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('y'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==5-j)||(i==1&&j==0)||(i==2&&j==1)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case('z'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==4&&j<5 ) || (i==0&&j<5) || (i==4-j)) {
							letra[i][j]=SYMB;	
						}
					}
				}
			transferirMatriz();
			break;
			case(' '):
				limparMatriz();
				transferirMatriz();
			break;
			case('1'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i<5&&j==2)||(i==4&&j>0&&j<4)||(i==1&&j==1)) {
							letra[i][j]=SYMB;	
						}
					}
				}	
				transferirMatriz();	
			break;
				case('2'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==4&&j<5 ) || (i==0&&j<4&&j>0) || (i==4-j&&i>0)||(i==1&&j==0)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
			case('3'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==4&&j<4&&j>0 ) || (i==0&&j<4&&j>0) || (i==2&&j<4&&j>0)||(i==1&&j==4)||(i==3&&j==4)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
			case('4'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((j==3&&i>-1)||(j==2&&i==1)||(j==1&&i==2)||(j>-1&&i==3)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
			case('5'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((j==0&&i>-1&&i<3)||(i==0&&j>-1)||(i==2&&j<4)||(i==3&&j==4)||(i==4&&j<4)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
			case('6'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((j==0&&i==3)||(i==0&&j>0&&j<4)||(i==2&&j<4&&j>0)||(i==3&&j==4)||(i==4&&j<4&&j>0)||(i==1&&j==0)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
			case('7'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if( (i==0&&j<5) || (i==4-j)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
			case('8'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((j==0&&i==3)||(i==0&&j>0&&j<4)||(i==2&&j<4&&j>0)||(i==3&&j==4)||(i==4&&j<4&&j>0)||(i==1&&j==0)||(i==1&&j==4)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
			case('9'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if((i==0&&j>0&&j<4)||(i==2&&j<4&&j>0)||(i==3&&j==4)||(i==4&&j<4&&j>0)||(i==1&&j==0)||(i==1&&j==4)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
			case('0'):
				limparMatriz();
				for(i = 0; i<5; i++){
					for(j=0;j<5;j++){
						if(i>0&&j==0&&i!=4 || (i>0&&j==4&&i!=4) || (i==0&&j<5&&j!=4&&j!=0 )|| (i==4&&j<5&&j!=4&&j!=0 )||(i==4-j&&i!=0&&i!=4)) {
							letra[i][j]=SYMB;	
						}
					}
				}
				transferirMatriz();	
			break;
		}
	}
	for(i = 0; i<5; i++){
		printf("\t\t    ");
		for(j=0;j<100;j++){
			printf("%c", palavra[i][j]);
		}
		printf("\n");
	}
	printf("\n");
}

typedef struct{         //ENDEREÇOS
    char Rua[50];
    char Complemento[20];
    char Bairro[50];
    char Cidade[50];
    char Estado[20];
    char CEP[20];
}Endereco;

typedef struct{         //ALUNOS
    Endereco endereco;
    char Nome[50];
    char Sobrenome[50];
    char CPF_A[20];
    char Celular[20];
    char Email[50];
    char DataNas[10];
	int ID_Aluno;
    int A_ativo; 
}Aluno;

typedef struct{         //PROFESSORES
    Endereco endereco;
    char Nome[50];
    char Sobrenome[50];
    char Celular[20];
    char Email[50];
    char Carga_horaria[10];
    char CPF_P[20];
	int ID_Professor;
    int P_ativo; 
}Professor;

typedef struct{         //CURSOS
    char Nome_curso[50];
    char Aulas[50];
    char carga_h[10];
    char valor[10];
    int ID_Curso;
    int C_ativo;  
}Cursos;

typedef struct{         //TURMAS
    char Nome[20];
    char Aulas[50];
    char carga_horaria[15];
	int ID_Turma;
    int T_ativo;  
}Turmas;

typedef struct{			//MATRICULAS
	int ID_Curso;
	int ID_Aluno;
	char DataMat[10];
	int M_ativo;
	int ID_Mat;
}Matriculas;

void listar(char s[20]){
	/*Função para universal para listar, nela em especifico a função percorre a lista 2 vezes, a primeira para contabilizar quantos itens 
	  existem e passando esse numero como parametro na função "Texto", assim exibindo a quantidade exata no texto em grande escala,
	  a segunda vez que percorre a lista é para justamente exibir os itens na lista.
	*/
	if(strcmp(s,"alunos.bin")==0){
		Aluno alunos;					
		int qnt = 0;
    	FILE *A = fopen(s, "rb");
    	fpos_t Byte = 0;
		system("cls");
        if(A == NULL){
            printf("\n\nErro ao Abrir o arquivo!\n\n");
            system("pause");
            exit(1);
        }else{
			while(fread(&alunos, sizeof(Aluno), 1, A)){
				qnt+=1;
			}
        	Texto("lista ", qnt);
			fsetpos(A, &Byte);
        	while(fread(&alunos, sizeof(Aluno), 1, A)){
            	printf("Nome ....: %s %s\n", alunos.Nome, alunos.Sobrenome);
            	printf("CPF .....: %s\n", alunos.CPF_A);
            	printf("ID ......: %d\n", alunos.ID_Aluno);
            	printf("\n-------------------\n\n");
            }fclose(A);
		}getchar();
    }
	if(strcmp(s,"cursos.bin")==0){
		int qnt = 0;									
    	Cursos cur;												
		fpos_t Byte = 0;											
    	FILE *C = fopen(s, "rb");
        if(C == NULL){
            printf("\n\nErro ao Abrir o arquivo!\n\n");
        	system("pause");
            exit(1);
        }else{
			while(fread(&cur, sizeof(Cursos), 1, C)){
				qnt +=1;
			}
            system("cls");
			fsetpos(C, &Byte);
        	Texto("lista ",qnt);
        	while(fread(&cur, sizeof(Cursos), 1, C)){
            	printf("Nome .........: %s \n", cur.Nome_curso);
            	printf("Valor ........: %s\n", cur.valor);
            	printf("ID ...........: %d\n", cur.ID_Curso);
            	printf("\n-------------------\n\n");
       		}fclose(C);
    	}getchar();
	}
	if(strcmp(s,"professores.bin")==0){
		int qnt =0;									
	    Professor prof;								
		fpos_t Byte =0;								
    	FILE *B = fopen(s, "rb");
        if(B == NULL){
            printf("\n\nErro ao Abrir o arquivo!\n\n");
            system("pause");
            exit(1);
        }else{
            system("cls");
			while(fread(&prof, sizeof(Professor), 1, B)){
				qnt +=1;
			}
        	Texto("lista ", qnt);
			fsetpos(B, &Byte);
        	while(fread(&prof, sizeof(Professor), 1, B)){
            	printf("Nome .........: %s %s\n", prof.Nome, prof.Sobrenome);
            	printf("CPF ..........: %s\n", prof.CPF_P);
            	printf("ID ...........: %d\n", prof.ID_Professor);
            	printf("\n-------------------\n\n");
        	}fclose(B);
    	}getchar();
	}
	if(strcmp(s,"turmas.bin")==0){
		Turmas turma;											
		int qnt =0;													
		fpos_t Byte =0;												
	    FILE *D= fopen(s, "rb");
	    if(D == NULL){
	        printf("\n\nErro ao Abrir o arquivo!\n\n");
	        system("pause");
	        exit(1);
	    }else{
	        system("cls");
			while(fread(&turma, sizeof(Turmas), 1, D)){
				qnt+=1;
			}
	        Texto("lista ",qnt);
			fsetpos(D, &Byte);
	        while(fread(&turma, sizeof(Turmas), 1, D)){
	            printf("Nome .........: %s \n", turma.Nome);
	            printf("Carga Horaria : %s\n", turma.carga_horaria);
	            printf("ID ...........: %d\n", turma.ID_Turma);
	            printf("\n-------------------\n\n");
			}
	        fclose(D);
	    }getchar();
	}
	if(strcmp(s,"matriculas.bin")==0){
		Matriculas mat;												
		int qnt =0;													
		fpos_t Byte =0;
	    FILE *A = fopen(s, "rb");
	    if(A == NULL){
	        printf("\n\nErro ao Abrir o arquivo!\n\n");
	        system("pause");
	        exit(1);
	    }else{
	        system("cls");
			while(fread(&mat, sizeof(Matriculas), 1, A)){
				qnt +=1;
			}
	        Texto("lista ",qnt);
			fsetpos(A, &Byte);
	        while(fread(&mat, sizeof(Matriculas), 1, A)){
					printf("\n\n ---------- Lista de Matriculas ----------\n\n");
	            	printf("ID CURSO .......: %d\n", mat.ID_Curso);
	            	printf("ID ALUNO .......: %d\n", mat.ID_Aluno);
	            	printf("ID MATRICULA ...: %d\n", mat.ID_Mat);
	            	printf("DATA MATRICULA .: %s\n", mat.DataMat);
	            	printf("\n-------------------\n\n");
			}
			fclose(A);
	    }getchar();
	}
}

void listar_alunosmat(char s[12]){			
	/*Função para listar todos os alunos, nela em especifico a função percorre a lista 2 vezes, a primeira para contabilizar quantos alunos 
	  existem e passando esse numero como parametro na função "Texto", assim exibindo o numero exato de alunos no texto em grande escala,
	  a segunda vez que percorre a lista é para justamente exibir os alunos na lista.
      devido a um bug na hora de exibir a lista na matricula tivemos que refazer a função adaptando-a para o caso da matricula.
    */
	Aluno alunos;							
    int i = 0;
	int qnt = 0;
	fpos_t Byte = 0;
    FILE *A = fopen(s, "rb");
    if(A == NULL){
        printf("\n\nErro ao Abrir o arquivo!\n\n");
        system("pause");
        exit(1);
    }else{
        while(fread(&alunos, sizeof(Aluno), 1, A)){
			qnt+=1;
		}
		system("cls");
    	Texto("lista ", qnt);
		fsetpos(A, &Byte);
    	while(fread(&alunos, sizeof(Aluno), 1, A)){
        	printf("Nome ....: %s %s\n", alunos.Nome, alunos.Sobrenome);
        	printf("CPF .....: %s\n", alunos.CPF_A);
        	printf("ID ......: %d\n", alunos.ID_Aluno);
        	printf("\n-------------------\n\n");
		}
		fclose(A);
	}
}

void excluir(char s[20]){					
	//Função universal para exclusão fisica dos arquivos, basta passar nos parametros qual arquivo você quer que seja feita a exclusão fisica.
	FILE *A = fopen("temp.bin", "ab+");
	if (A==NULL){
		printf("\\nErro ao Abrir o arquivo!");
        system("pause");
        exit(1);
	}else{
		if(strcmp(s,"alunos.bin")==0){
			Aluno alunos;
			FILE *B =fopen(s, "rb+");
   			while(fread(&alunos, sizeof(Aluno), 1, B)){
            	if(alunos.A_ativo==1){
            		fwrite(&alunos, sizeof(Aluno), 1, A);
				}
    		}
			fclose(B);
			fclose(A);
			struct  midia;
        	FILE *C = fopen(s, "w");
        	fclose(C);
        	FILE *D =fopen("temp.bin", "rb+");
			FILE *E =fopen(s, "ab+");
   			while(fread(&alunos, sizeof(Aluno), 1, D)){
            	fwrite(&alunos, sizeof(Aluno), 1, E);
    		}
			fclose(D);
			fclose(E);
        	struct  midia;
        	FILE *F = fopen("temp.bin", "w");
        	fclose(F);
		}
		if(strcmp(s,"cursos.bin")==0){
			Cursos curso;
			FILE *B =fopen(s, "rb+");
   			while(fread(&curso, sizeof(Cursos), 1, B)){
            	if(curso.C_ativo==1){
            		fwrite(&curso, sizeof(Cursos), 1, A);
				}
    		}
			fclose(B);
			fclose(A);
			struct  midia;
        	FILE *C = fopen(s, "w");
        	fclose(C);
        	FILE *D =fopen("temp.bin", "rb+");
			FILE *E =fopen(s, "ab+");
   			while(fread(&curso, sizeof(Cursos), 1, D)){
            	fwrite(&curso, sizeof(Cursos), 1, E);
    		}
			fclose(D);
			fclose(E);
        	struct  midia;
        	FILE *F = fopen("temp.bin", "w");
        	fclose(F);
		}
		if(strcmp(s,"professores.bin")==0){
			Professor prof;
			FILE *B =fopen(s, "rb+");
   			while(fread(&prof, sizeof(Professor), 1, B)){
            	if(prof.P_ativo==1){
            		fwrite(&prof, sizeof(Professor), 1, A);
				}
    		}
			fclose(B);
			fclose(A);
			struct  midia;
        	FILE *C = fopen(s, "w");
        	fclose(C);
        	FILE *D =fopen("temp.bin", "rb+");
			FILE *E =fopen(s, "ab+");
   			while(fread(&prof, sizeof(Professor), 1, D)){
            	fwrite(&prof, sizeof(Professor), 1, E);
    		}
			fclose(D);
			fclose(E);
        	struct  midia;
        	FILE *F = fopen("temp.bin", "w");
        	fclose(F);
		}
		if(strcmp(s,"turmas.bin")==0){
			Turmas turma;
			FILE *B =fopen(s, "rb+");
   			while(fread(&turma, sizeof(Turmas), 1, B)){
            	if(turma.T_ativo==1){
            		fwrite(&turma, sizeof(Turmas), 1, A);
				}
    		}
			fclose(B);
			fclose(A);
			struct  midia;
        	FILE *C = fopen(s, "w");
        	fclose(C);
        	FILE *D =fopen("temp.bin", "rb+");
			FILE *E =fopen(s, "ab+");
   			while(fread(&turma, sizeof(Turmas), 1, D)){
            	fwrite(&turma, sizeof(Turmas), 1, E);
    		}
			fclose(D);
			fclose(E);
        	struct  midia;
        	FILE *F = fopen("temp.bin", "w");
        	fclose(F);
		}
		if(strcmp(s,"matriculas.bin")==0){
			Matriculas mat;
			FILE *B =fopen(s, "rb+");
   			while(fread(&mat, sizeof(Matriculas), 1, B)){
            	if(mat.M_ativo==1){
            		fwrite(&mat, sizeof(Matriculas), 1, A);
				}
    		}
			fclose(B);
			fclose(A);
			struct  midia;
        	FILE *C = fopen(s, "w");
        	fclose(C);
        	FILE *D =fopen("temp.bin", "rb+");
			FILE *E =fopen(s, "ab+");
   			while(fread(&mat, sizeof(Matriculas), 1, D)){
            	fwrite(&mat, sizeof(Matriculas), 1, E);
    		}
			fclose(D);
			fclose(E);
        	struct  midia;
        	FILE *F = fopen("temp.bin", "w");
        	fclose(F);
		}
	}
}

void dados(char s[20], char Procurado[40]){
	//Função universal para exibir dados do item informado no parametro.
	if(strcmp(s,"alunos.bin")==0){
    	Aluno alunos;
    	fpos_t Byte;
    	FILE *A = fopen(s, "rb");
    	Byte = consultar(s, Procurado);
        if(A == NULL){
            printf("\n\nErro ao Abrir o arquivo!\n\n");
            system("pause");
            exit(1);
        }else{
            if (Byte != -1){
        	    system("cls");
        		Texto("dados   ", -1);
				while(fread(&alunos, sizeof(Aluno),1, A)){
					if(strcmp(Procurado, alunos.Nome)==0){
		            	printf("Nome .........: %s\n", alunos.Nome);
		            	printf("Sobrenome ....: %s\n", alunos.Sobrenome);
		            	printf("Celular ......: %s\n", alunos.Celular);
		            	printf("E-mail .......: %s\n", alunos.Email);
		            	printf("CPF ..........: %s\n", alunos.CPF_A);
		            	printf("Data Nas .....: %s\n", alunos.DataNas);
		            	printf("Rua ..........: %s\n", alunos.endereco.Rua);
		            	printf("Complemento ..: %s\n",alunos.endereco.Complemento);
		            	printf("Bairro........: %s\n", alunos.endereco.Bairro);
		            	printf("Cidade .......: %s\n",alunos.endereco.Cidade);
		            	printf("Estado .......: %s\n", alunos.endereco.Estado);
		            	printf("CEP ..........: %s\n", alunos.endereco.CEP);
		            	printf("ID ...........: %d\n", alunos.ID_Aluno);
		        		printf("\n-------------------\n\n");
    				}
                }
            }
        }
	}
	if(strcmp(s,"cursos.bin")==0){
		Cursos cur;
    	fpos_t Byte;
    	FILE *C = fopen(s, "rb");
    	Byte = consultar(s,Procurado);
        if(C == NULL){
            printf("\n\nErro ao Abrir o arquivo!\n\n");
            system("pause");
            exit(1);
        }else{
            system("cls");
        	Texto("dados   ",-1);
        	while(fread(&cur, sizeof(Cursos), 1, C)){
				if(strcmp(Procurado, cur.Nome_curso)==0){
		            printf("Nome .........: %s\n", cur.Nome_curso);
		            printf("Valor ........: %s\n", cur.valor);
		            printf("Carga Horaria : %s\n", cur.carga_h);
		            printf("Aulas ........: %s\n", cur.Aulas);
			        printf("\n-------------------\n\n");
        			getchar();
            	}
        	}
    	}
	}
	if(strcmp(s,"professores.bin")==0){
	    Professor prof;
	    fpos_t Byte;
	    FILE *B = fopen(s, "rb");
	    Byte = consultar(s,Procurado);
        if(B == NULL){
            printf("\n\nErro ao Abrir o arquivo!\n\n");
            system("pause");
            exit(1);
        }else{
            system("cls");
        	Texto("dados   ",-1);
        	while(fread(&prof, sizeof(Professor), 1, B)){
				if(strcmp(Procurado, prof.Nome)==0){
		            printf("Nome .........: %s\n", prof.Nome);
		            printf("Sobrenome ....: %s\n", prof.Sobrenome);
		            printf("Celular ......: %s\n", prof.Celular);
		            printf("E-mail .......: %s\n", prof.Email);
		            printf("CPF ..........: %s\n", prof.CPF_P);
		            printf("Carga H ......: %s\n", prof.Carga_horaria);
		
		            printf("Rua ..........: %s\n", prof.endereco.Rua);
		            printf("Complemento ..: %s\n", prof.endereco.Complemento);
		            printf("Bairro........: %s\n", prof.endereco.Bairro);
		            printf("Cidade .......: %s\n", prof.endereco.Cidade);
		            printf("Estado .......: %s\n", prof.endereco.Estado);
		            printf("CEP ..........: %s\n", prof.endereco.CEP);
		        	printf("\n-------------------\n\n");
		        	getchar();
            	}
        	}
    	}
	}
	if(strcmp(s,"turmas.bin")==0){
		Turmas turma;
	    fpos_t Byte;
	    FILE *D= fopen(s, "rb");
	    Byte = consultar(s, Procurado);
        if(D == NULL){
            printf("\n\nErro ao Abrir o arquivo!\n\n");
            system("pause");
            exit(1);
        }else{
            system("cls");
        	Texto("dados   ",-1);
        	while(fread(&turma, sizeof(Turmas), 1, D)){
				if(strcmp(Procurado, turma.Nome)==0){
		            printf("Nome ..........: %s\n", turma.Nome);
		            printf("Aulas .........: %s\n", turma.Aulas);
		            printf("Carga Horaria .: %s\n", turma.carga_horaria);
		            printf("ID ............: %d\n", turma.ID_Turma);
		            printf("\n-------------------\n\n");
            	}
        	}
    	}
	}
}

void cadastrar(char s[20]){
	//Função universal de cadastro de item, relativo ao arquivo informado no parametro.
	if(strcmp(s,"alunos.bin")==0){
		Aluno alunos;
        int op, i=0;
        do{ 
			system("cls");
        	Texto("cadastro", -1);
        	printf("\n----- Informações do aluno ------\n\n\n");
            getchar();
            printf("Nome .......:");
            gets(alunos.Nome);
            printf("Sobrenome ..:");
            gets(alunos.Sobrenome);
            printf("Celular ....:");
            gets(alunos.Celular);
            printf("E-mail .....:");
            gets(alunos.Email);
            printf("CPF ........:");
            gets(alunos.CPF_A);
            printf("Data Nas ...:");
            gets(alunos.DataNas);
            printf("\n----- Endereço do aluno ------\n\n");
            printf("Rua, N° ....:");
            gets(alunos.endereco.Rua);
            printf("Complemento :");
            gets(alunos.endereco.Complemento);
            printf("Bairro .....:");
            gets(alunos.endereco.Bairro);
            printf("Cidade .....:");
            gets(alunos.endereco.Cidade);
            printf("Estado .....:");
            gets(alunos.endereco.Estado);
            printf("CEP ........:");
            gets(alunos.endereco.CEP);
			alunos.A_ativo=1;
			alunos.ID_Aluno = defineID(s);
            FILE *A = fopen(s, "ab+");
            if(A == NULL){
                printf("\\nErro ao Abrir o arquivo!");
                system("pause");
                exit(1);
            }else{
            	fwrite(&alunos, sizeof(Aluno), 1, A);
			}
            fclose(A);
            system("cls");
            printf("\n----- Aluno cadastrado com Sucesso ------\n\n\n");
            printf("\n1 - Começar um novo cadastro?\n0 - Voltar\n\nR:");
            scanf("%d",&op);
        }while(op!=0);
	}
	if(strcmp(s,"cursos.bin")==0){
		Cursos cur;
        int op, i=0;
        do{ 
			system("cls");
        	Texto("cadastro",-1);
        	printf("\n----- Informações do Curso ------\n\n\n");
            getchar();
            printf("Nome .......:");
            gets(cur.Nome_curso);
            printf("Valor ......:");
            gets(cur.valor);
            printf("Carga Horaria ..:");
            gets(cur.carga_h);
            printf("Aulas ......:");
            gets(cur.Aulas);
			cur.C_ativo=1;
			cur.ID_Curso= defineID(s);
            FILE *C =fopen(s, "ab+");
            if(C ==NULL){
                printf("\nErro ao Abrir ou Criar o arquivo!");
                system("pause");
            	exit(1);
            }else{
				fwrite(&cur, sizeof(Cursos), 1, C);
			}
            fclose(C);
        	system("cls");
            printf("\n----- Curso cadastrado com Sucesso ------\n\n\n");
            printf("\n1 - Começar um novo cadastro?\n0 - Voltar\n\nR:");
            scanf("%d",&op);
        }while(op!=0);
	}
	if(strcmp(s,"professores.bin")==0){
    	Professor prof;
        int op, i=0;
        do{ 
			system("cls");
        	Texto("cadastro",-1);
        	printf("\n----- Informações do Professor ------\n\n\n");
            getchar();
            printf("Nome .......:");
            gets(prof.Nome);
            printf("Sobrenome ..:");
            gets(prof.Sobrenome);
            printf("Celular ....:");
            gets(prof.Celular);
            printf("E-mail .....:");
            gets(prof.Email);
            printf("Custo Carga H .:");
            gets(prof.Carga_horaria);
            printf("CPF ........:");
            gets(prof.CPF_P);
            printf("\n----- Endereço do aluno ------\n\n");
            printf("Rua, N° ....:");
            gets(prof.endereco.Rua);
            printf("Complemento :");
            gets(prof.endereco.Complemento);
            printf("Bairro .....:");
            gets(prof.endereco.Bairro);
            printf("Cidade .....:");
            gets(prof.endereco.Cidade);
            printf("Estado .....:");
            gets(prof.endereco.Estado);
            printf("CEP ........:");
            gets(prof.endereco.CEP);
            prof.P_ativo=1;
            prof.ID_Professor= defineID(s);
            FILE *B =fopen(s, "ab+");
            if(B ==NULL){
                printf("\nErro ao Abrir ou Criar o arquivo!");
                system("pause");
                exit(1);
            }else{
            	fwrite(&prof, sizeof(Professor), 1, B);
			}
            fclose(B);
            system("cls");
            printf("\n----- Professor cadastrado com Sucesso ------\n\n\n");
            printf("\n1 - Começar um novo cadastro?\n0 - Voltar\n\nR:");
            scanf("%d",&op);
        }while(op!=0);
	}
	if(strcmp(s,"turmas.bin")==0){
		Turmas turma;
        int op, i=0;
        do{ 
			system("cls");
         	Texto("cadastro",-1);
        	printf("\n----- Informações da Turma------\n\n\n");
            getchar();
            printf("Nome .......:");
            gets(turma.Nome);
            printf("Aulas ......:");
            gets(turma.Aulas);
            printf("Carga Horaria ..:");
            gets(turma.carga_horaria);
			turma.T_ativo=1;
			turma.ID_Turma= defineID(s);
            FILE *D =fopen(s, "ab+");
            if(D ==NULL){
	            printf("\nErro ao Abrir ou Criar o arquivo!");
	            system("pause");
	            exit(1);
            }else{
            	fwrite(&turma, sizeof(Turmas), 1, D);
			}
            fclose(D);
            system("cls");
            printf("\n----- Turma cadastrada com Sucesso ------\n\n\n");
            printf("\n1 - Começar um novo cadastro?\n0 - Voltar\n\nR:");
            scanf("%d",&op);
        }while(op!=0);
	}
	if(strcmp(s,"matriculas.bin")==0){
		Matriculas mat;
		Aluno alunos;
		Cursos cur;
		char r[15]="cursos.bin";
		char a[15] = "alunos.bin";
		char curso[50], Aprocurado[50];
		int op;
		int i= 0;
		do{ 
			system("cls");
        	Texto("cadastro",-1);
			printf("Cursos: ");
			listar(r);
			printf("Digite o curso escolhido: ");
			gets(curso);
			fpos_t Byte;
	    	FILE *C = fopen(r, "rb+");
   			Byte = consultar(r, curso);
   			fsetpos(C, &Byte);
        	if(C == NULL){
                printf("\n\nErro ao Abrir o arquivo!\n\n");
                system("pause");
                exit(1);
            }else{
            	system("cls");
            	fread(&cur, sizeof(Cursos), 1, C);
            	mat.ID_Curso = cur.ID_Curso;
				fclose(C);
            	printf("\n\n\t----- Curso selecionado! -----\n\n");
        		getchar();
        	}
			system("cls");
			listar_alunosmat(a);
			printf("Selecione o aluno a ser matriculado: ");
			gets(Aprocurado);		
		    FILE *A = fopen(a, "rb+");
		    Byte = consultar(a, Aprocurado);
			fsetpos(A, &Byte);
	        if(A == NULL){
                printf("\n\nErro ao Abrir o arquivo!\n\n");
                system("pause");
                exit(1);
            }else{
            	if (Byte != -1){
            	system("cls");
            	fread(&alunos, sizeof(Aluno), 1, A);
            	mat.ID_Aluno = alunos.ID_Aluno;
				fclose(A);
            	}
            printf("\n\n\t----- Aluno selecionado! -----\n\n");
        	getchar(); 
        	}
    		system("cls");
			printf("Digite a data da matricula: ");
			gets(mat.DataMat);
			mat.M_ativo=1;
			mat.ID_Mat = defineID(s);
            FILE *M = fopen(s, "ab+");
            if(M == NULL){
                printf("\\nErro ao Abrir o arquivo!");
                system("pause");
                exit(1);
            }else{
            	fwrite(&mat, sizeof(Matriculas), 1, M);
			}
            fclose(M);
			system("cls");
            printf("\n----- Matricula registrada com Sucesso ------\n\n\n");
            printf("\n1 - Começar um novo cadastro?\n0 - Voltar\n\nR:");
            scanf("%d",&op);
		}while(op!=0);
	}
}

void remover(char s[20], char Procurado[40]){
	//Função universal de remoção de item informado no parametro.
	if(strcmp(s,"alunos.bin")==0){
	    Aluno alunos;
	    fpos_t Byte;
	    FILE *A= fopen(s, "rb+");
	    Byte = consultar(s,Procurado);
	    if (Byte != -1){
			fflush(stdin);
			alunos.A_ativo=0;
	        fsetpos(A, &Byte);
	        fwrite(&alunos, sizeof(Aluno), 1, A);
	        fclose(A);
			excluir(s);
	        printf("\n\nAluno removido com Sucesso!!\n");
	        getchar();
	    }else{
	    	printf("Aluno não encontrado");
	    	fclose(A);
	    	getchar();
		}
	}
	if(strcmp(s,"cursos.bin")==0){
		Cursos cur;
    	fpos_t Byte;
    	FILE *C= fopen(s, "rb+");
    	Byte = consultar(s, Procurado);
     	if (Byte != -1){
			fflush(stdin);
			cur.C_ativo=0;
            fsetpos(C, &Byte);
            fwrite(&cur, sizeof(Cursos), 1, C);
            fclose(C);
			excluir(s);
            printf("\n\nCurso removido com Sucesso!!\n");
        }else{
        	printf("Curso não encontrado");
        	fclose(C);
        	getchar();
		}
	}
	if(strcmp(s,"professores.bin")==0){
    	Professor prof;
    	fpos_t Byte;
    	FILE *B= fopen(s, "rb+");
    	Byte = consultar(s,Procurado);
    	if (Byte != -1){
			fflush(stdin);
			prof.P_ativo=0;
            fsetpos(B, &Byte);
            fwrite(&prof, sizeof(Professor), 1, B);
            fclose(B);
			excluir(s);
            printf("\n\nProfessor removido com Sucesso!!\n");
            getchar();
        }else{
        	printf("Aluno não encontrado");
        	fclose(B);
        	getchar();
		}
	}
	if(strcmp(s,"turmas.bin")==0){
		Turmas turma;	
    	fpos_t Byte;
    	FILE *D= fopen(s, "rb+");
    	Byte = consultar(s,Procurado);
     	if (Byte != -1){
			fflush(stdin);
			turma.T_ativo=0;
            fsetpos(D, &Byte);
            fwrite(&turma, sizeof(Turmas), 1, D);
			fclose(D);
			excluir(s);
            printf("\n\nTurma removida com Sucesso!!\n");
            getchar();
        }else{
        	printf("Turma não encontrado");
        	getchar();
		}
	}
}

void removermat(int ID, char s[16]){						
	/*Função de remover a matricula logicamente para depois chamar a função de remoção fisica da matricula, 
	  passando nos parametros o ID da matricula e o nome do arquivo.	
	*/
    Matriculas mat;												
    fpos_t Byte;
    FILE *A= fopen(s, "rb+");
    Byte = consultarID(s, ID);
    if (Byte != -1){
		fflush(stdin);
		mat.M_ativo=0;
        fsetpos(A, &Byte);
        fwrite(&mat, sizeof(Matriculas), 1, A);
		fclose(A);
		excluir(s);
        printf("\n\nMatricula removido com Sucesso!!\n");
		getchar();
    }else{
        printf("Matricula não encontrado");
        fclose(A);
        getchar();
	}
}

int consultar(char s[20], char Procurado[40]){
	//Função universal de consulta de Byte atraves do item informado no parametro.
	if(strcmp(s,"alunos.bin")==0){	
    	FILE *A = fopen(s, "rb+");
    	Aluno alunos;
	    fpos_t byte;
    	int tam= sizeof(alunos);
    	do{
        	fread(&alunos, sizeof(Aluno), 1, A);
            if(strcmp(Procurado, alunos.Nome)==0){
                byte = ftell(A)-tam;
                fclose(A);
                return(byte);}

    	}while(eof(A));
		fclose(A);
		return(-1);
	}
	if(strcmp(s,"cursos.bin")==0){	
    	FILE *C= fopen(s, "rb+");
    	Cursos cur;
    	fpos_t byte;
    	int tam= sizeof(cur);
    	do{
        	fread(&cur, sizeof(Cursos), 1, C);
            if(strcmp(Procurado, cur.Nome_curso)==0){
                byte = ftell(C)-tam;
                fclose(C);
                return(byte);}
    	}while(eof(C));
		fclose(C);
		return(-1);
	}
	if(strcmp(s,"professores.bin")==0){
		FILE *B = fopen(s, "rb+");
    	Professor prof;
    	fpos_t byte;
    	int tam= sizeof(prof);
	    do{
	        fread(&prof, sizeof(Professor), 1, B);
	        if(strcmp(Procurado, prof.Nome)==0){
	            byte = ftell(B)-tam;
	            fclose(B);
	            getchar();
	            return(byte);
			}
	    }while(eof(B));
		fclose(B);
		return(-1);
	}
	if(strcmp(s,"turmas.bin")==0){
    	FILE *D = fopen(s, "rb+");
    	Turmas turma;
    	fpos_t byte;
    	int tam= sizeof(turma);
    	do{
        	fread(&turma, sizeof(Turmas), 1, D);
            if(strcmp(Procurado, turma.Nome)==0){
                byte = ftell(D)-tam;
                fclose(D);
                return(byte);}
    	}while(eof(D));
		fclose(D);
		return(-1);
	}
	if(strcmp(s,"matriculas.bin")==0){
		Matriculas mat;
		Aluno alunos;
		Cursos cur;
		char r[15]="cursos.bin";
		char a[15] = "alunos.bin";
		char curso[50], Aprocurado[50];
		int op;
		int i= 0;
	 	do{ 
			system("cls");
        	Texto("cadastro",-1);
			printf("Cursos: ");
			listar(r);
			printf("Digite o curso escolhido: ");
			gets(curso);
			fpos_t Byte;
	    	FILE *C = fopen(r, "rb+");
   			Byte = consultar(r, curso);
   			fsetpos(C, &Byte);
        	if(C == NULL){
                printf("\n\nErro ao Abrir o arquivo!\n\n");
                system("pause");
                exit(1);
            }else{
            	system("cls");
            	fread(&cur, sizeof(Cursos), 1, C);
            	mat.ID_Curso = cur.ID_Curso;
				fclose(C);
            	printf("\n\n\t----- Curso selecionado! -----\n\n");
        		getchar();
        	}
			system("cls");
			listar_alunosmat(a);
			printf("Selecione o aluno a ser matriculado: ");
			gets(Aprocurado);
		    FILE *A = fopen(a, "rb+");
		    Byte = consultar(a, Aprocurado);
			fsetpos(A, &Byte);
        	if(A == NULL){
                printf("\n\nErro ao Abrir o arquivo!\n\n");
                system("pause");
                exit(1);
            }else{
            	if (Byte != -1){
		            system("cls");
		            fread(&alunos, sizeof(Aluno), 1, A);
		            mat.ID_Aluno = alunos.ID_Aluno;
					fclose(A);
            	}
        	printf("\n\n\t----- Aluno selecionado! -----\n\n");
        	getchar(); 
        	}
    		system("cls");
			printf("Digite a data da matricula: ");
			gets(mat.DataMat);
			mat.M_ativo=1;
			mat.ID_Mat = defineID(s);
            FILE *M = fopen(s, "ab+");
            if(M == NULL){
                printf("\\nErro ao Abrir o arquivo!");
                system("pause");
                exit(1);
            }else{
            	fwrite(&mat, sizeof(Matriculas), 1, M);
			}
            fclose(M);
            system("cls");
            printf("\n----- Matricula registrada com Sucesso ------\n\n\n");
            printf("\n1 - Começar um novo cadastro?\n0 - Voltar\n\nR:");
            scanf("%d",&op);
		}while(op!=0);
	}
}

int consultarID(char s[20], int ID){
	//Função universal de consulta de Byte atraves do ID informado.
	if(strcmp(s,"alunos.bin")==0){
		FILE *A = fopen(s, "rb+");
		Aluno alunos;
    	fpos_t byte;
    	int tam= sizeof(alunos);
    	do{
        	fread(&alunos, sizeof(Aluno), 1, A);
            if(ID== alunos.ID_Aluno){
            	byte = ftell(A)-tam;
                fclose(A);
                return(byte);
			}
    	}while(eof(A));
		fclose(A);
		return(-1);
	}
	if(strcmp(s,"cursos.bin")==0){
    	FILE *C= fopen(s, "rb+");
    	Cursos cur;
    	fpos_t byte;
    	int tam= sizeof(cur);
    	do{
        	fread(&cur, sizeof(Cursos), 1, C);
            if(ID== cur.ID_Curso){
                byte = ftell(C)-tam;
                fclose(C);
                return(byte);
			}
    	}while(eof(C));
		fclose(C);
		return(-1);
	}
	if(strcmp(s,"matriculas.bin")==0){
		FILE *D = fopen(s, "rb+");		
	    Matriculas mat;
    	fpos_t byte;
    	int tam= sizeof(mat);
    	do{
        	fread(&mat, sizeof(Matriculas), 1, D);
            if(ID== mat.ID_Mat){
                byte = ftell(D)-tam;
                fclose(D);
                return(byte);
			}
    	}while(eof(D));
		fclose(D);
		return(-1);
	}
}

void alterar(char s[20], char Procurado[40]){
	/*Função universal para alterar as informações registradas com base no arquivo informado no paramentro + o item a ser alterado,
	  tambem informado no paramentro.
	*/
	char d;
	if(strcmp(s,"alunos.bin")==0){
		int op;									
		Aluno alunos;
    	fpos_t Byte;
    	FILE *A= fopen(s, "rb+");
    	Byte = consultar(s,Procurado);
     	if (Byte != -1){
        	do{
            	system("cls");
		        printf("\n---------- Dados a serem alterados -----------\n\n");
		        printf("\n1 - Nome \n2 - Sobrenome \n3 - Celular");
		        printf("\n4 - E-mail \n5 - CPF \n6 - Data Nas ");
		        printf("\n7 - Rua/Nº \n8 - Complemento \n9 - Bairro");
		        printf("\n10 - Cidade \n11 - Estado \n12 - CEP");
		        printf("\n0 - Voltar \n\n---------> Escolha uma opção: ");
		        scanf("%d",&op);
		        getchar();
	            switch(op){
	                case 1:
	                    if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nNome Atual: %s \nDeseja Alterar(S/N)?", alunos.Nome);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Nome:");
	                            fflush(stdin); gets(alunos.Nome);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nNome alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                	break;
	                case 2:
	                     if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nSobrenome Atual: %s \nDeseja Alterar(S/N)?", alunos.Sobrenome);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Sobrenome:");
	                            fflush(stdin); gets(alunos.Sobrenome);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\nSobrenome alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                	break;
	                case 3:
	                    if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nCelular Atual: %s \nDeseja Alterar(S/N)?", alunos.Celular);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Nome:");
	                            fflush(stdin); gets(alunos.Celular);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nCelular alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                    break;
	                case 4:
	                     if (Byte != -1) {
	                        fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nE-mail Atual: %s \nDeseja Alterar(S/N)?", alunos.Email);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo E-mail:");
	                            fflush(stdin); gets(alunos.Email);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nE-mail alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                	break;
	                case 5:
	                    if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nCPF: %s \nDeseja Alterar(S/N)?", alunos.CPF_A);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo CPF:");
	                            fflush(stdin); gets(alunos.CPF_A);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nCPF alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                	break;
	            	case 6:
	                     if (Byte != -1) {
	                            fsetpos(A, &Byte);
	                            fread (&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nData nascimento Atual: %s \nDeseja Alterar(S/N)?", alunos.DataNas);
	                            fflush(stdin); scanf("%c", &d);
	                        	if(toupper(d) == 'S'){
		                            printf("\n\nDigite o nova Data Nas:");
		                            fflush(stdin); gets(alunos.DataNas);
		                            fsetpos(A, &Byte);
		                            fwrite(&alunos, sizeof(Aluno), 1, A);
		
		                            printf("\n\nData nascimento alterada com Sucesso!!\n");
		                            getchar();
	                    		}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	            		break;
	            	case 7:
	                    if (Byte != -1) {
	                        fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nRua e Nº Atuais: %s \nDeseja Alterar(S/N)?", alunos.endereco.Rua);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite a Nova Rua e Nº:");
	                            fflush(stdin); gets(alunos.endereco.Rua);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nRua e Nº alterados com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                    break;
	                case 8:
	                     if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nComplemento Atual: %s \nDeseja Alterar(S/N)?", alunos.endereco.Complemento);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Complemnto:");
	                            fflush(stdin); gets(alunos.endereco.Complemento);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\nComplemento alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                	break;
	                case 9:
	                    if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\nBairro Atual: %s \nDeseja Alterar(S/N)?", alunos.endereco.Bairro);
                            fflush(stdin); scanf("%c", &d);
	                    	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Bairro:");
	                            fflush(stdin); gets(alunos.endereco.Bairro);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\nBairro alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                    break;
	                case 10:
	                     if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nCidade Atual: %s \nDeseja Alterar(S/N)?", alunos.endereco.Cidade);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Cidade:");
	                            fflush(stdin); gets(alunos.endereco.Cidade);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nCidade alterado com Sucesso!!\n");
	                            getchar();
	                    	}
						}else{
	                		printf("Registo não encontrado");
	            		}
	                	break;
	                case 11:
	                    if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nEstado Atual: %s \nDeseja Alterar(S/N)?", alunos.endereco.Estado);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Estado:");
	                            fflush(stdin); gets(alunos.endereco.Estado);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nEstado alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                	break;
	            	case 12:
	                     if (Byte != -1) {
                            fsetpos(A, &Byte);
                            fread (&alunos, sizeof(Aluno), 1, A);
                            printf("\n\nCEP Atual: %s \nDeseja Alterar(S/N)?", alunos.endereco.CEP);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o nova CEP:");
	                            fflush(stdin); gets(alunos.endereco.CEP);
	                            fsetpos(A, &Byte);
	                            fwrite(&alunos, sizeof(Aluno), 1, A);
	                            printf("\n\nCEP alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	            		}
	                	break;
	            }
	        }while(op != 0);
	    }else{
	        printf("Registo não encontrado");
	        getchar();
	    }fclose(A);
	}
	if(strcmp(s,"cursos.bin")==0){
		int op;						
    	Cursos cur;
    	fpos_t Byte;
    	FILE *C= fopen(s, "rb+");
    	Byte = consultar(s,Procurado);
    	if (Byte != -1) {
        	do{
            	system("cls");
		        printf("\n---------- Dados a serem alterados -----------\n\n");
		        printf("\n1 - Nome \n2 - Valor \n3 - Carga Horaria");
		        printf("\n4 - Aulas\n");
		        printf("\n0 - Voltar \n\n---------> Escolha uma opção: ");
		        scanf("%d",&op);
        		getchar();
            	switch(op){
                	case 1:
                    	if (Byte != -1) {
                            fsetpos(C, &Byte);
                            fread (&cur, sizeof(Cursos), 1, C);
                            printf("\n\nNome Atual: %s \nDeseja Alterar(S/N)?", cur.Nome_curso);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Nome do Curso:");
	                            fflush(stdin); gets(cur.Nome_curso);
	                            fsetpos(C, &Byte);
	                            fwrite(&cur, sizeof(Cursos), 1, C);
	
	                            printf("\n\nNome alterado com Sucesso!!\n");
	                            getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                    	break;
                	case 2:
                    	 if (Byte != -1) {
                            fsetpos(C, &Byte);
                            fread (&cur, sizeof(Cursos), 1, C);
                            printf("\n\nValor Atual: %s \nDeseja Alterar(S/N)?", cur.valor);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
                            	printf("\n\nDigite o novo Valor .:");
                            	fflush(stdin); gets(cur.valor);
                            	fsetpos(C, &Byte);
                            	fwrite(&cur, sizeof(Cursos), 1, C);
                            	printf("\nValor alterado com Sucesso!!\n");
                            	getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                		break;
                	case 3:
                    	if (Byte != -1) {
                            fsetpos(C, &Byte);
                            fread (&cur, sizeof(Cursos), 1, C);
                            printf("\n\nCarga Horaria Atual: %s \nDeseja Alterar(S/N)?", cur.carga_h);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
		                        printf("\n\nDigite a nova Carga Horaria:");
		                        fflush(stdin); gets(cur.carga_h);
		                        fsetpos(C, &Byte);
		                        fwrite(&cur, sizeof(Cursos), 1, C);
		
		                        printf("\n\nCarga Horaria alterada com Sucesso!!\n");
		                        getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
	                    break;
	                case 4:
                     	if (Byte != -1) {
                            fsetpos(C, &Byte);
                            fread (&cur, sizeof(Cursos), 1, C);
                            printf("\n\nAulas Atual: %s \nDeseja Alterar(S/N)?", cur.Aulas);
                            fflush(stdin); scanf("%c", &d);
		                    if(toupper(d) == 'S'){
		
		                        printf("\n\nDigite as Novas Aulas:");
		                        fflush(stdin); gets(cur.Aulas);
		                        fsetpos(C, &Byte);
		                        fwrite(&cur, sizeof(Cursos), 1, C);
		
		                        printf("\n\nAulas alteradas com Sucesso!!\n");
		                        getchar();
		                	}
                		} else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                		break;
				}
        	}while(op != 0);
    	}
    	fclose(C);
	}
	if(strcmp(s,"professores.bin")==0){
		int op;											
    	Professor prof;
    	fpos_t Byte;
    	FILE *B= fopen(s, "rb+");
    	Byte = consultar(s,Procurado);
    	if (Byte != -1) {
        	do{
            	system("cls");
		        printf("\n---------- Dados a serem alterados -----------\n\n");
		        printf("\n1 - Nome \n2 - Sobrenome \n3 - Celular");
		        printf("\n4 - E-mail \n5 - CPF \n6 - Data Nas ");
		        printf("\n7 - Rua/Nº \n8 - Complemento \n9 - Bairro");
		        printf("\n10 - Cidade \n11 - Estado \n12 - CEP");
		        printf("\n0 - Voltar \n\n---------> Escolha uma opção: ");
		        scanf("%d",&op);
		        getchar();
            	switch(op){
                	case 1:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1, B);
                            printf("\n\nNome Atual: %s \nDeseja Alterar(S/N)?", prof.Nome);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Nome:");
	                            fflush(stdin); gets(prof.Nome);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	                            printf("\n\nNome alterado com Sucesso!!\n");
	                            getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                    	break;
                	case 2:
	                     if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1, B);
                            printf("\n\nSobrenome Atual: %s \nDeseja Alterar(S/N)?", prof.Sobrenome);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Sobrenome:");
	                            fflush(stdin); gets(prof.Sobrenome);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	                            printf("\nSobrenome alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	                		getchar();
			            }
	    	            break;
                	case 3:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1, B);
                            printf("\n\nCelular Atual: %s \nDeseja Alterar(S/N)?", prof.Celular);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Nome:");
	                            fflush(stdin); gets(prof.Celular);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
                            	printf("\n\nCelular alterado com Sucesso!!\n");
                            	getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                    	break;
                	case 4:
                     	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1, B);
                            printf("\n\nE-mail Atual: %s \nDeseja Alterar(S/N)?", prof.Email);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo E-mail:");
	                            fflush(stdin); gets(prof.Email);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	                            printf("\n\nE-mail alterado com Sucesso!!\n");
	                            getchar();
	                    	}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                		break;
                	case 5:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1,B);
                            printf("\n\nCPF Atual: %s \nDeseja Alterar(S/N)?", prof.CPF_P);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
                            	printf("\n\nDigite o novo CPF:");
                            	fflush(stdin); gets(prof.CPF_P);
                            	fsetpos(B, &Byte);
                            	fwrite(&prof, sizeof(Professor), 1, B);
                            	printf("\n\nCPF alterado com Sucesso!!\n");                            
                            	getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                		break;
            		case 6:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1,B);
                            printf("\n\nCarga Horária Atual: %s \nDeseja Alterar(S/N)?", prof.Carga_horaria);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
		                        printf("\n\nDigite o nova Carga Horária:");
		                        fflush(stdin); gets(prof.Carga_horaria);
		                        fsetpos(B, &Byte);
		                        fwrite(&prof, sizeof(Professor), 1, B);
		                        printf("\n\nCarga Horária alterada com Sucesso!!\n");
		                        getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
            		case 7:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1,B);
                            printf("\n\nRua e Nº Atuais: %s \nDeseja Alterar(S/N)?", prof.endereco.Rua);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite a Nova Rua e Nº:");
	                            fflush(stdin); gets(prof.endereco.Rua);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	                            printf("\n\nRua e Nº alterados com Sucesso!!\n");
	                            getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                    	break;
                	case 8:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1,B);
                            printf("\n\nComplemento Atual: %s \nDeseja Alterar(S/N)?", prof.endereco.Complemento);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Complemnto:");
	                            fflush(stdin); gets(prof.endereco.Complemento);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	                            printf("\nComplemento alterado com Sucesso!!\n");
	                            getchar();
                    		}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                		break;
                	case 9:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1,B);
                            printf("\nBairro Atual: %s \nDeseja Alterar(S/N)?", prof.endereco.Bairro);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Bairro:");
	                            fflush(stdin); gets(prof.endereco.Bairro);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	
	                            printf("\nBairro alterado com Sucesso!!\n");
	                            getchar();
	                    	}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                    	break;
                	case 10:
                     	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1,B);
                            printf("\n\nCidade Atual: %s \nDeseja Alterar(S/N)?", prof.endereco.Cidade);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Cidade:");
	                            fflush(stdin); gets(prof.endereco.Cidade);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	                            printf("\n\nCidade alterado com Sucesso!!\n");
	                            getchar();
	                    	}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
			            }
		                break;
                	case 11:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1,B);
                            printf("\n\nEstado Atual: %s \nDeseja Alterar(S/N)?", prof.endereco.Estado);
                            fflush(stdin); scanf("%c", &d);
                        	if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Estado:");
	                            fflush(stdin); gets(prof.endereco.Estado);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	                            printf("\n\nEstado alterado com Sucesso!!\n");
	                            getchar();
	            	        }
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                		break;
            		case 12:
                    	if (Byte != -1) {
                            fsetpos(B, &Byte);
                            fread (&prof, sizeof(Professor), 1,B);
                            printf("\n\nCEP Atual: %s \nDeseja Alterar(S/N)?", prof.endereco.CEP);
                            fflush(stdin); scanf("%d", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o nova CEP:");
	                            fflush(stdin); gets(prof.endereco.CEP);
	                            fsetpos(B, &Byte);
	                            fwrite(&prof, sizeof(Professor), 1, B);
	                       	    printf("\n\nCEP alterado com Sucesso!!\n");
	                            getchar();
	                    	}
                		}else{
                			printf("Registo não encontrado");
                			getchar();
            			}
                		break;
				}
        	}while(op != 0);
        }else{
            printf("Registo não encontrado");
            getchar();
        }
	    fclose(B);
	}
	if(strcmp(s,"turmas.bin")==0){
		int op;
    	Turmas turma;
    	fpos_t Byte;
    	FILE *D= fopen(s, "rb+");
    	Byte = consultar(s,Procurado);
    	if (Byte != -1) {
        	do{
            	system("cls");
        		printf("\n---------- Dados a serem alterados -----------\n\n");
		        printf("\n1 - Nome \n2 - Aulas \n3 - Carga Horaria");
		        printf("\n0 - Voltar \n\n---------> Escolha uma opção: ");
		        scanf("%d",&op);
		        getchar();
	            switch(op){
	                case 1:
	                    if (Byte != -1) {
	                        fsetpos(D, &Byte);
                            fread (&turma, sizeof(Turmas), 1, D);
                            printf("\n\nNome Atual: %s \nDeseja Alterar(S/N)?", turma.Nome);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite o novo Nome:");
	                            fflush(stdin); gets(turma.Nome);
	                            fsetpos(D, &Byte);
	                            fwrite(&turma, sizeof(Turmas), 1, D);
	
	                            printf("\n\nNome alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	                		getchar();
	            		}
	                    break;
	                case 2:
	                    if (Byte != -1) {
                            fsetpos(D, &Byte);
                            fread (&turma, sizeof(Turmas), 1, D);
                            printf("\n\nAulas Atual: %s \nDeseja Alterar(S/N)?", turma.Aulas);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite a nova Carga Horaria:");
	                            fflush(stdin); gets(turma.carga_horaria);
	                            fsetpos(D, &Byte);
	                            fwrite(&turma, sizeof(Turmas), 1, D);
	
	                            printf("\n\nCarga Horaria alterado com Sucesso!!\n");
	                            getchar();
	                    	}
	                	}else{
	                		printf("Registo não encontrado");
	                		getchar();
			            }
	                    break;
	                case 3:
	                    if (Byte != -1) {
                            fsetpos(D, &Byte);
                            fread (&turma, sizeof(Turmas), 1, D);
                            printf("\n\nCarga Horaria Atual: %s \nDeseja Alterar(S/N)?", turma.carga_horaria);
                            fflush(stdin); scanf("%c", &d);
	                        if(toupper(d) == 'S'){
	                            printf("\n\nDigite as Novas Aulas:");
	                            fflush(stdin); gets(turma.Aulas);
	                            fsetpos(D, &Byte);
	                            fwrite(&turma, sizeof(Turmas), 1, D);
	                            printf("\n\nAulas alteradas com Sucesso!!\n");
	                            getchar();
	                    	}	
	                	}else{
	                		printf("Registo não encontrado");
	                		getchar();
	            		}
	                	break;
				}
        	}while(op != 0);
    	}fclose(D);
	}
}

void alterarmat(int ID, char m[16]){			
	//Função de alterar registro da matricula indicada, passando nos parametros o ID da matricula, e o nome do arquivo.
    int op;
	char d, Aprocurado[40];
    char c[12] = "cursos.bin";
    Matriculas mat;
	Aluno alunos;
	Cursos cur;
    fpos_t Byte;
    fpos_t ByteAl;
	char a[12] = "alunos.bin";	
    FILE *B = fopen(a, "rb+");
    FILE *A= fopen(m, "rb+");
    FILE *C = fopen(c, "rb+");
    if(A == NULL){
    	printf("\n\nErro ao Abrir o arquivo!\n\n");
        system("pause");
        exit(1);
    }else{
    	Byte = consultarID(m, ID);
     	if (Byte != -1){
        	do{
           	 	system("cls");
        		printf("\n---------- Dados a serem alterados -----------\n\n");
        		printf("\n1 - Aluno \n2 - Curso \n3 - Data Matricula");
        		printf("\n0 - Voltar \n\n---------> Escolha uma opção: ");
        		scanf("%d",&op);
        		getchar();
            	switch(op){
            		case 1:
            			if(B == NULL){
    	  					printf("\n\nErro ao Abrir o arquivo!\n\n");
			            	system("pause");
            				exit(1);
    					}else{
            				fsetpos(A, &Byte);
	            			fread(&mat,sizeof(Matriculas), 1, A);
    	        			ByteAl = consultarID(a, mat.ID_Aluno);
        	    			fsetpos(B, &ByteAl);
            				fread(&alunos,sizeof(Aluno),1,B);
            				printf("\n\nNome Atual: %s \nDeseja Alterar(S/N)?", alunos.Nome);
                    		fflush(stdin); scanf("%c", &d);
                    		if(toupper(d) == 'S'){
                    			system("cls");
                    			listar_alunosmat(a);
	                    		printf("Selecione o aluno a ser matriculado: ");
								scanf("%s", &Aprocurado);
    							ByteAl = consultar(a, Aprocurado);
								fsetpos(A, &Byte);
            					system("cls");
            					fsetpos(B, &ByteAl);
			    	        	fread(&alunos, sizeof(Aluno), 1, B);
			            		mat.ID_Aluno = alunos.ID_Aluno;
			            		fsetpos(A, &Byte);
								fwrite(&mat, sizeof(Matriculas), 1, A);
								printf("\n\nAluno alterado com Sucesso!!\n");
								getchar();
								getchar();       
          				  	}
            			}
            		break;  		
            		case 2:
            			if(C == NULL){
    	  					printf("\n\nErro ao Abrir o arquivo!\n\n");
			            	system("pause");
            				exit(1);
    					}else{
            				fsetpos(A, &Byte);
	            			fread(&mat,sizeof(Matriculas), 1, A);
    	        			ByteAl = consultarID(c, mat.ID_Curso);
        	    			fsetpos(C, &ByteAl);
            				fread(&cur,sizeof(Cursos),1,C);
            				printf("\n\nCurso Atual: %s \nDeseja Alterar(S/N)?", cur.Nome_curso);
                    		fflush(stdin); scanf("%c", &d);
                    		if(toupper(d) == 'S'){
                    			system("cls");
                    			listar(c);
	                    		printf("Selecione o curso para a matricula: ");
								scanf("%s", &Aprocurado);
    							ByteAl = consultar(c, Aprocurado);
								fsetpos(A, &Byte);
            					system("cls");
            					fsetpos(C, &ByteAl);
			    	        	fread(&cur, sizeof(Cursos), 1, C);
			            		mat.ID_Curso = cur.ID_Curso;
			            		fsetpos(A, &Byte);
								fwrite(&mat, sizeof(Matriculas), 1, A);
								printf("\n\nCurso alterado com Sucesso!!\n");
								getchar();
								getchar();
          				  	}
            			}
            				break;
            			case 3:
            				fsetpos(A, &Byte);
	            			fread(&mat,sizeof(Matriculas), 1, A);
    	        			printf("\n\nData Atual: %s \nDeseja Alterar(S/N)?", mat.DataMat);
        	    			fflush(stdin); scanf("%c", &d);
            				if(toupper(d) == 'S'){
            					printf("Digite a data da matricula: ");
								fflush(stdin); gets(mat.DataMat);
								fsetpos(A, &Byte);
								fwrite(&mat, sizeof(Matriculas), 1, A);
								printf("\n\nData alterada com Sucesso!!\n");
        	    	        }								
    				}
        		}while(op != 0);
    	}else{
    		printf("Registo não encontrado");
    		getchar();
    	}
	}
    fclose(A);
    fclose(B);
    fclose(C);
}

void dadosID(char s[20], int ID){
	//Função universal para exibir os dados pelo ID informado.
	if(strcmp(s,"alunos.bin")==0){
	    Aluno alunos;
	    fpos_t Byte;
	    FILE *A = fopen(s, "rb");
	    Byte = consultarID(s, ID);
	    if(A == NULL){
	        printf("\n\nErro ao Abrir o arquivo!\n\n");
            system("pause");
	        exit(1);
	    }else{
	        if (Byte != -1){
				while(fread(&alunos, sizeof(Aluno), 1, A)){
					if(ID == alunos.ID_Aluno){
		   	        	printf("Nome .........: %s\n", alunos.Nome);
	   		        	printf("Sobrenome ....: %s\n", alunos.Sobrenome);
			            printf("Celular ......: %s\n", alunos.Celular);
		    	        printf("E-mail .......: %s\n", alunos.Email);
		        	    printf("CPF ..........: %s\n", alunos.CPF_A);	
			            printf("Data Nas .....: %s\n", alunos.DataNas);
		           		printf("Rua ..........: %s\n", alunos.endereco.Rua);
			            printf("Complemento ..: %s\n", alunos.endereco.Complemento);
			            printf("Bairro........: %s\n", alunos.endereco.Bairro);
			            printf("Cidade .......: %s\n", alunos.endereco.Cidade);
		    	        printf("Estado .......: %s\n", alunos.endereco.Estado);
		            	printf("CEP ..........: %s\n", alunos.endereco.CEP);
			            printf("ID ...........: %d\n", alunos.ID_Aluno);
	        			printf("\n-------------------\n\n");
	        			fclose(A);
	                }
	            }
	        }
	   	}
	}
	if(strcmp(s,"cursos.bin")==0){
	    Cursos cur;
	    fpos_t Byte;
	    FILE *C = fopen(s, "rb");
	    Byte = consultarID(s, ID);
        if(C == NULL){
                    printf("\n\nErro ao Abrir o arquivo!\n\n");
                    system("pause");
                    exit(1);
        }else{
        	while(fread(&cur, sizeof(Cursos), 1, C)){
				if(ID ==cur.ID_Curso){
            		printf("Nome .........: %s\n", cur.Nome_curso);
            		printf("Valor ........: %s\n", cur.valor);
            		printf("Carga Horaria : %s\n", cur.carga_h);
            		printf("Aulas ........: %s\n", cur.Aulas);
        			printf("\n-------------------\n\n");
        			fclose(C);
            	}
        	}
    	}
	}
	if(strcmp(s,"matriculas.bin")==0){	
	    Matriculas mat;
	    fpos_t Byte;
	    FILE *A = fopen(s, "rb");
	    Byte = consultarID(s, ID);
	    if(A == NULL){
	                printf("\n\nErro ao Abrir o arquivo!\n\n");
	                system("pause");
	                exit(1);
	    }else{
	        if (Byte != -1){
	            system("cls");
	        	Texto("dados   ",-1);
				while(fread(&mat, sizeof(Matriculas), 1, A)){
					if(ID ==mat.ID_Mat){
						printf("\n\n ---------- Dados do Aluno Matriculado ----------\n\n");
			            dadosID("alunos.bin", mat.ID_Aluno);
			            
			            printf("\n\n ---------- Dados do Curso Matriculado ----------\n\n");
						dadosID("cursos.bin", mat.ID_Curso);
		        		printf("\n-------------------\n\n");		
		        		getchar();
	    			}
				}
	        }
		}
	}
}

int defineID(char s[12]){					
	//Função universal para gerar o ID, basta passar nos parametros qual arquivo você quer que gere o ID.
	int id = 1;
	fpos_t *Byte = 0;
	if(strcmp(s,"alunos.bin")==0){
		FILE *A = fopen("alunosid.bin", "rb");
        if(A == NULL){
        	FILE *B = fopen("alunosid.bin", "ab+");
        	fwrite(&id, sizeof(int), 1, B);
        	fclose(B);
        	fclose(A);
        }else{
        	
			fsetpos(A, Byte);
			id += fread(&id,sizeof(int),1,A);
			fclose(A);
			FILE *C = fopen("alunosid.bin", "wb");
			fwrite(&id, sizeof(int), 1, C);
		}	
	    fclose(A);	
		return id;
	}
	if(strcmp(s,"cursos.bin")==0){
		FILE *A = fopen("cursosid.bin", "rb");
        if(A == NULL){
        	FILE *B = fopen("cursosid.bin", "ab+");
        	fwrite(&id, sizeof(int), 1, B);
        	fclose(B);
        	fclose(A);
        }else{
			fsetpos(A, Byte);
			id += fread(&id,sizeof(int),1,A);
			fclose(A);
			FILE *C = fopen("cursosid.bin", "wb");
			fwrite(&id, sizeof(int), 1, C);
		}	
	    fclose(A);	
		return id;
	}
	if(strcmp(s,"professores.bin")==0){
		FILE *A = fopen("professoresid.bin", "rb");
        if(A == NULL){
        	FILE *B = fopen("professoresid.bin", "ab+");
        	fwrite(&id, sizeof(int), 1, B);
        	fclose(B);
        	fclose(A);
        }else{
			fsetpos(A, Byte);
			id += fread(&id,sizeof(int),1,A);
			fclose(A);
			FILE *C = fopen("professoresid.bin", "wb");
			fwrite(&id, sizeof(int), 1, C);
		}	
	    fclose(A);	
		return id;
	}
	if(strcmp(s,"turmas.bin")==0){
		FILE *A = fopen("turmasid.bin", "rb");
        if(A == NULL){
        	FILE *B = fopen("turmasid.bin", "ab+");
        	fwrite(&id, sizeof(int), 1, B);
        	fclose(B);
        	fclose(A);
        }else{
			fsetpos(A, Byte);
			id += fread(&id,sizeof(int),1,A);
			fclose(A);
			FILE *C = fopen("turmasid.bin", "wb");
			fwrite(&id, sizeof(int), 1, C);
		}	
	    fclose(A);	
		return id;
	}
	if(strcmp(s,"matriculas.bin")==0){
		FILE *A = fopen("matriculasid.bin", "rb");
        if(A == NULL){
        	FILE *B = fopen("matriculasid.bin", "ab+");
        	fwrite(&id, sizeof(int), 1, B);
        	fclose(B);
        	fclose(A);
        }else{
			fsetpos(A, Byte);
			id += fread(&id,sizeof(int),1,A);
			fclose(A);
			FILE *C = fopen("matriculasid.bin", "wb");
			fwrite(&id, sizeof(int), 1, C);
		}	
	    fclose(A);	
		return id;
	}
}

int excluir_todos(char s[12]){									
	//Função universal para limpar todos os registros, passando como parametro o nome do arquivo.
    int op;
    printf("Deseja Realmente excluir todos? \n [1-Sim ou 2-Não]: ");
    scanf("%d",&op);
    if (op == 1){
        struct  midia;
        FILE *A = fopen(s, "w");
        printf("\n\nTodos os Dados excluidos com Exito!\n\n");
        fclose(A);
    }
    getchar();
}

void menu_alunos(){												
	//Menu de alunos, dentro de um loop existe um switch case que alterna diante sua escolha de ação.
    int op, posReg, posAlt;
    char Procurado[40];
    char s[12]="alunos.bin";
    do{
        system("cls");
        Texto("alunos  ",-1);
        printf("\n\t\t\t1 - Cadastrar aluno; \n\t\t\t2 - Lista de Alunos;");
        printf("\n\t\t\t3 - Consultar Aluno; \n\t\t\t4 - Alteração de Registro; \n\t\t\t5 - Remover Aluno; ");
        printf("\n\t\t\t6 - Excluir todos os Registros;");
        printf("\n\t\t\t0 - Voltar \n\n\t\t\t-> Escolha uma opção:  ");
        scanf("%d",&op);
        switch(op){
            case 1:
                cadastrar(s);
                break;
            case 2:
                listar(s);
                break;
            case 3:
                system("cls");
                Texto("consulta",-1);
                printf("\nDigite o nome Desejado: ");
                scanf("%s", Procurado);
                posReg = consultar(s, Procurado);
                dados(s, Procurado);
                getchar();
                break;
            case 4:
                system("cls");
                Texto("alteracao",-1);
                printf("\nDigite o nome Desejado: ");
                scanf("%s", Procurado);
                alterar(s, Procurado);
                break;
            case 5:
                system("cls");
                Texto("remocao ",-1);
                printf("\nDigite o nome Desejado: ");
                scanf("%s", Procurado);
                remover(s, Procurado);
                break;
            case 6:
				system("cls");
                Texto("aviso    ",-1);
                printf("\n\n---------- Excluir Todos Registros de Alunos ----------\n\n");
                excluir_todos(s);
                break;
        }
        getchar();
    }while(op != 0);
}

void menu_professores(){										
	//Menu de professores, dentro de um loop existe um switch case que alterna diante sua escolha de ação.
    int op, posRegP, posAlt;
    char procurado[40];
    char s[15]= "professores.bin";
    do{
        system("cls");
       	Texto("professor",-1);
        printf("\n\t\t\t1 - Cadastrar Professor; \n\t\t\t2 - Lista de Professores;");
        printf("\n\t\t\t3 - Consultar Professor; \n\t\t\t4 - Alteração de Professores; \n\t\t\t5 - Remover Professor;");
        printf("\n\t\t\t6 - Excluir todos os Registros;");
        printf("\n\t\t\t0 - Voltar \n\n\t\t\t---------> Escolha uma opção: ");
        scanf("%d",&op);
            switch(op){
                case 1:
                    cadastrar(s);
                    break;
                case 2:
                    listar(s);
                    getchar();
                    break;
                case 3:              
                    system("cls");
					Texto("consulta",-1);
                    printf("\n\n---------- Consulta de Professores ----------\n\n");
                    printf("\nDigite o nome Desejado: ");
                    scanf("%s", &procurado);
                    posRegP = consultar(s, procurado);
                    dados(s, procurado);
                    break;
                case 4:
                    system("cls");
                    Texto("alteracao", -1);
                    printf("\n\n---------- Alteração de Registros de Professores ----------\n\n");
                    printf("\nDigite o nome Desejado: ");
                    scanf("%s", procurado);
                    alterar(s, procurado);
                    break;
                case 5:
                    system("cls");
                    Texto("remocao  ",-1);
                    printf("\n\n---------- Excluir Registro de Professor ----------\n\n");
                    printf("\nDigite o nome Desejado: ");
                    scanf("%s", procurado);
                    remover(s, procurado);
                    break;
                case 6:
                    system("cls");
					Texto("aviso   ",-1);
                    printf("\n\n---------- Excluir Todos Registros de Professores ----------\n\n");
                    excluir_todos(s);
                    break;
        }
    }while(op != 0);
}

void menu_cursos(){												
	//Menu de cursos, dentro de um loop existe um switch case que alterna diante sua escolha de ação.
    int op, posReg, posAlt;
    char procurado[40];
    char r[15]= "cursos.bin";
    do{
        system("cls");
        Texto("curso   ",-1);
        printf("\n\t\t\t1 - Cadastrar Curso; \n\t\t\t2 - Lista de Cursos;");
        printf("\n\t\t\t3 - Consultar Curso; \n\t\t\t4 - Alteração dos dados do Cursos; \n\t\t\t5 - Excluir um Curso; ");
        printf("\n\t\t\t6 - Excluir todos os Registros;");
        printf("\n\t\t\t0 - Voltar \n\n\t\t\t---------> Escolha uma opção: ");
        scanf("%d",&op);
            switch(op){
                case 1:
                    cadastrar(r);
                    break;
                case 2:
                    listar(r);
                    break;
                case 3:
                    system("cls");
					Texto("consulta",-1);
                    printf("\nDigite o nome do Curso Desejado: ");
                    scanf("%s", procurado);
                    posReg = consultar(r, procurado);
                    dados(r, procurado);
                    break;
                case 4:
                    system("cls");
                    Texto("alteracao",-1);
                    printf("\nDigite o nome do Curso Desejado: ");
                    scanf("%s", procurado);
                    alterar(r, procurado);
                    break;
                case 5:
                	system("cls");
                	Texto("remocao  ",-1);
                    printf("\nDigite o nome do Curso Desejado: ");
                    scanf("%s", procurado);
                    remover(r, procurado);
                    break;
                case 6:
                    system("cls");
					Texto("aviso    ",-1);
                    printf("\n\n---------- Excluir Todos Registros de Cursos ----------\n\n");
                    excluir_todos(r);
                    break;
            }
            getchar();
    }while(op != 0);
}

void menu_turmas(){											
	//Menu de turmas, dentro de um loop existe um switch case que alterna diante sua escolha de ação.
    int op, posReg, posAlt;
    char procurado[40];
    char t[15]= "turmas.bin";
    do{
        system("cls");
        Texto("turma    ",-1);
        printf("\n\t\t\t1 - Cadastrar Turma; \n\t\t\t2 - Lista de turmas;");
        printf("\n\t\t\t3 - Consultar Turma; \n\t\t\t4 - Alteração dos dados da Turma; \n\t\t\t5 - Excluir uma Turma;");
        printf("\n\t\t\t6 - Excluir todos os Registros;");
        printf("\n\t\t\t0 - Voltar \n\n\t\t\t---------> Escolha uma opção: ");
        scanf("%d",&op);
            switch(op){
                case 1:
                    cadastrar(t);
                    break;
                case 2:
                    listar(t);
                    break;
                case 3:
                    system("cls");
                    Texto("consulta",-1);
                    printf("\nDigite o nome da Turma Desejado: ");
                    scanf("%s", procurado);
                    posReg = consultar(t, procurado);
                    dados(t, procurado);
                    getchar();
                    break;
                case 4:
                    system("cls");
                    Texto("alteracao",-1);
                	printf("\nDigite o nome do Curso Desejado: ");
                    scanf("%s", procurado);
                	alterar(t, procurado);
                    break;
                case 5:
					system("cls");
					Texto("remocao   ",-1);
                    printf("\nDigite o nome do Turma Desejado: ");
                    scanf("%s", procurado);
                    remover(t, procurado);
                    break;
                case 6:
                	system("cls");
					Texto("aviso    ",-1);
                    printf("\n\n---------- Excluir Todos Registros de Turmas ----------\n\n");
                    excluir_todos(t);
                    break;
            }
            getchar();
    }while(op != 0);
}

void menu_matricula(){						
	//Menu de matriculas, dentro de um loop existe um switch case que alterna diante sua escolha de ação.
	int op, posReg, posAlt, ID;
    char procurado[40];
	char m[16] = "matriculas.bin";
	do{
		system("cls");
		Texto("matricula",-1);
		printf("\n\t\t\t1 - Matricular; \n\t\t\t2 - Lista de Matriculas;");
        printf("\n\t\t\t3 - Consultar Matricula; \n\t\t\t4 - Alteração dos dados da Matricula; \n\t\t\t5 - Excluir uma Matricula;");
        printf("\n\t\t\t6 - Excluir todos os Registros;");
        printf("\n\t\t\t0 - Voltar \n\n\t\t\t---------> Escolha uma opção: ");
        scanf("%d",&op);
            switch(op){
                case 1:
                    cadastrar(m);
                    break;
                case 2:
                    listar(m);
                    break;
                case 3:
                    system("cls");
                    Texto("consulta",-1);
                    printf("\nDigite o ID da matricula desejada: ");
                    scanf("%d", &ID);
                    posReg = consultarID(m, ID);
                    dadosID(m, ID);
                    getchar();
                    break;
                case 4:
                    system("cls");
                    Texto("alteracao",-1);
                   	printf("\nDigite o ID da matricula desejada: ");
                    scanf("%d", &ID);
                    alterarmat(ID, m);
                    break;
                case 5:
					system("cls");
					Texto("remocao    ",-1);
                    printf("\nDigite o ID da Matricula Desejada: ");
                    scanf("%d", &ID);
                    removermat(ID, m);
                    break;
                case 6:
                    system("cls");
					Texto("aviso     ",-1);
                    printf("\n\n---------- Excluir Todos Registros de Matriculas ----------\n\n");
                    excluir_todos(m);
                    break;
            }
            getchar();
    }while(op != 0);
}

void main(){
    setlocale(LC_ALL, "");
    //Menu principal, dentro de um loop existe um switch case que alterna diante sua escolha de ação.
    int op;
    do{
        system("cls");
        printf(ANSI_COLOR_RESET);
        Texto("escola", -1);
        printf(ANSI_COLOR_BLUE  "\n\t\t\t1 - Menu de Alunos");
		printf(ANSI_COLOR_RED "\n\t\t\t2 - Menu de Professores");
        printf(ANSI_COLOR_GREEN "\n\t\t\t3 - Menu de Cursos");
		printf(ANSI_COLOR_MAGENTA "\n\t\t\t4 - Menu de Turmas");
		printf(ANSI_COLOR_YELLOW "\n\t\t\t5 - Menu Matricula");
        printf(ANSI_COLOR_RESET "\n\t\t\t0 - Sair \n\n\t\t   Escolha uma opção e tecle ENTER .:");
		scanf("%d",&op);
           switch(op){
                case 1:
                	system("color 1");
                    menu_alunos();
                break;
            case 2:
            		system("color 4");
                    menu_professores();
                break;
            case 3:
            		system("color 2");
                    menu_cursos();
                break;
            case 4:
            		system("color 5");
                    menu_turmas();
                break;
            case 5:
            		system("color 6");
            		menu_matricula();
            	break;
        }getchar();
    }while(op != 0);
    system("cls");
    printf("\n\n\n\t -- Até Mais! -- \n\n\n");
}
