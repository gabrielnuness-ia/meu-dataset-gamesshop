Entrega do Projeto avaliativo Meu Dataset-Gameshop

# O que é o projeto?
- O projeto visa receber os dados de uma empresa fabricante global de games e, a partir desses dados gerar insights úteis afim de melhorar a eficiência logística da empresa.

## informações sobre a empresa
- A empresa foca apenas em fabricação de consoles, deixando a distribuição e venda para terceiros
- Os produtos são vendidos globalmente
  
## Materiais
- Foram disponibilizadas três planilhas com dados brutos.

## Objetivos a serem cumpridos

- [X] Consolidar todas as bases de terceiros para realizar uma análise
- [X] Transformar dados de vendasem informações relevantes para a fabricante
- [X] Quais são os produtos mais populares em cada país
- [X] Como otimizar o processo de transporte e logística até o momento da venda

# Execução passo a passo
- Primeiro foram criadas as pastas, como sugerido na aula.
- Em seguida, as planilhas com dados brutos foram inseridas na pasta data/raw.data
- Então os dados foram abertos no excel e unidos afim de termos dados completos em um único local
- A partir daí, vieram as análises com inteligência artificial.
- Os resultados foram obtidos.

## Aprendizado, Execução Passo a Passo e Resultado

- Esse foi um bom desafio. Não conheço muito de programação, então projetos que envolvem git/github/vscode são um pouco mais desafiadores. Por esse motivo, decidi não fazer FORK do repositório do professor, decidi fazer o meu e subir os arquivos em busca de me desafiar. Consegui. Aqui tive ajuda do Copilot, mas poderia assistir as aulas específicas novamente, caso fosse necessário.
  
