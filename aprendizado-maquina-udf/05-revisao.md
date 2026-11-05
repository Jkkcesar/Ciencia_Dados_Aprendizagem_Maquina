<img src="assets/logo-udf.jpg" alt="UDF Centro Universitário" width="230">

**Profa. Kadidja Valéria | UDF**  
Ciência de Dados e Aprendizado de Máquina · Sistemas de Informação · 2026.2

# Questões de revisão — Registro individual

## Identificação

- Estudante ou equipe: **Julio César de Aguiar Nunes**
- Turma: **Sistemas de Informação - 2026.2**
- Data de realização: **30/10/2026**
- Integrantes e contribuições (se em equipe): **Julio César de Aguiar Nunes**

Responda com suas palavras e apresente os cálculos quando solicitados. Os números dos exercícios manuais não são os resultados do laboratório.

## 1. Explique a diferença entre regra programada para bloquear uma palavra e modelo de spam treinado com exemplos.

**Resposta:** Uma regra programada aplica uma condição explícita, definida por uma pessoa, como bloquear mensagens que contenham determinada palavra. Ela não se adapta por conta própria a novos padrões. Um modelo de aprendizado de máquina é treinado com exemplos rotulados como spam ou legítimos e aprende combinações de características que ajudam a classificar novas mensagens. Seus resultados dependem da qualidade e da representatividade dos exemplos.

## 2. Por que codificar evadiu/permaneceu como 1/0 não transforma classificação em regressão?

**Resposta:** Os valores 1 e 0 representam duas classes distintas, não quantidades contínuas. A tarefa continua sendo classificação porque o objetivo é atribuir uma categoria — evadiu ou permaneceu — e não estimar uma medida numérica cuja distância entre valores tenha significado.

## 3. Uma biblioteca quer estimar empréstimos e descobrir perfis. Que tarefas correspondem a cada pergunta?

**Resposta:** Estimar o número de empréstimos é **regressão**, uma tarefa supervisionada, pois o alvo é numérico. Descobrir perfis sem categorias previamente definidas é **agrupamento (clustering)**, uma tarefa não supervisionada que procura grupos de observações semelhantes.

## 4. O que são atributo, alvo e unidade de análise no laboratório educacional?

**Resposta:**
- **Unidade de análise:** cada estudante representado por um registro.
- **Atributos:** características usadas para fazer a previsão, como frequência, nota e entregas até a semana 4.
- **Alvo:** o resultado que se deseja prever; no laboratório, `evasao_fim_semestre` (0 = permaneceu, 1 = evadiu).

## 5. Por que calcular a mediana antes de dividir os dados pode invalidar a avaliação?

**Resposta:** Calcular a mediana usando todos os dados incorpora informação da distribuição do teste na preparação do treino, causando vazamento de dados (*data leakage*) e podendo tornar a avaliação otimista. Primeiro se separa treino e teste; o imputador é ajustado apenas no treino. Na validação cruzada, ele deve ser ajustado dentro de cada *fold*, por exemplo, mantendo a imputação e o modelo juntos em um `Pipeline`.

## 6. Em uma matriz didática com TN=80, FP=5, FN=10, TP=5, calcule acurácia e sensibilidade. O resultado é suficiente para aprovar o modelo?

**Resposta:**
- **Total:** 80 + 5 + 10 + 5 = 100 amostras.
- **Acurácia:** (TP + TN) / Total = (5 + 80) / 100 = **85%**.
- **Sensibilidade (recall):** TP / (TP + FN) = 5 / (5 + 10) = 5 / 15 = **33,3%**.

**Conclusão:** A acurácia isolada não é suficiente para aprovar o modelo. A sensibilidade indica que ele identifica apenas 5 dos 15 casos positivos e deixa passar 10 (66,7%). Se a classe positiva representa estudantes em risco, essa taxa de falsos negativos pode ser especialmente preocupante.

## 7. Valores reais 100, 120, 140 e previsões 110, 115, 130. Calcule MAE e informe a unidade se o alvo for vendas em reais.

**Resposta:**
- Erros absolutos: |100 - 110| = 10; |120 - 115| = 5; |140 - 130| = 10.
- **MAE:** (10 + 5 + 10) / 3 = 25 / 3 ≈ **8,33**.
- Como o alvo está em reais, o MAE é **R$ 8,33**. A unidade do erro é a mesma do alvo.

## 8. Um R² de -0,2 significa “20% de acertos negativos”? Explique.

**Resposta:** Não. R² não é uma porcentagem de acertos. Ele compara o erro quadrático do modelo com o erro de uma referência que prevê a média do alvo. Um R² negativo significa que, nessa avaliação, o modelo teve erro quadrático maior do que essa referência; portanto, prever a média teria sido melhor. O valor -0,2 não significa “20% de acertos negativos”.

## 9. Uma árvore tem acurácia 1,00 no treino e 0,65 na validação. Que hipótese investigar e como?

**Resposta:** A diferença sugere **sobreajuste (*overfitting*)**: a árvore pode ter aprendido detalhes específicos do treino que não se repetem em dados novos. Investigaria a profundidade máxima e o tamanho mínimo das folhas, comparando configurações com validação feita apenas no treino. A escolha deve se apoiar no desempenho de validação, não no teste.

## 10. Por que escolher a profundidade pelo teste prejudica a estimativa final?

**Resposta:** Se a profundidade for escolhida com base nos resultados do teste, esses resultados influenciam uma decisão sobre o modelo. O teste deixa de ser uma avaliação independente e a estimativa final pode ficar otimista. A profundidade deve ser escolhida com treino e validação; o teste fica reservado para uma avaliação final.

## 11. Baixa frequência associada à evasão demonstra causa? Proponha explicação alternativa.

**Resposta:** Não. A associação observada demonstra correlação, não necessariamente causalidade. Uma explicação alternativa é que uma mudança no horário de trabalho reduza a frequência e também torne difícil continuar no curso. Nesse caso, a condição de trabalho pode contribuir para os dois acontecimentos, sem que a baixa frequência, por si só, prove a causa da evasão.

## 12. Um modelo sinaliza um estudante como possível evasão. Que ação responsável pode ser adotada?

**Resposta:** Um profissional pode verificar o sinal e convidar o estudante, de forma respeitosa e voluntária, para conversar sobre apoio acadêmico ou outros recursos disponíveis. A previsão deve ser tratada como incerta, nunca como motivo para punição ou decisão automática. A equipe deve explicar o uso dos dados de forma apropriada, proteger a privacidade e oferecer ao estudante meios de corrigir informações ou contestar uma avaliação.

## Fontes adicionais consultadas

**Material didático da Unidade 4 — Ciência de Dados e Aprendizado de Máquina, UDF; registros das atividades de laboratório e do PBL integrador.**

[Voltar ao início](README.md).
