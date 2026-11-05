<img src="assets/logo-udf.jpg" alt="UDF Centro Universitário" width="230">

**Profa. Kadidja Valéria | UDF**  
Ciência de Dados e Aprendizado de Máquina · Sistemas de Informação · 2026.2

# Autoavaliação e conferência da entrega

## Identificação

- Estudante ou equipe: **Julio César de Aguiar Nunes**
- Turma: **Sistemas de Informação - 2026.2**
- Data de realização: **30/10/2026**
- Integrantes e contribuições (se em equipe): **Julio César de Aguiar Nunes**

## Checklist

- [ ] Diferenciei explicitamente IA, Ciência de Dados e ML com um exemplo; as respostas registradas abordam ML, mas não comparam as três áreas.
- [X] Completei o quadro supervisionado/não supervisionado.
- [X] Justifiquei pelo menos cinco situações-problema.
- [X] Registrei a investigação da biblioteca.
- [X] Identifiquei atributos, alvo, unidade e momento da previsão.
- [X] Executei e documentei a prática em Python/Colab.
- [X] Escolhi configurações usando treino/validação.
- [X] Mantive o teste fora do ajuste e da seleção.
- [X] Interpretei acurácia, matriz de confusão, MAE e R².
- [X] Comparei com uma referência e discuti erros.
- [X] Registrei limitações dos dados sintéticos, privacidade e possíveis vieses.
- [X] Formulei recomendações de apoio com revisão humana.
- [X] Respondi às questões individuais.
- [ ] Confirmei todos os links e arquivos de evidências; o registro do PBL aponta para um notebook cujo caminho ainda precisa ser conferido.
- [X] Substituí os campos PREENCHER ou justifiquei os não aplicáveis.

## Reflexão individual

- O que aprendi e consigo explicar: **Aprendi a diferenciar classificação e regressão pelo tipo de alvo, a comparar modelos com uma referência simples e a interpretar por que a acurácia, sozinha, pode esconder casos de evasão não identificados. Também consigo explicar o papel do `Pipeline` e da validação cruzada para evitar vazamento de dados durante a imputação e a seleção de hiperparâmetros.**
- Qual foi minha principal dificuldade: **Interpretar R² sem tratá-lo como porcentagem de acertos e manter a separação correta entre treino, validação e teste, especialmente durante a validação cruzada.**
- Qual evidência mostra meu avanço: **No laboratório, registrei a seleção de `max_depth=5` pela validação cruzada (acurácia média de 0,7222), a acurácia de teste de 78% e a sensibilidade de 68,85%, além de interpretar os falsos positivos e negativos. No PBL integrador, considerei o custo maior dos falsos negativos e propus uma intervenção voluntária com revisão humana. O registro de regressão, porém, apresenta MAE de 1,2 e R² de 0,75, enquanto a saída do notebook foi anotada como MAE de 28,59 e R² de 0,8774; esses valores não estão conciliados e não os trato como uma evidência única.**
- Como contribuí com a equipe: **Contribuí com a definição técnica dos atributos, do alvo e das métricas no PBL Biblioteca em Foco. No PBL integrador, registrei a construção do pipeline e a modelagem, a interpretação das métricas e a análise de limitações, vieses, privacidade e apoio aos estudantes.**
- O que preciso revisar: **Preciso conciliar os resultados de regressão entre o relatório e a saída do notebook antes de apresentar um resultado definitivo. Também quero aprofundar aprendizado não supervisionado, como agrupamento (*clustering*), e formas de ajustar hiperparâmetros sem comprometer a avaliação final.**
- Ferramentas de apoio utilizadas, incluindo IA quando houver, e como verifiquei as respostas: **Utilizei o Google Colab para executar Python, a documentação do Scikit-Learn e o Gemini como apoio de estudo e formatação. Verifiquei os conceitos com o material didático e confrontei as métricas registradas com as saídas disponíveis no notebook; a divergência dos resultados de regressão ficou explicitamente registrada para conferência.**

## Critérios de avaliação

Escala sugerida do material: nível 3 consistente, 2 adequado com lacunas, 1 parcial, 0 ausente/incoerente. Nota do critério = peso × nível/3. A professora pode ajustar a aplicação.

| Critério | Peso aula 1 | Peso aula 2/PBL |
| --- | --- | --- |
| Problema e conceitos | 3,0 | 2,0 |
| Dados e justificativa | 2,0 | 2,0 |
| Método e avaliação | 1,0 | 3,0 |
| Interpretação e responsabilidade | 2,0 | 2,0 |
| Clareza e colaboração | 2,0 | 1,0 |
| Total | 10,0 | 10,0 |

Na aula 1, método corresponde à avaliação proposta. Na aula 2, inclui execução e interpretação. A maior acurácia isolada não assegura a melhor avaliação da atividade.

## Fontes de apoio

- SCIKIT-LEARN. *User Guide*. https://scikit-learn.org/stable/user_guide.html.
- SCIKIT-LEARN. *Common pitfalls and recommended practices*. https://scikit-learn.org/stable/common_pitfalls.html.
- ORANGE DATA MINING. *Test and Score*. https://orangedatamining.com/widget-catalog/evaluate/testandscore/.

Referências indicadas no material didático do módulo, consultadas em 14 out. 2026. Registre a data da sua própria consulta quando utilizar novas fontes.

[Voltar ao início](README.md).
