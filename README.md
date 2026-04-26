# Análise de Performance de Produção Pós Retrofit ⚙📈🐍

**Objetivo:** Avaliar a estabilidade e desempenho de uma máquina injetora após o retrofit, utilizando indicadores estatísticos e de produtividade.

## Desenvolvimento
- Gerar Dados com Numpy
  - Gerar dados simulados de tempo de ciclo com valores aleatórios reprodutíveis;
  - **Variação:** Entre 20 e 45 segundos;
  - **Amostra:** A média de tempo de ciclo diário dos últimos 30 dias
 
- Produtividade
  - Analisar média e mediana do tempo de ciclo em relação ao tempo esperado;
  - Calcular a produtividade real (pçs/h) e comparar com a produtividade esperada;
  - Avaliar a variação de produtividade (%).
  - Verificar conformidade dos ciclos em relação à meta (dias fora do esperado).
 
- Variabilidade do Processo
  - Calcular o coeficiente de variação e classificar;
  - Identificar outliers (anomalias).
 
- Visualização Gráfica
  - Calcular os limites de controle (UCL e LCL) com base no CEP;
  - Plotar gráfico de controle para visualizar a variação e estabilidade do processo.
 
## Conclusão
Após o retrofit da injetora, os dados coletados ao longo de 30 dias indicam que:

- O tempo médio de ciclo ficou em **33,8 s**, **3,8 s** acima da meta de 30 segundos.
- Isso representa uma perda de produtividade de aproximadamente **11,2%**, com produção média de **107** peças/hora, contra as 120 esperadas peças/hora.
- Dos 30 dias analisados, **22 dias (73%)** performaram fora do estabelecido, indicando recorrência do desvio.
- O coeficiente de variação indica um processo com **alta variabilidade (instável)**.
- Não foram identificadas anomalias relevantes (pontos fora de controle), sugerindo ausência de causas especiais.
- No gráfico de controle, é observado variações consistentes ao longo do período, reforçando que o processo apresenta **variabilidade contínua**, e não desvios pontuais.
- O processo encontra-se estável do ponto de vista estatístico (sem causas especiais), porém desalinhado com a meta de desempenho, indicando necessidade de ajustes no processo para redução do tempo de ciclo.
---
# TECNOLOGIAS USADAS
- Jupyter Notebook: 7.2.2
- Python: 3.12.7
  - Numpy:  1.26.4
  - Matplotlib: 3.9.2   

## Instalação das bibliotecas
```bash
pip install numpy
pip install matplotlib
```
