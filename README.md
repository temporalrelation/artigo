# Identificação de Tipos de Relações Temporais *event-time* em Português com Abordagem Baseada em Regras

Neste artigo, apresentamos um método computacional para identificar tipos de relações temporais entre eventos e expressões temporais em textos em português. Utilizando uma abordagem baseada em regras e conjuntos de <i>features</i> relevantes, desenvolvemos conjuntos de regras utilizando algoritmos de aprendizagem de regras, além de regras manuais específicas para o idioma. Os experimentos no <i>corpus</i> TimeBankPT[^timebankpt] demonstraram a eficácia do nosso método, superando o <i>baseline</i>[^baseline] em termos de acurácia e <i>F1-score</i>. Esta pesquisa apresenta aplicações práticas no campo do resumo de documentos, compreensão de histórias e análise de notícias. Por meio do uso de regras explicáveis, possibilita uma compreensão aprimorada do tempo em textos.


# Conjunto de <i>Features</i>
Apresentamos nosso [Conjunto de *Features*](conjunto_de_features.md) organizadas por tipo de informações linguísticas.


# Conjuntos de Regras
Apresentamos nossos [Conjuntos de Regras](rules) desenvolvidos para a tarefa de identificar tipos de relações temporais entre evento e expressão temporal em textos em português.

Cada regra possui o seguinte formato:

> *[código da regra, 'TIPO DA RELAÇÃO TEMPORAL', ordem da regra, "expressão lógica que representa a regra", 'algoritmo de origem', acurácia, total de acertos, número de vezes que foi acionada]*

A expressão lógica que representa a regra é composta por conjunções de condições. Cada condição é constituída por uma *`feature`* de nosso [conjunto de *features*](conjunto_de_features.md), um `operador`, que pode ser de igualdade ou desigualdade, e o `valor` da *feature*.


# Referências

[^timebankpt]: COSTA, Francisco; BRANCO, António. TimeBankPT: A TimeML Annotated Corpus of Portuguese. In: LREC. 2012. p. 3727-3734.
[^baseline]: COSTA, Francisco Nuno Quintiliano Mendonça Carapeto. Processing Temporal Information in Unstructured Documents. 2012. Tese de Doutorado. Universidade de Lisboa (Portugal).
