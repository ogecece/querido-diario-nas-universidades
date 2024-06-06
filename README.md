# Querido Diário nas Universidades

## Sumário da documentação
1. [Contextualização do projeto](#contextualizacao)
2. [Bibliotecas importantes](#bibliotecas)
3. [Artigo 1](#artigo1)
4. [Artigo 2](#artigo2)
5. [Artigo 3](#artigo3)
6. [Entenda este repositório](#entenda)

**- Contextualização do projeto**
Trabalhar na resolução de problemas específicos não é uma tarefa trivial. O problema pode até estar claro, mas não existe a maneira correta de resolvê-lo, ou ainda, a maneira com que foi pensada a resolução não é possível de ser executada, por falta de pessoas, conhecimento, ou até mesmo recursos computacionais, de dados, ou .... E o que fazer quando se tem uma imensidão de possibilidades de trabalho, como é o caso da plataforma Querido Diário? A proposta ambiciosa de se ter em um único local o acesso a nível municipal dos diários oficiais abre possibilidades para diferentes áreas. Como esses dados serão armazenados e disponibilizados? Qual a ferramenta de nuvem utilizar? Como fazer a integração com diferentes sistemas de informações municipais? Como utilizar esses dados? O conjunto de perguntas é infinito e a vontade de responder essas perguntas permanece.

O Querido Diário nas Universidades surgiu em busca de uma aceleração dessas respostas por meio de parcerias com Instituições de Ensino. O projeto iniciou em setembro de 2022 e acaba de completar 2 anos de vigência. O apoio principal é da FIOCRUZ por meio da Fundação para o Desenvolvimento Científico e Tecnológica para a Saúde. Para a FIOCRUZ é importante consolidar informações relevantes para o desenvolvimento científico, principalmente em prol da Plataforma de Ciência de Dados Aplicados à Saúde.
Durante esses 2 anos, foram realizadas parcerias com Universidades e Instituto Federal, contando com o desenvolvimento de quatro desenvolvimentos com auxílio direto. Além disso, foram desenvolvidas pesquisas acompanhadas assincronamente e desenvolvidas pela própria equipe com uma chamada especial para alunos de graduação de qualquer lugar do país. Neste documento é possível acessar os repositórios e ver quem foram as pessoas envolvidas em cada um desses projetos.


**- Artigo 1**
Conhecer e utilizar técnicas de processamento de linguagem natural requer conhecimentos técnicos do processamento e específicos do escopo do texto em que se analisa. Esse documento traz um resumo dos resultados da revisão sistemática e bibliométrica de documentos científicos coletados na Web of Science, Scielo e Scopus relacionados à processamento de linguagem natural em diários oficiais brasileiros. Os principais resultados apontam sobre uma defasagem ao nível de publicações sobre o tema. Além disso, se considerar o âmbito de diário oficial municipal os resultados apontam para um número ainda menor. A partir desses resultados, é necessário refletir sobre como é possível realizar pesquisas científicas com o uso dos diários oficiais brasileiros, uma fonte confiável e alternativa na consulta pública.

**- Artigo 2**

<a name="contextualizacao"></a> 
Formalizada pelas Portarias n° 1.459 e 650 de 2011, a Rede Cegonha visou o repasse de recursos no intuito de criar mais Centros de Parto Normal e Casas de Gestantes, Bebês e Puérperas, a ampliação de exames pré-natal e doenças sexualmente transmissíveis visando diminuir as taxas de mortalidade materno-infantil nos municípios. Além de indicadores como mortalidade e cobertura vacinal, não há como mensurar a dimensão da adesão dos municípios a esse plano. O processamento de linguagem natural em textos de diários oficiais pode ser uma técnica promissora para ser usado conjuntamente a esses indicadores já consolidados na literatura de avaliação de políticas de saúde materno-infantil, especialmente para os municípios que são heterogêneos.  Nesse sentido, o estudo tem como objetivo comparar as técnicas de pré-processamento de linguagem natural (tokenização, stemming, taxonomia, remoção de stopwords, cortes de palavra baseado em frequência, N-grama, TF-IDF, bag-of-words, suavização e normalização) na extração de entidades nomeadas de diários oficiais dos municípios que possuem instituições incluídas na Rede Cegonha entre os anos de 2011 e 2021 (anos em que o Rede Cegonha teve vigência). Atualmente a Rede Cegonha está sendo substituída pela RAMI. Uma parte deste trabalho foi publicado no [Congresso da Região Brasileira da Sociedade Internacional de Biometria](https://rbras.org.br). Os dados utilizados para compor os indicadores de saúde materno-infantil podem ser consultados [aqui](https://drive.google.com/drive/folders/1HoYBnePlh3MTZXC0guEbDr2XXO9k_W0g?usp=sharing).

**- Artigo 3**

O avanço tecnológico trouxe novas oportunidades de estudo na ciência da informação, especialmente com o acesso online a uma ampla gama de documentos, incluindo os diários oficiais municipais. Este estudo visa aprimorar o processamento desses documentos, focando no reconhecimento de entidades nomeadas. Foram utilizadas técnicas de pré-processamento e a biblioteca spacy para analisar 30.000 excertos de diários oficiais de municípios. Os resultados destacam a importância da lematização na identificação de entidades, ressaltando a complexidade da tarefa. Esses documentos desempenham um papel crucial no monitoramento de políticas públicas e que as técnicas de processamento de linguagem natural têm um grande potencial no contexto governamental.

**- Algumas bibliotecas úteis para o projeto:**
<a name="bibliotecas"></a>

**[Bertopic](https://maartengr.github.io/BERTopic/getting_started/quickstart/quickstart.html)**, é uma biblioteca que podemos utilizar para fazer modelagem de tópicos utilizando língua portuguesa. Teve bons resultados no trabalho realizado pela UNIT.

**[Scrapy](https://docs.scrapy.org/en/latest/topics/spiders.html)** é uma biblioteca que permite extrair informações de websites. Alguns comandos básicos:

**[NLTK](https://www.nltk.org)** é uma plataforma para trabalhar com linguagem natural. É uma API robusta na qual é necessário acessar os [subpacotes](https://www.nltk.org/api/nltk.html) de sua estrutura para trabalhar com as diversas funcionalidades, tais como modelos de linguagem, pré-processamento, análise de sentimento, entre outros.

**[SpaCy](https://spacy.io/usage/spacy-101)** é uma biblioteca _open-source_ para trabalhar com Processamento de Linguagem Natural (PLN). Na documentação, é possível aprender sobre as _features_ do pacote, tais como pré-processamento de textos, modelos estatísticos incorporados, reconhecimento de entidades, entre outros.

O _corpus_, frequentemente mencionado no PLN, é uma coletânea de textos, sendo estes frequentemente o conjunto de dados linguístico em que será realizada a análise. Os pacotes que utilizam artifício da PLN possuem a capacidade de ler esse conjunto de dados e tranformá-los em _corpus_ que são possíveis de serem interpretados pela linguagem da máquina.

**_Alguns outros pacotes_**

**[Pandas](https://pandas.pydata.org/)**

### Entenda este repositório
<a name="entenda"></a>

Este projeto é fruto da iniciativa da [**Open Knowledge Brasil**](https://ok.org.br) com o lançamento da chamada de voluntários para trabalhar no âmbito do [Querido Diário nas Universidades](https://ok.org.br/noticia/querido-diario-nas-universidades/).
