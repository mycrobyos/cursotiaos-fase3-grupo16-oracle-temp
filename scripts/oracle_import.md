# Guia Completo: Configuração e Importação Oracle SQL Developer



## 🔧 Passo a Passo da Configuração

### Etapa 1: Login e Conexão
![Login Oracle](../assets/import/01_login.png)

### Etapa 2: Processo de Importação
![Importação](../assets/import/02_importacao.png)

### Etapa 3: Configuração da Importação (1/5)
![Importação 1 de 5](../assets/import/03_importacao1de5.png)

### Etapa 4: Definição da Tabela (2/5)
![Importação 2 de 5](../assets/import/04_importacao2de5.png)

### Etapa 5: Mapeamento de Colunas (3/5)
![Importação 3 de 5](../assets/import/05_importacao3de5.png)

#### TIMESTAMP
![Timestamp Config](../assets/import/06_importacao4de5_timestamp.png)

#### UMIDADE_DHT  
![Umidade Config](../assets/import/07_importacao4de5_umidade.png)

#### LDR_VALOR
![LDR Config](../assets/import/08_importacao4de5_ldr.png)

#### Nutrientes N, P, K
![NPK Config](../assets/import/09_importacao4de5_np.png)

#### Status e Indicadores
![Status Config](../assets/import/12_importacao4de5_bloqueio.png)
- BLOQUEIO_EXTERNO: NUMBER(1,0)
- RELAY_STATUS: NUMBER(1,0)  
- UMIDADE_BAIXA: NUMBER(1,0)
- NPK_OK: NUMBER(1,0)
- PH_OK: NUMBER(1,0)

### Etapa 6: Revisão Final
![Revisão](../assets/import/17_revisao.png)

### Etapa 7: Importação Concluída
![Finalizada](../assets/import/18_finalizada.png)

## ✅ Verificação dos Dados

### Visualizar Estrutura da Tabela
![Tabela](../assets/import/19_tabela.png)

### Consulta Completa dos Dados
![Select All](../assets/import/20_select_all.png)

![Resultado Select](../assets/import/21_select_all_result.png)

## 🚨 Troubleshooting

### Problemas Comuns

1. **Erro de Conexão**
   - Verifique credenciais FIAP
   - Confirme conectividade de rede
   - Teste novamente a conexão

2. **Erro na Importação**
   - Verifique formato do arquivo CSV
   - Confirme delimitadores
   - Revise tipos de dados das colunas

3. **Tabela não Criada**
   - Verifique permissões do usuário
   - Confirme nome da tabela (sem caracteres especiais)
   - Tente recriar com nome diferente

### Dicas Importantes

- ⚠️ Nome da tabela: máximo 30 caracteres, sem espaços
- ⚠️ Sempre teste a conexão antes de importar
- ⚠️ Faça backup dos dados antes de modificações
- ⚠️ Verifique tipos de dados adequados para cada coluna

## 📊 Próximos Passos

Após importação bem-sucedida:
1. Execute consultas de análise (ver `consultas_analise.sql`)
2. Explore os dados com diferentes filtros
3. Desenvolva dashboard para visualização
4. Documente insights encontrados