# Título do projeto: Análise de vendas de uma rede de fast-food

## 💡 Resumo do projeto

Este projeto pessoal tem como objetivo marcar minha primeira aplicação prática dos conhecimentos em Análise de Dados que adquiri durante meu estágio no Banco do Brasil e nos estudos do Programa de Certificação Profissional em Análise de Dados do Google.

Selecionei esse projeto a partir da plataforma de educação Rocketseat, com o intuito de iniciar uma jornada de projetos voltados à construção do meu portfólio.

Ele me propõe a buscar dados públicos de uma rede de fast food na plataforma Kaggle, realizar uma análise exploratória e criar um dashboard interativo.

## ❓ Problema de negócio / contexto

Perguntas propostas:
1) Qual o produto mais vendido?
2) Existe um horário de pico de pedidos?
3) Qual produto gera mais receita?


## 📊 Dados utilizados

- O conjunto de dados que utilizei para análise é o [Chaska Cafe Sales Data](https://www.kaggle.com/datasets/gatabhjsbaj/chaska-cafe-sales-data), localizado na plataforma do Kaggle. 

Este conjunto de dados consiste em um arquivo CSV, com tamanho de 495,73 kB, que contém informações diárias sobre as vendas de itens vegetarianos de um fast food ao longo do ano de 2023. Ele apresenta colunas com a data em que as vendas foram registradas, a categoria à qual o item pertence, o item em si (alimento ou bebida) e o número de vendas de cada item específico.

O dataset, em seu formato original, apresenta as datas no padrão yyyy-mm-dd. No entanto, alterei esse formato para o padrão brasileiro apenas para fins de estudo, a fim de facilitar a compreensão e a análise.

Também com fins educativos, incluí uma coluna com preços em dólar americano, já que o dataset original está em inglês, e outra com esses valores convertidos para reais. Para isso, utilizei a função do Google Sheets =E2*GOOGLEFINANCE("CURRENCY:USDBRL").

O objetivo de adicionar valores fictícios de preços foi suprir a ausência dessas informações no dataset original. Dessa forma, tornou-se possível apresentar insights iniciais relacionados à receita do Chaska Cafe, o que enriquece a análise proposta neste projeto.

Outras observações:

Os dados permanecem em seu formato original em inglês; no entanto, para facilitar os estudos, renomeei as colunas para o português, alterei as datas para o formato brasileiro e acrescentei as conversões de dólar americano para real.

Os tipos de dados foram definidos da seguinte forma:

→ Coluna Data: data

→ Coluna Categoria: texto simples

→ Coluna Produto: texto simples

→ Preço ($): dólar americano

→ Preço (R$): moeda

→ Vendas: número

Os dados foram classificados por categoria.

Não há linhas duplicadas, valores nulos ou espaços em branco extras.

Os nomes das colunas foram formatados em negrito e centralizados.

A largura das colunas foi ajustada.





## 🤝 Contato

[Email](cabraldorosarioanaleticia@gmail.com)

[Linkedin](https://www.linkedin.com/in/ana-let%C3%ADcia-cabral-do-ros%C3%A1rio-9a067631a/)