- Para ter o melhor resultado inseri prompts em 3 diferentes IAs (Chatgpt, Claude, Grok3 todos em modo gratuito). O Copilot infelizmente não lê planilhas, então ficou de fora.
iniciei com o prompt mais simples enviado em aula, no ChatGPT, busquei um agente especialista (https://chatgpt.com/g/g-xqNBnrR2o-data-analyst/), enquanto o grok3 foi usado no modo Think e o Claude apenas chat normal.

- Tive então o primeiro grande desafio: As três IAs entregaram respostas diferentes.
  
- Para confirmar o resultado correto, voltei à planilha oficial, com as 3 camadas de venda e criei os cálculos (a segunda planilha na pasta processed_data. Afim de evitar erros, pintei as linhas para melhor visualização. Assim pude conferir quem tava certo e quem tava errado (mas também percebi que se fossem muito mais dados, eu poderia ter um grande problema) mas que, assim como esses, seria resolvido.
  
- Após confirmação, o ChatGPT especilista conseguiu entregar o resultado correto logo na primeira tentativa, mesmo com um prompt simples, enquanto Grok3 e Claude erraram, tendo claude errado nas próximas 3 tentativas, sendo descartado e o ChatGPT acabaram as tentativas de uso.
  
- Fiz uma nova tentativa no Grok3 com um novo prompt, ele então corrigiu e me entregou corretamente o resultado ideal, com algumas informações extras, conforme arquivo Prompts Grok3, que foi utilizado até o final do projeto.

# RESPOSTAS

## 1 - Os Dados Brutos e Organizados Estão nas Pastas raw_data e processed_data
- Na pasta raw_data encontram-se os dados brutos, como solicitado
- Na pasta processed_data encontram-se os dados organizados. Há duas planilhas, pois uma delas foi utilizada para conferência dos valores de vendas cada país, em busca de entregar uma resposta 100% correta.


## 2 - Transformar os Dados de Vendas em Informações Relevantes

- Aqui está a tabela de resumo das vendas por país com os valores de venda somados (mesmo em moedas distintas):

País	Quantidade Total Vendida	Receita Total

- Canadá:
Vendas:	46
Receita: $4090

- França	
Vendas:36
Receita: $3210

- Japão
Vendas:27
Receita: $2510

- Austrália
Vendas:28
Receita: $2330

- Alemanha	
Vendas:23
Receita: $2010
- Reino Unido
Vendas:13
Receita: $1260
  
- EUA
Vendas:5
Receita: $520



## 3 - Quais São Os Produtos Mais Vendidos em Cada País

Com base na análise dos dados de vendas das plataformas AliExpress, Etsy e Shopee, identificamos os produtos mais populares em cada país, considerando a quantidade total vendida de cada produto. Em alguns países, há empates entre dois ou mais produtos que venderam a mesma quantidade máxima. Abaixo está a lista dos produtos mais populares por país:

### Produtos Mais Populares por País

- País
- Produto Mais Popular
- Quantidade Vendida

### Canadá
NEW MEGANIUM RG 40XXV (SKU-40XXV01): 17

### França
Empate: 
 - NEW MEGANIUM RG35XX (SKU-35XX01): 9
 - NEW MEGANIUM RG CubeXX (SKU-CUBEXX01): 9 
 - NEW MEGANIUM RG 40XXV (SKU-40XXV01): 9
9 (cada)

### Austrália
Empate: 
 - NEW MEGANIUM RG28XX (SKU-28XX01): 10
 - NEW MEGANIUM RG CubeXX (SKU-CUBEXX01): 10 
10 (cada)
   
### Japão
- NEW MEGANIUM RG 40XXV (SKU-40XXV01): 11

### Alemanha
- NEW MEGANIUM RG35XX (SKU-35XX01): 7

### Reino Unido
- NEW MEGANIUM RG35XX (SKU-35XX01): 7

### EUA
- MEGANIUM RG353M (SKU-353M01): 3



## 4 = Como Otimizar o Processo de Transporte e Logística até o Momento da Venda

### Resultado

Para ajudar a empresa fabricante de games global (fictícia) a otimizar seus custos e logística, considerando os dados de vendas fornecidos e a distribuição igual de containers em todos os locais, podemos gerar insights estratégicos baseados em uma análise detalhada. Abaixo estão as recomendações para melhorar a eficiência operacional e reduzir desperdícios, utilizando os números de vendas por país: Canadá (46), França (36), Austrália (28), Japão (27), Alemanha (23), Reino Unido (13) e EUA (5).

## 1. Realocar Containers com Base na Demanda Real
Problema: A empresa mantém containers em quantidades iguais em todos os países, mas as vendas variam significativamente. Por exemplo, o Canadá (46 vendas) e a França (36 vendas) têm uma demanda muito maior que os EUA (5 vendas) e o Reino Unido (13 vendas). Isso sugere que a alocação atual não reflete a necessidade real, gerando custos desnecessários de armazenamento em locais de baixa demanda.
Solução: Redistribuir os containers proporcionalmente às vendas. Aumentar a alocação no Canadá e na França, enquanto reduzir nos EUA e no Reino Unido. Isso minimiza custos de manutenção e acelera o atendimento em mercados mais ativos.

## 2. Criar Centros de Distribuição Regionais
Problema: Manter containers separados em todos os países pode ser ineficiente, especialmente em regiões próximas umas das outras.
Solução: Estabelecer hubs logísticos regionais para consolidar a distribuição:
Europa: Um hub para atender França (36 vendas), Alemanha (23 vendas) e Reino Unido (13 vendas), aproveitando a proximidade geográfica.
América do Norte: Um hub para Canadá (46 vendas) e EUA (5 vendas), reduzindo a necessidade de containers nos EUA.
Ásia-Pacífico: Um hub para Japão (27 vendas) e Austrália (28 vendas), otimizando o transporte na região.
Benefício: Redução de custos de transporte e manutenção, além de maior eficiência na gestão de inventário.

## 3. Analisar Custos Locais de Armazenamento e Envio
Problema: Os custos de manter containers variam entre os países. Locais com custos altos e baixa demanda, como possivelmente os EUA (5 vendas), podem ser ineficientes.
Solução: Avaliar os custos operacionais (armazenamento e envio) em cada país. Se, por exemplo, o Japão tem custos elevados, pode ser mais econômico atender sua demanda (27 vendas) a partir de um hub regional na Ásia, desde que o impacto no tempo de entrega seja viável.
Benefício: Redução de despesas em locais caros, mantendo a capacidade de atendimento.

## 4. Adotar um Sistema de Gestão de Inventário Dinâmico
Problema: A demanda por games pode variar devido a lançamentos ou sazonalidade, e a alocação fixa de containers não acompanha essas mudanças.
Solução: Implementar um sistema baseado em dados, com previsões de demanda e monitoramento em tempo real das vendas. Isso permitiria ajustes rápidos, como aumentar containers no Canadá antes de um grande lançamento ou reduzir no Reino Unido em períodos de baixa.
Benefício: Evitar excessos ou faltas de estoque, otimizando custos e melhorando a resposta ao mercado.

## 5. Aproveitar Economias de Escala no Transporte
Problema: Enviar pequenas quantidades de produtos para países com baixa demanda aumenta o custo por unidade.
Solução: Consolidar envios em lotes maiores para países de alta demanda, como Canadá (46 vendas) e França (36 vendas), utilizando transporte mais econômico.
Benefício: Redução dos custos de frete e aumento da margem de lucro.

## 6. Reavaliar Containers em Países de Baixa Demanda
Problema: Manter containers nos EUA (5 vendas) pode ser desnecessário, dado o baixo volume.
Solução: Eliminar containers em locais de baixa demanda e atender esses mercados a partir de hubs regionais próximos, como usar o hub do Canadá para os EUA.
Benefício: Diminuição de custos fixos sem comprometer o atendimento.

## Conclusão
Para otimizar custos e logística, a empresa deve:
1 - Realocar containers com base nas vendas (mais no Canadá e França, menos nos EUA e Reino Unido).
2 - Criar hubs regionais na Europa, América do Norte e Ásia-Pacífico.
3- Analisar custos locais e priorizar locais mais econômicos.
4 - Implementar um sistema dinâmico de gestão de inventário.
5 - Consolidar envios para reduzir custos de transporte.
6 - Reduzir containers em países de baixa demanda, como os EUA.

Essas ações permitirão à empresa alinhar sua logística à demanda real, reduzir custos operacionais e responder de forma ágil às variações do mercado global de games, melhorando sua eficiência e rentabilidade.

