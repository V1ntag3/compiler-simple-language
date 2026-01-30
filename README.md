# ⚙️ Compilador de LPMS

Este projeto consiste na implementação de um **compilador para a linguagem LPMS**, desenvolvido em **Python**, com foco em aprendizado de conceitos de compiladores, análise sintática, geração de código intermediário e geração de código em Assembly.

O projeto utiliza um arquivo `requirements.txt` para gerenciamento de dependências.

---

## 📌 Objetivo do Projeto

O objetivo principal é compreender, na prática, as etapas envolvidas no desenvolvimento de um compilador, incluindo:

- Análise léxica
- Análise sintática
- Construção da AST (Abstract Syntax Tree)
- Geração de código de três endereços
- Geração de código Assembly (x86_64)

---

## 🛠️ Requisitos

- Python 3.13 ou superior
- pip
- Ambiente virtual (recomendado)

---

## ⚙️ Configuração do Ambiente

### 1️⃣ Criação do Ambiente Virtual

```bash
python3 -m venv venv
```
2️⃣ Ativação do Ambiente Virtual
Windows
```bash
.\venv\Scripts\activate
```

Linux / macOS
```bash
source venv/bin/activate
```
## 3️⃣ Instalação das Dependências
```bash
pip install -r requirements.txt
```
### ▶️ Executando o Projeto
Após configurar o ambiente, execute o compilador com:
```bash
python3 main.py input.lps
```
Onde:
- main.py é o arquivo principal do compilador
- input.lps é o arquivo de entrada contendo o código-fonte em LPMS

## 📁 Arquivos Importantes
Arquivo	Descrição
```bash
main.py	#Arquivo principal do compilador
input.lps	#Arquivo de teste principal
input2.lps	#Arquivo de teste alternativo
main_etapa_2.py	#Implementação da etapa 2 com suporte à AST
assembly_code.s	#Código Assembly gerado pelo compilador
```
## 🧠 Funcionamento do Compilador
Durante a execução, o compilador:

1. Lê o código-fonte LPMS
2. Gera a AST (Abstract Syntax Tree)
3. Produz o código intermediário (três endereços)
4. Gera o código Assembly (x86_64)
5. Salva o resultado no arquivo assembly_code.s
6. O código intermediário é exibido no terminal.

## 🧪 Testes
Os arquivos:
```bash
input.lps
input2.lps
```
Contêm exemplos funcionais que demonstram as operações suportadas pelo compilador.

## 💻 Execução do Código Assembly
O código Assembly gerado pode ser executado online utilizando:

🔗 https://www.mycompiler.io/pt/new/asm-x86_64

Basta copiar o conteúdo do arquivo assembly_code.s e colar na plataforma.

## 📌 Observações
- A implementação da AST foi finalizada na etapa 2, disponível em main_etapa_2.py.
- Essa funcionalidade foi adicionada posteriormente, conforme solicitado na disciplina.
- Algumas funcionalidades podem estar em fase experimental.
