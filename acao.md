# Plano de Ação para a Entrega do Projeto

## Entrega Obrigatória

### Passos para a Configuração do Banco de Dados no Oracle SQL Developer

1. **Download e Instalação do Oracle SQL Developer**
   - Acesse o site [Oracle SQL Developer](https://www.oracle.com/database/sqldeveloper/technologies/download/).
   - Faça o download da versão correspondente ao seu sistema operacional (Windows, Linux ou Mac OSX).
   - Realize o cadastro gratuito, se necessário.
   - Descompacte o arquivo baixado e execute o programa SQLDEVELOPER.

2. **Configuração da Conexão com o Banco de Dados**
   - Clique em “Nova Conexão” (ícone + em verde).
   - Preencha os campos:
     - **Nome:** FIAP (ou outro nome de sua escolha).
     - **Nome do Usuário:** Seu RM (ex.: RM12345).
     - **Senha:** Sua data de nascimento no formato DDMMYY (ex.: 070905).
     - **Nome do Host:** oracle.fiap.com.br.
     - **Porta:** 1521.
     - **SID:** ORCL.
   - Clique em **Testar** para verificar a conexão.

3. **Importação dos Dados**
   - Localize o ícone “Tabelas (Filtrado)” e clique com o botão direito.
   - Selecione “Importar Dados”.
   - Carregue o arquivo da Fase 2 com os dados dos sensores.
   - Defina o nome da tabela (sem espaços ou caracteres especiais, máximo de 30 caracteres).
   - Configure os campos e colunas conforme necessário.
   - Finalize a importação e execute o comando `SELECT * FROM NOME_DA_SUA_TABELA;` para verificar os dados.

4. **Exploração dos Dados**
   - Realize consultas SQL para explorar os dados armazenados no banco Oracle.

### Entregáveis

- **Repositório no GitHub:**
  - Estrutura organizada (ex.: `meugit/cursotiao/pbl/fase3/...`).
  - Arquivo `README.md` documentando o projeto com prints do banco.
  - Códigos em C/C++ ou Python utilizados.

- **Vídeo:**
  - Gravar um vídeo de até 5 minutos (YouTube, como “não listado”) demonstrando o funcionamento do projeto.

---

## Programa Ir Além (Opcional)

### Opção 1 – Dashboard em Python

1. **Ferramentas:**
   - Utilize bibliotecas como Streamlit ou Dash.

2. **Funcionalidades:**
   - Visualizar níveis de umidade, P, K e pH.
   - Exibir status da irrigação.
   - Fornecer sugestões de irrigação baseadas em clima.

3. **Entregáveis:**
   - Código-fonte do dashboard.
   - Prints ou vídeo demonstrando o funcionamento.

### Opção 2 – Machine Learning no Agronegócio

1. **Base de Dados:**
   - Utilize o arquivo `produtos_agricolas.csv` com as variáveis: N, P, K, temperatura, umidade, pH, chuva, label.

2. **Atividades:**
   - Realizar análise exploratória com pelo menos 5 gráficos.
   - Identificar o “perfil ideal” de solo/clima para 3 culturas escolhidas.
   - Desenvolver 5 modelos preditivos com diferentes algoritmos.
   - Comparar os resultados dos modelos.

3. **Entregáveis:**
   - Jupyter Notebook (`SeuNome_RMxxxx_fase3_cap1.ipynb`) com código e análises.
   - Vídeo de até 5 minutos (YouTube, como “não listado”) apresentando o trabalho.