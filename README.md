# Logistic-Regression
Apresentação dos atributos da base de dados:
tempo_diario_site: tempo diário no site em minutos.
idade: idade do consumidor.
renda_media_regiao: Média da renda do consumidor na região.
tempo_medio_internet: Média em minutos por dia que o consumidor está na internet.
titulo: Título do anúncio.
cidade: Cidade do consumidor.
sexo: Se o consumidor era ou não masculino.
pais: País do consumidor.
timestamp_clique': hora em que o consumidor clicou no anúncio ou janela fechada.
clique: 0 ou 1 indicam se clicou ou não no anúncio.


Iniciei a análise exploratória dos dados utilizando o Power BI Desktop (anexo a este, assim como publicado em https://sites.google.com/view/clarice-satiko-aoto/data-science/e-commerce-m%C3%A1quina-preditiva)

Para complementar a análise, gerei um relatório utilizando o Pandas Profiling e assim como no Power BI, quebrei o atributo 'timestamp_clique' em ano, mes, dia e hora.

Construí a máquina preditiva utilizando a Regressão Logística, fazendo diversos testes com as variáveis, e as acurácias são apresentadas conforme seguem:
1) renda_media_regiao, idade, tempo_medio_internet, sexo : 84%
2) tempo_diario_site, idade, tempo_medio_internet, renda_media_regiao : 86%
3) sexo, tempo_medio_internet, renda_media_regiao : 70%
4) sexo, tempo_medio_internet, idade : 90%
5) sexo, tempo_diario_site, idade : 89%

Conclusão: Apesar de ter utilizado apenas tres variáveis, a melhor acurácia apresentada foi de 90%, significando que nem sempre mais informações resultam em respostas melhores.
