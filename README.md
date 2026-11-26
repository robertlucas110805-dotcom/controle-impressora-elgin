# 🖨️ Controle de Impressora Térmica Elgin (i8 / i9)

## 📘 Sobre o Projeto

Este projeto foi desenvolvido por alunos com o objetivo de criar uma aplicação em linguagem **C** capaz de controlar impressoras térmicas Elgin dos modelos **i8 e i9**, utilizando a DLL oficial `E1_Impressora01.dll`.

O sistema permite realizar operações de impressão e enviar comandos diretamente à impressora, utilizando os recursos disponibilizados pela biblioteca da Elgin.

O trabalho foi desenvolvido como parte das atividades acadêmicas do curso de Ciência da Computação.

---

## 🧰 Tecnologias Utilizadas

- **Linguagem C**
- **GCC / MinGW** – Compilador
- **E1_Impressora01.dll** – Biblioteca de comunicação da Elgin
- **Git e GitHub** – Controle de versão e armazenamento do projeto
- **Windows** – Sistema operacional de execução

---

## 📁 Estrutura do Projeto

```text
Projeto/
│
├── .gitignore
├── CANC_SAT.xml
├── E1_Impressora01.dll
├── README.md
├── XMLSAT.xml
└── main.c
```

**Descrição dos arquivos:**

- `main.c`: código-fonte principal do sistema.
- `E1_Impressora01.dll`: biblioteca responsável pela comunicação com a impressora.
- `XMLSAT.xml`: arquivo XML utilizado nas operações SAT.
- `CANC_SAT.xml`: arquivo XML utilizado no cancelamento SAT.
- `README.md`: documentação do projeto.

---

## ⚙️ Instalação e Execução

### 1. Baixar o Projeto do GitHub

1. Acesse o repositório do projeto no GitHub.
2. Clique no botão verde **Code**.
3. Selecione a opção **Download ZIP**.
4. Aguarde o download do arquivo.

### 2. Extrair os Arquivos

1. Acesse a pasta onde o arquivo ZIP foi baixado.
2. Clique com o botão direito sobre ele.
3. Selecione **Extrair Tudo**.
4. Escolha um local para salvar a pasta do projeto.
5. Abra a pasta extraída.

### 3. Instalar e Configurar o Compilador

Para compilar o projeto, é necessário possuir o GCC instalado no Windows, por meio do MinGW.

1. Instale uma distribuição do MinGW que disponibilize o GCC.
2. Configure o caminho da pasta `bin` do compilador nas variáveis de ambiente do Windows (PATH).
3. Abra o Prompt de Comando (CMD).
4. Digite o seguinte comando:

```bash
gcc --version
```

5. Se aparecer a versão do GCC, significa que o compilador está instalado e disponível no terminal.

### 4. Verificar os Arquivos Necessários

Antes de compilar e executar o programa, verifique se os seguintes arquivos estão na pasta principal do projeto:

- `main.c`
- `E1_Impressora01.dll`
- `XMLSAT.xml`
- `CANC_SAT.xml`

**Importante:** a DLL precisa ter a mesma arquitetura do compilador utilizado (x86 ou x64).

Os arquivos XML e a DLL também precisam estar disponíveis na pasta de execução do programa.

### 5. Compilar o Projeto

1. Abra a pasta principal do projeto.
2. Clique na barra de endereço do Explorador de Arquivos.
3. Digite `cmd` e pressione Enter.
4. O Prompt de Comando será aberto diretamente na pasta do projeto.
5. Execute o seguinte comando:

```bash
gcc main.c -o impressora.exe
```

6. Pressione Enter.
7. Caso não apareçam erros, o arquivo `impressora.exe` será gerado na pasta.

### 6. Executar o Programa

Após a compilação:

1. No mesmo Prompt de Comando, execute:

```bash
impressora.exe
```

2. Pressione Enter.
3. Aguarde a inicialização do programa.
4. Siga as instruções apresentadas na tela.
5. Utilize as opções disponíveis para realizar as operações com a impressora Elgin.

**Observação:** a impressora deve estar conectada e configurada corretamente para que os testes de comunicação e impressão possam ser realizados.

---

## 🧪 Testes do Sistema

O projeto permite realizar testes das funcionalidades de comunicação e impressão, incluindo:

- Teste de conexão com a impressora.
- Impressão de textos.
- Impressão de QR Code.
- Impressão de código de barras.
- Impressão de arquivos XML SAT.
- Operação de cancelamento SAT.
- Acionamento da gaveta de dinheiro.
- Emissão de sinal sonoro.

---

## ⚠️ Possíveis Problemas

**Erro: GCC não reconhecido**

Verifique se o MinGW está instalado e se o caminho da pasta `bin` foi adicionado corretamente ao PATH.

**Erro: DLL não encontrada**

Verifique se o arquivo `E1_Impressora01.dll` está na pasta de execução do programa.

**Erro relacionado à arquitetura da DLL**

**Erro ao localizar os arquivos XML**

Verifique se `XMLSAT.xml` e `CANC_SAT.xml` estão disponíveis na pasta de execução do programa.

---

## 👥 Integrantes do Grupo

- Robert Lucas
- Martinho
- Gabriel Silva Oliveira
- Rafael Manuel

---

## 📄 Licença e Referências

Projeto desenvolvido para fins acadêmicos, utilizando a biblioteca de comunicação disponibilizada pela Elgin.

Consulte a documentação e os materiais técnicos oficiais da Elgin para obter informações adicionais sobre a DLL e os comandos de comunicação com a impressora.
## Pré-requisitos e Compilação (Windows)
Certifique-se de que os arquivos `E1_Impressora01.dll` (mesma arquitetura do compilador: x86 ou x64), `XMLSAT.xml` e `CANC_SAT.xml` estejam na raiz do projeto junto com o executável.

Para compilar via terminal (GCC/MinGW):
```bash
gcc main.c -o impressora.exe
