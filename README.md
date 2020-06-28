# CLUSTERIZAR-INPE

INSTITUTO FEDERAL DO CEARÁ.

CURSO DE LICENCIATURA EM GEOGRAFIA. 

AUTOR - MARCELO CLARO LARANJEIRA.

ORIENTADOR PROF. MAILTON NOGUEIRA.

Data de início dos trabalhos 12/02/2020.

O ESTUDO PRESENTE, USANDO LINGUAGENS DO PYTHON E APRENDIZAGEM DE MÁQUINA, PARA DETERMINAR CORES DOMINANTES DE IMAGENS DO SATÉLITE, CATEGORIZAR-LAS E QUANTIFICAR-LAS EM PORCENTAGEM,  COM TÉCNICA EM MACHINE LEARNING NÃO SUPERVISIONADA. TAIS RESULTADOS PERMITEM ANALISAR COM MAIS CLAREZA A NATUREZA DAS TONALIDADES E SUA REPRESENTATIVIDADE QUANTITATIVA NESSE ESPAÇO FOTOGRAFADO. PODENDO SERVIR PARA MONITORAR A COBERTURA VEGETAL, SUA DIMINUIÇÃO E AUMENTO EM UM PERÍODO SANZONAL.

Sendo um projeto simples para demonstrar o uso de métodos de aprendizado de máquina não supervisionados (agrupando com o KMeans do scikit-learn ) para extrair cores das imagens, especificamente os produzidos pelo satélite LANDSAT8, com o intuito de monitorizar áreas de cobertura vegetal da microregião do Sertão de Crateús/CE.


A pesquisa tem como meta de cunho didático e inclusivo para pessoas com acuidade visual comprometida ou limitada, sendo possível, analises feitas por inteligência artificial, tendo em vista as cores da imagens do satélite, categorizando-as e agrupando em porcentagem, para que o discente, possa fazer suas interpretações por base númerica (vocalizada ou não), sem a necessidade das cognição física visual das cores para o mesmo. E introduzir as ciências humanas, principalmente a geográfica, aos patamares tecnológicos atualizados do mercado e da sociedade. 

INTRODUÇÃO CÓDIGO

Aprendizado de máquina com Python - Noções básicas.

Estamos vivendo na 'era dos dados' que é enriquecida com melhor poder computacional e mais recursos de armazenamento. Esses dados ou informações estão aumentando dia a dia, mas o verdadeiro desafio é entender todos os dados. Empresas e organizações estão tentando lidar com isso criando sistemas inteligentes usando os conceitos e metodologias da ciência de dados, mineração de dados e aprendizado de máquina. Entre eles, o aprendizado de máquina é o campo mais emocionante da ciência da computação. Não seria errado chamarmos o aprendizado de máquina de aplicação e ciência de algoritmos que dão sentido aos dados.

Neste projeto, mostrarei como usar o OpenCV, Python e o algoritmo de agrupamento k-means para encontrar as cores mais dominantes em uma imagem.

Então, o que exatamente é k-means? K-means é um algoritmo de agrupamento .

O objetivo é particionar n pontos de dados em k  clusters. Cada um dos n  pontos de dados será atribuído a um cluster com a média mais próxima. A média de cada cluster é chamada de "centróide" ou "centro".

Em geral, a aplicação de k-médias produz k clusters separados dos n pontos de dados originais . Os pontos de dados dentro de um cluster específico são considerados "mais parecidos" entre si do que os pontos de dados que pertencem a outros clusters.

No nosso caso, agruparemos as intensidades de pixel de uma imagem RGB. Dada uma  imagem de tamanho MxN , temos  pixels MxN , cada um composto por três componentes: Vermelho, Verde e Azul, respectivamente.

Vamos tratar esses  pixels MxN como nossos pontos de dados e agrupá-los usando k-means.

Os pixels que pertencem a um determinado cluster serão mais semelhantes em cores do que os pixels pertencentes a um cluster separado.

Uma ressalva de k-means é que precisamos especificar o número de clusters que queremos gerar com antecedência . Existem algoritmos que selecionam automaticamente o valor ideal de k, mas esses algoritmos estão fora do escopo desta publicação.
