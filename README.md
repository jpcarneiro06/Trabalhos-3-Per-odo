# Portfólio de Projetos em Estatística — Renda e Escolaridade (PNAD Contínua)

## Sobre os projetos
Os dois trabalhos abaixo foram desenvolvidos na disciplina Estatística Computacional, utilizando dados da PNAD Contínua (IBGE) para o estado do Rio de Janeiro, com foco na relação entre escolaridade e rendimento. O segundo trabalho dá continuidade direta à base e às análises do primeiro, avançando de estatística descritiva para modelos de inferência mais sofisticados e séries temporais.

---

## Projeto 1 — Análise de Rendimento por Anos de Estudo

### Objetivos
1. **Análise de Rendimento por Anos de Estudo**
   Verificar se há diferença no rendimento entre três grupos de escolaridade na UF do RJ:
   - Até 9 anos de estudo
   - Entre 10 e 12 anos de estudo
   - 13 anos de estudo ou mais

2. **Análise Inferencial e Testes de Hipótese**
   Aplicar uma ANOVA para testar se as diferenças observadas entre os grupos são estatisticamente significativas, relacionando os resultados com o que os box-plots sugerem visualmente.

3. **Análises Adicionais**
   Investigar diferenças de rendimento por gênero e por faixa etária (≤ 25, 26–35, 36–50, > 50 anos).

### Metodologia
- Estatística descritiva: número de observações, rendimento médio e desvio padrão por grupo, com box-plots comparativos.
- Estatística inferencial: ANOVA, discutindo a diferença entre o que a análise descritiva sugere e o que o teste formal confirma.
- Análises complementares segmentando por gênero e faixa etária.

---

## Projeto 2 — Inferência Estatística e Séries Temporais

### Estrutura

**Parte 1 — Complemento da Análise Descritiva**
Extensão da análise por gênero e faixa etária iniciada no Projeto 1.

**Parte 2 — Inferência Cross-Section: Regressão Linear Simples**
- Teste de independência entre renda e escolaridade via tabela de contingência.
- Regressão linear simples relacionando rendimento e escolaridade, respondendo ao impacto esperado de um ano a mais de escolaridade sobre a renda e à renda esperada para uma pessoa com 9 anos de escolaridade.
- Diagnóstico de resíduos (homoscedasticidade, normalidade e ausência de autocorrelação).

**Parte 3 — Modelos Log-Nível e Regressão Múltipla**
- Transformação log do modelo da Parte 2 para corrigir heterocedasticidade e não-normalidade, respondendo ao impacto percentual de um ano a mais de escolaridade sobre a renda.
- Nova análise de resíduos e comparação com o modelo original.
- Extensão para regressão múltipla, incluindo gênero e faixa etária como variáveis explicativas, comparando com o modelo simples.

**Parte 4 — Séries Temporais**
- Decomposição de uma série temporal em tendência e sazonalidade (aditiva ou multiplicativa, com justificativa).
- Previsão da série escolhida para um horizonte de 12 meses, com avaliação de acurácia no período de validação.

### Metodologia e Ferramentas
- R (RMarkdown), com testes de independência (qui-quadrado), regressão linear simples e múltipla (`lm()`), modelos log-nível, diagnóstico de resíduos (homoscedasticidade, normalidade, autocorrelação) e decomposição/previsão de séries temporais.

---

## Observações
Código-fonte (RMarkdown) não disponibilizado nesta versão do portfólio. Os arquivos em PDF neste repositório correspondem aos relatórios finais entregues nas respectivas disciplinas, contendo a análise completa e o script utilizado.
