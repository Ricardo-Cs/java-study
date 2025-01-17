# Repositório de Estudo de Java

Este repositório foi criado para organizar meus estudos em Java. Aqui você encontrará exemplos de código, anotações, projetos e exercícios para praticar os conceitos fundamentais e avançados da linguagem Java.

## Propósito

- Aprender os conceitos básicos de Java.
- Praticar a sintaxe da linguagem e as melhores práticas.
- Desenvolver projetos simples para aplicar o conhecimento adquirido.
- Explorar bibliotecas e frameworks populares.

---

## Requisitos para começar

### 1. Instalação do Java

1. Acesse o site oficial do Java para download: [Oracle Java Downloads](https://www.oracle.com/java/technologies/javase-downloads.html).
2. Baixe e instale a versão mais recente (ou LTS) do Java Development Kit (JDK) para o seu sistema operacional.

### 2. Configuração de Variáveis de Ambiente

#### Windows

1. Abra o **Painel de Controle** e vá para **Sistema > Configurações Avançadas do Sistema > Variáveis de Ambiente**.
2. Encontre a variável `Path` na seção **Variáveis do Sistema** e clique em **Editar**.
3. Adicione o caminho para o diretório `bin` do JDK (exemplo: `C:\Program Files\Java\jdk-XX\bin`).
4. Crie uma nova variável de ambiente chamada `JAVA_HOME` com o caminho para o diretório principal do JDK (exemplo: `C:\Program Files\Java\jdk-XX`).
5. Teste as configurações no terminal:

   ```bash
   java -version
   javac -version
   ```

#### Linux/MacOS

1. Abra o terminal e edite o arquivo de configuração do shell (como `.bashrc` ou `.zshrc`):

   ```bash
   nano ~/.bashrc
   ```

2. Adicione as seguintes linhas:

   ```bash
   export JAVA_HOME=/caminho/para/jdk
   export PATH=$JAVA_HOME/bin:$PATH
   ```

3. Atualize o shell:

   ```bash
   source ~/.bashrc
   ```

4. Teste as configurações:

   ```bash
   java -version
   javac -version
   ```

---

## Estrutura do Repositório

- **`docs/`**: Minhas anotações/códigos de referência.
- **`exercises/`**: Exercícios práticos organizados por tópico.
- **`projects/`**: Projetos simples para consolidar o aprendizado.

---

## Ferramentas Recomendadas

- **Editor/IDE**:
    - [IntelliJ IDEA](https://www.jetbrains.com/idea/) (recomendado)
    - [Eclipse](https://www.eclipse.org/)
    - [VS Code](https://code.visualstudio.com/) com extensão de Java

- **Compilação e execução no terminal**:
    - Para compilar: `javac NomeDoArquivo.java`
    - Para executar: `java NomeDoArquivo`

---

**Bons estudos! ☕**
