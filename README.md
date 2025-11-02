# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Sistema de Irrigação Inteligente - Fase 3

## Grupo 16 - Oracle

## 👨‍🎓 Integrantes (por ordem alfabética): 
- <a href="https://www.linkedin.com/in/daniel-baião-0b351049/">Daniel Emilio Baião</a>
- <a href="https://www.linkedin.com/company/inova-fusca">Erik Criscuolo</a>
- <a href="https://www.linkedin.com/company/inova-fusca">Hugo Rodrigues Carvalho Silva</a>
- <a href="https://www.linkedin.com/company/inova-fusca">Marcus Vinícius Loureiro Garcia</a> 
- <a href="https://www.linkedin.com/company/inova-fusca">Sidney William de Paula Dias</a> 

## 👩‍🏫 Professores:
### Tutora 
- <a href="https://www.linkedin.com/in/sabrina-otoni-22525519b/">Sabrina Otoni</a>
### Coordenador
- <a href="https://www.linkedin.com/company/inova-fusca">André Godoi Chiovato</a>


## 📜 Descrição

Este projeto implementa um **Sistema de Irrigação Inteligente** desenvolvido para o agronegócio, utilizando tecnologias de IoT (Internet das Coisas) e análise de dados para otimizar o uso da água na agricultura.

### Objetivos do Projeto

O sistema tem como principal objetivo automatizar e otimizar o processo de irrigação de culturas, contribuindo para:
- **Sustentabilidade**: Redução do desperdício de água através do monitoramento inteligente
- **Produtividade**: Melhoria na qualidade e quantidade da produção agrícola
- **Eficiência**: Automatização do processo de irrigação baseado em dados reais dos sensores

### Funcionalidades Principais

1. **Monitoramento em Tempo Real**: Coleta de dados de sensores de umidade do solo, luminosidade (LDR), nutrientes (N, P, K) e pH
2. **Sistema de Irrigação Automatizada**: Ativação automática do sistema de irrigação (relay) baseada nas condições do solo
3. **Análise de Dados**: Processamento e análise dos dados históricos coletados pelos sensores
4. **Banco de Dados Oracle**: Armazenamento e consulta eficiente dos dados no Oracle SQL Developer
5. **Dashboard Interativo**: Visualização das métricas e status do sistema em tempo real

### Tecnologias Utilizadas

- **Hardware**: Sensores de umidade DHT, sensor LDR, sensores NPK, sensor de pH, módulo relay
- **Banco de Dados**: Oracle SQL Developer para armazenamento e análise dos dados
- **Linguagens**: Python/C++ para programação dos sensores e análise de dados
- **Visualização**: Dashboard desenvolvido em Python (Streamlit/Dash)
- **Controle de Versão**: GitHub para gerenciamento do código fonte

## 🔧 Como executar o código

### Pré-requisitos
- Oracle SQL Developer instalado
- Python 3.8+ (para dashboard opcional)
- Acesso ao banco Oracle da FIAP (oracle.fiap.com.br)

### Configuração do Banco de Dados
1. Abra o Oracle SQL Developer
2. Crie nova conexão com as credenciais da FIAP:
   - Host: oracle.fiap.com.br
   - Porta: 1521
   - SID: ORCL
   - Usuário: Seu RM
   - Senha: Data de nascimento (DDMMYY)
3. Importe os dados do arquivo `assets/dados_historicos_2024.csv`
4. Execute as consultas SQL disponíveis em `scripts/`

### Dashboard (Opcional)
```bash
pip install streamlit pandas plotly
streamlit run src/dashboard.py
```

## 📊 Banco de Dados Oracle

### Estrutura da Tabela
O sistema utiliza uma tabela com os seguintes campos:
- `TIMESTAMP`: Marca temporal dos dados coletados
- `UMIDADE_DHT`: Umidade do ar capturada pelo sensor DHT
- `LDR_VALOR`: Valor do sensor de luminosidade
- `N_PRESENTE`, `P_PRESENTE`, `K_PRESENTE`: Presença dos nutrientes NPK
- `BLOQUEIO_EXTERNO`: Status de bloqueio externo do sistema
- `RELAY_STATUS`: Status do sistema de irrigação (0=desligado, 1=ligado)
- `UMIDADE_BAIXA`: Indicador de umidade baixa do solo
- `NPK_OK`: Status dos nutrientes NPK
- `PH_OK`: Status do pH do solo

## 🚀 Funcionalidades Implementadas

### Consultas SQL Desenvolvidas
1. **Análise de Umidade Baixa**: Identificação de períodos críticos
2. **Status da Irrigação**: Monitoramento do sistema de relay
3. **Dados Mais Recentes**: Consulta dos últimos registros
4. **Estatísticas de Ativação**: Contagem de ativações do sistema
5. **Média de Umidade**: Cálculos estatísticos dos dados

### Dashboard Interativo
- Visualização em tempo real dos níveis de umidade
- Gráficos de nutrientes P, K e pH
- Status visual do sistema de irrigação
- Sugestões baseadas em dados climáticos

## 🎥 Demonstração

[Link do vídeo de demonstração (YouTube - não listado)]

## 📚 Referências

- Oracle SQL Developer Documentation
- Python Streamlit Framework
- IoT Sensors Documentation
- FIAP - Curso de Tecnologia em IoT

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>


