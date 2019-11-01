# Análise de sentimento de tuítes

Código em R utilizado para matéria de 1º de novembro do Vortex Media.

Foram coletados 850.029 tuítes entre 17h04 do dia 29 de outubro de 2019 e 12h09 de 30 de outubro de 2019, resultantes da busca por “Bolsonaro” na [API do Twitter](https://help.twitter.com/pt/rules-and-policies/twitter-api), utilizando [este código](https://gist.github.com/voltdatalab/4b2351f5752e5f2b64c6978f53965a74). Destes, analisamos 749.625 (88%) que continham alguma menção direta no texto ao nome Bolsonaro.

O vocabulário dos tuítes foi comparado com dois léxicos da biblioteca [lexiconPT](https://cran.r-project.org/web/packages/lexiconPT/lexiconPT.pdf), que relaciona diferentes palavras do português com valores de sentimento positivo ou negativo atribuídos a elas. O algoritmo foi capaz de detectar o sentimento de 46% do total de tuítes mencionando Bolsonaro.

Como os léxicos podem atribuir valores diferentes a termos iguais, consideramos apenas os tuítes em que a diferença entre os valores não ultrapassa 5, para evitar dados conflitantes.
