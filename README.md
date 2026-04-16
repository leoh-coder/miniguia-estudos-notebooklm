# 📚 Miniguia de Educação Financeira Pessoal com NotebookLM

> Projeto desenvolvido como parte do **Bootcamp Bradesco - GenAI & Dados** na plataforma [DIO](https://www.dio.me/), utilizando o [NotebookLM](https://notebooklm.google.com/) como ferramenta de aprendizagem ativa com Inteligência Artificial Generativa.

---

## 🎯 Contexto e Objetivos

**Assunto escolhido:** Educação Financeira Pessoal — com foco em conceitos introdutórios de orçamento, investimento e planejamento financeiro.

**Por que esse tema?**
A educação financeira é uma das competências mais importantes para autonomia e qualidade de vida, porém ainda pouco difundida de forma acessível no Brasil. Estudar o tema com apoio de IA Generativa permite construir um material de consulta personalizado, com linguagem clara e resumos objetivos.

**Objetivos de estudo com este caderno:**
- Compreender os fundamentos do orçamento pessoal (receitas, despesas, reserva de emergência)
- Entender a diferença entre renda fixa e renda variável
- Aprender o conceito de juros compostos e sua influência no longo prazo
- Identificar os principais tipos de investimento acessíveis ao investidor iniciante
- Construir um vocabulário financeiro básico e funcional

---

## 📂 Curadoria de Fontes

As fontes abaixo foram selecionadas por serem abertas, gratuitas, em português e de instituições confiáveis. Todas foram inseridas no NotebookLM via upload de PDF ou link direto.

| # | Fonte | Tipo | Link |
|---|-------|------|------|
| 1 | **Banco Central do Brasil — Caderno de Educação Financeira** | PDF gratuito | [bcb.gov.br](https://www.bcb.gov.br/content/cidadaniafinanceira/documentos_cidadania/Cuidando_do_seu_dinheiro_Gestao_de_Financas_Pessoais/caderno_cidadania_financeira.pdf) |
| 2 | **CVM — Guia do Investidor Iniciante** | PDF gratuito | [investidor.gov.br](https://www.investidor.gov.br/publicacao/download/GuiaDoInvestidor.pdf) |
| 3 | **Tesouro Nacional — Tesouro Direto: como funciona** | Texto/Web | [tesourodireto.com.br](https://www.tesourodireto.com.br/conheca/como-funciona.htm) |
| 4 | **ENEF — Estratégia Nacional de Educação Financeira** | PDF gratuito | [vidaedinheiro.gov.br](https://www.vidaedinheiro.gov.br/wp-content/uploads/2017/08/Plano-Diretor-ENEF.pdf) |
| 5 | **Serasa — Guia de Orçamento Pessoal** | Texto/Web | [serasa.com.br/ensina](https://www.serasa.com.br/ensina/dicas/orcamento-pessoal/) |

---

## 🧠 Engenharia de Prompts e Cicatrizes

Abaixo estão os prompts estratégicos testados no NotebookLM, as variações aplicadas e os aprendizados de cada iteração.

---

### Prompt 1 — Definição de conceito
**Objetivo:** Obter uma definição clara e acessível de juros compostos.

```
Explique o conceito de juros compostos de forma simples, como se estivesse explicando para alguém que nunca estudou finanças. Use um exemplo numérico com R$ 1.000,00 aplicados por 12 meses.
```

**Resposta obtida (resumo):** O NotebookLM explicou que juros compostos são "juros sobre juros", onde o rendimento de cada período é somado ao capital e serve de base para o cálculo seguinte. Com R$ 1.000,00 a 1% ao mês, após 12 meses o valor seria de aproximadamente R$ 1.126,83 — diferente dos juros simples, que resultariam em exatamente R$ 1.120,00.

**Cicatriz:** A primeira versão do prompt não incluía o exemplo numérico e a resposta ficou muito abstrata. Ao adicionar "use um exemplo numérico", a resposta ficou mais didática e concreta.

---

### Prompt 2 — Comparação entre conceitos
**Objetivo:** Diferenciar renda fixa de renda variável de forma clara.

```
Com base nas fontes disponíveis, compare renda fixa e renda variável destacando: risco, retorno esperado e perfil de investidor mais adequado para cada uma. Organize em formato de tabela.
```

**Resposta obtida (resumo):** O modelo gerou uma tabela comparativa apontando que renda fixa oferece previsibilidade e menor risco (adequada ao perfil conservador), enquanto a renda variável apresenta maior potencial de retorno associado a maior volatilidade (adequada ao perfil arrojado). A CVM e o Banco Central foram citados como fontes.

**Cicatriz:** Pedir "organize em formato de tabela" foi determinante — sem essa instrução, a resposta vinha em texto corrido e era mais difícil de comparar visualmente.

---

### Prompt 3 — Geração de glossário
**Objetivo:** Extrair os principais termos técnicos do material.

```
Liste os 10 termos financeiros mais importantes presentes nas fontes e defina cada um em no máximo 2 linhas, em linguagem acessível para iniciantes.
```

**Resposta obtida (resumo):** O NotebookLM gerou um glossário com termos como liquidez, volatilidade, rentabilidade, selic, diversificação, aporte, carteira, benchmark, inflação e reserva de emergência — todos com definições curtas e claras.

**Cicatriz:** Limitar a "no máximo 2 linhas" foi essencial. Sem esse limite, as definições ficavam longas demais e perdiam a utilidade como glossário de consulta rápida.

---

### Prompt 4 — Criação de plano de ação
**Objetivo:** Transformar o conhecimento em algo aplicável.

```
Com base no conteúdo das fontes, crie um passo a passo simples para uma pessoa que ganha R$ 3.000,00 por mês e quer começar a organizar suas finanças do zero. Liste no máximo 5 passos práticos.
```

**Resposta obtida (resumo):** O modelo sugeriu: (1) mapear todas as receitas e despesas, (2) criar um orçamento com a regra 50-30-20, (3) montar uma reserva de emergência de 3 a 6 meses de despesas, (4) quitar dívidas com juros altos antes de investir, (5) começar a investir em renda fixa com valores pequenos (ex: Tesouro Selic).

**Cicatriz:** A instrução "no máximo 5 passos" forçou o modelo a priorizar o que é realmente essencial, evitando uma lista genérica e extensa.

---

## 📖 Miniguia de Estudo

### Resumos Estruturados

**Orçamento Pessoal**
O orçamento é o mapa das finanças pessoais. A regra mais usada é a 50-30-20: 50% da renda para necessidades, 30% para desejos e 20% para poupança/investimentos. O primeiro passo é sempre registrar todas as entradas e saídas por pelo menos um mês.

**Reserva de Emergência**
Valor guardado em investimento de alta liquidez (como Tesouro Selic ou CDB com liquidez diária) equivalente a 3 a 6 meses das despesas mensais. É o alicerce de qualquer planejamento financeiro — sem ela, qualquer imprevisto vira dívida.

**Juros Compostos**
Considerados a "oitava maravilha do mundo" por Einstein, os juros compostos fazem o dinheiro crescer de forma exponencial ao longo do tempo. Quanto antes se começa a investir, maior o efeito do tempo sobre o capital.

**Renda Fixa vs. Renda Variável**
Renda fixa (Tesouro Direto, CDB, LCI/LCA) oferece previsibilidade e é indicada para reserva de emergência e objetivos de curto/médio prazo. Renda variável (ações, FIIs) tem maior potencial de retorno no longo prazo, mas exige maior tolerância à volatilidade.

---

### Glossário de Conceitos

| Termo | Definição |
|-------|-----------|
| **Liquidez** | Facilidade de transformar um investimento em dinheiro sem perda de valor |
| **Volatilidade** | Variação do preço de um ativo ao longo do tempo |
| **Rentabilidade** | Ganho percentual obtido sobre um investimento |
| **Selic** | Taxa básica de juros da economia brasileira, definida pelo Banco Central |
| **Diversificação** | Distribuir investimentos em diferentes ativos para reduzir riscos |
| **Aporte** | Valor depositado periodicamente em um investimento |
| **Carteira** | Conjunto de todos os investimentos de uma pessoa |
| **Benchmark** | Indicador de referência usado para comparar a performance de um investimento |
| **Inflação** | Aumento generalizado dos preços que reduz o poder de compra da moeda |
| **Reserva de emergência** | Valor guardado para cobrir imprevistos sem precisar contrair dívidas |

---

### Prompts Reutilizáveis

Estes prompts podem ser usados em qualquer sessão futura de estudo no NotebookLM sobre finanças pessoais:

```
1. "Explique [conceito] de forma simples com um exemplo prático em reais."

2. "Compare [conceito A] e [conceito B] em formato de tabela com os critérios: risco, retorno, liquidez e perfil indicado."

3. "Liste os [N] termos mais importantes sobre [tema] e defina cada um em no máximo 2 linhas."

4. "Crie um passo a passo prático para [objetivo financeiro] com no máximo 5 etapas claras e acionáveis."

5. "Com base nas fontes, quais são os erros mais comuns que iniciantes cometem ao [ação financeira]? Liste os 3 principais."

6. "Resuma os principais pontos de [fonte específica] em tópicos. Destaque o que é mais relevante para quem está começando."
```

---

## 🛠️ Tecnologias Utilizadas

- **[NotebookLM](https://notebooklm.google.com/)** — Google (IA Generativa para aprendizagem ativa)
- **GitHub** — versionamento e publicação do material

---

## 👨‍💻 Autor

**Leonardo Henrique Ramos Ferreira**
[LinkedIn](https://linkedin.com/in/seu-perfil) | [GitHub](https://github.com/seu-usuario)

---

*Projeto desenvolvido durante o Bootcamp Bradesco - GenAI & Dados · DIO · 2025*
