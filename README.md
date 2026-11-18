# Controle de Impressora Térmica Elgin (i8 / i9)

Sistema em linguagem C para controle de impressoras térmicas Elgin via DLL (`E1_Impressora01.dll`) no Windows.

## Integrantes do Grupo
* Robert Lucas
* Martinho
* Gabriel Silva Oliveira
* Rafael Manuel

## Pré-requisitos e Compilação (Windows)
Certifique-se de que os arquivos `E1_Impressora01.dll` (mesma arquitetura do compilador: x86 ou x64), `XMLSAT.xml` e `CANC_SAT.xml` estejam na raiz do projeto junto com o executável.

Para compilar via terminal (GCC/MinGW):
```bash
gcc main.c -o impressora.exe
