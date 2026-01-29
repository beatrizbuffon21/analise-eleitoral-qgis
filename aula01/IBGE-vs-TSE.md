# Geografia Administrativa (IBGE) vs. Geografia Política (TSE)

Ao desenharmos um mapa eleitoral, não estamos apenas plotando números em um espaço abstrato.  
Estamos mapeando o "Lugar" (Place).

Segundo Agnew (1987), o comportamento político é estruturado pelo contexto social local.  
O "lugar" é composto por três elementos:

- **Locale (Cenário)**  
  Onde a vida cotidiana acontece (trabalho, casa, zona eleitoral).

- **Location (Localização)**  
  O impacto das estruturas macroeconômicas (ex: uma cidade industrial afetada por políticas nacionais).

- **Sense of Place (Senso de Lugar)**  
  A identidade subjetiva e o sentimento de pertencimento local.

O mapa do IBGE captura a demografia (Location), mas o mapa do TSE captura onde o ritual do voto acontece (Locale).  
O desafio do analista é cruzar essas duas realidades.

---

## O Município (Lógica do IBGE)

**O município**

**Definição**  
O município é uma unidade federativa autônoma, com estabilidade territorial e administrativa.  
É a base para a coleta de dados censitários (renda, escolaridade, IDH).

**O problema:**  
O Brasil possui mais de 5.500 municípios. Para análises nacionais, mapear cada um individualmente pode tornar a visualização caótica e fragmentada.

**Solução:**  
Frequentemente, agrupa-se os municípios em microrregiões (unidades intermediárias do IBGE) para facilitar a leitura de padrões regionais de voto e permitir a representação gráfica em uma única página.

---

## A Zona Eleitoral (Lógica do TSE)

**A zona eleitoral**

**Definição**  
A Zona Eleitoral não é uma cidade nem um ente federativo; é uma subdivisão administrativa da Justiça Eleitoral destinada a operacionalizar o pleito (alistamento, locais de votação, apuração).

**O problema:**  
Ao contrário dos municípios, que têm limites rígidos, as zonas eleitorais sofrem alterações frequentes (redesenho) promovidas pelos Tribunais Regionais Eleitorais (TREs).  
No Rio de Janeiro, por exemplo, houveram profundas mudanças nas zonas entre 1989 e 1994, o que muitas vezes impede a comparação direta de mapas históricos sem um tratamento prévio dos dados.

**Solução:**  
Em cidades pequenas, 1 Município = 1 Zona.  
Mas em metrópoles (Rio, SP), o município é grande demais para análise.  
Aqui, a Zona Eleitoral serve como uma lupa.  
Isso permite ao TSE ver a diferença entre o voto da periferia e o voto dos bairros de classe média dentro da mesma cidade.

---

## Cruzamento de Dados e Representação

Como saber a renda média (dado IBGE/Setor Censitário) de uma Zona Eleitoral (dado TSE), se as linhas dos mapas não batem perfeitamente?

**Solução**  
Utilização das Áreas de Ponderação (AREAP) do IBGE para compatibilizar esses limites, permitindo sobrepor dados sociais e políticos.

---

## A Lógica da Representação

O mapa eleitoral esconde uma desigualdade de valor.  
O voto de um eleitor em Roraima vale nove vezes mais (para eleger um deputado) do que o voto de um eleitor em São Paulo, devido às regras de piso (mínimo 8 deputados) e teto (máximo 70) que ignoram a população real medida pelo IBGE.  
O mapa mostra onde estão os votos, mas a regra do TSE define quanto eles valem.

Embora desenhemos mapas por município ou zona, a eleição para deputado é estadual.

---

## A Revolução do Geoprocessamento

Integração entre o sensoriamento remoto (imagens de satélite) e a capacidade computacional para análise geográfica.

Aplicável em planejamento urbano, análise ambiental, redes de transporte e política.

"Sempre que o onde aparece (...) haverá uma oportunidade para considerar a adoção de um SIG" (Câmara, 2001).

---

## O Pilar do SIG: Georreferenciamento de dados

Georreferenciamento: Identificação de dados com suas posições reais no espaço.

O Sistema de Coordenadas: Crucial para oferecer o "lastro real" à informação.

Sem referência geográfica correta, ocorrem erros que impedem a aplicação fundamentada do sistema.

A computação permite produzir informações espaciais com maior precisão e rapidez do que métodos manuais.

O modelo não deve ser tão abstrato que se distancie do comportamento dos objetos reais.

Todo modelo é uma simplificação do mundo real, pois é impossível reproduzir a paisagem em detalhes mínimos.

---

## Estruturas de dados (vetor e raster)

**Modelo Vetorial (Baseado em Objeto):**  
Elementos básicos: Ponto, Linha e Polígono.  
Cada objeto possui coordenadas e atributos próprios.  
Sujeito à Generalização Cartográfica (depende da escala de entrada).

**Modelo Matricial/Raster (Baseado em Campo):**  
Espaço dividido em uma grade de células (pixels).  
Qualidade determinada pela Resolução Espacial (tamanho da célula).  
Exemplo: Mapas de uso do solo ou imagens de satélite.

---

## Atributos na Representação Vetorial

**Tabela de Atributos:**  
Onde as conexões e dados qualitativos/quantitativos são armazenados.
