# iX Mobile Banking Prediction Challenge

## (Notebook com códigos e visualizações)[https://github.com/gxbriellops/ix-mobile-banking/blob/main/analise.ipynb]

## Análise Exploratória de Dados

### Introdução

Este repositório contém a análise exploratória para a competição "iX Mobile Banking Prediction Challenge" da Zindi. O objetivo é identificar fatores que influenciam a adoção de serviços financeiros móveis e encontrar oportunidades para inclusão financeira.

### Panorama dos Dados

**Estrutura do Dataset**:
- 108.446 registros
- 42 variáveis (informações demográficas, comportamentos financeiros, variável alvo)
- Variável Target: uso de serviços financeiros via internet (0/1)

**Valores Faltantes**:
- 15 variáveis têm mais de 40% de valores ausentes
- Variáveis mais incompletas: FQ31 (99.20%), FQ28 (98.61%), FQ30 (98.05%)

### Resultados Principais

#### Adoção de Serviços Financeiros Digitais

1. **Baixa penetração digital**: Apenas 27,5% dos entrevistados usam serviços financeiros digitais
   ```
   Target=0 (não usam): 78.735 pessoas (72,5%)
   Target=1 (usam): 29.711 pessoas (27,5%)
   ```

2. **Conta bancária não determina uso digital**: Ter conta bancária não aumenta a probabilidade de uso de serviços digitais
   ```
   Probabilidade de uso online:
   - Com conta bancária: 27,38%
   - Sem conta bancária: 27,43%
   ```

3. **Idade não é fator discriminante**:
   ```
   Perfil de idade dos usuários:
   - Média: 41,81 anos (vs. 41,86 na população total)
   - Mediana: 39,0 anos (igual à população total)
   ```

#### Comportamentos Financeiros

4. **Acesso limitado a serviços financeiros básicos**:
   ```
   Uso de caixas eletrônicos (FQ1):
   - Categoria 1: 48.896 (45,1%)
   - Categoria 2: 58.373 (53,8%)
   - Categorias 3+4: <2% combinadas
   ```

5. **Contraste entre tipos de poupança**:
   ```
   Poupança para negócios (FQ7):
   - Categoria 1: ~48.000 (79,2%)
   - Categoria 2: ~11.000 (18,1%)

   Poupança para velhice (FQ9):
   - Categoria 1: ~23.000 (21,2%)
   - Categoria 2: ~83.000 (76,5%)
   ```

#### Habilitadores de Inclusão Financeira

6. **Posse de celular e ID são necessários mas não suficientes**:
   ```
   Entre pessoas com ID nacional:
   - ~27% usam serviços financeiros online
   - ~73% não usam apesar de possuírem documentação
   ```

### Hipóteses Principais

1. **Hipótese de Infraestrutura Limitada**: Taxa similar de adoção entre pessoas com/sem conta bancária sugere limitações de infraestrutura digital.

2. **Hipótese de Confiança e Educação Financeira**: Fatores comportamentais parecem mais determinantes que acesso físico.

3. **Hierarquia de Necessidades Financeiras**: Operações básicas (saques) são mais adotadas que serviços avançados (crédito).

4. **Capital de Giro vs. Capital de Reserva**: Priorização de acesso imediato a capital para negócios versus poupança de longo prazo.

### Recomendações Estratégicas

1. **Pacotes de Inclusão Digital-Financeira**: Programas que conectem IDs, celulares e serviços financeiros.

2. **Produtos Financeiros para Empreendedorismo**: Desenvolver soluções voltadas para microempreendedores.

3. **Educação Financeira Digital**: Reduzir gap entre posse de tecnologia e uso de serviços financeiros.

4. **Modelos Alternativos**: Explorar alternativas ao modelo bancário tradicional.

### Próximos Passos

- Análise multivariada para identificar combinações de fatores preditivos
- Investigar variáveis geográficas na adoção
- Modelo preditivo considerando desbalanceamento da variável alvo
- Segmentação de clientes via análise de clusters

### Tecnologias Utilizadas

- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook
