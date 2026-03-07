# Título do projeto: Análise de vendas de uma rede de fast-food

## 💡 Resumo do projeto

Este projeto pessoal tem como objetivo marcar minha primeira aplicação prática pessoal dos conhecimentos em Análise de Dados que adquiri durante meu estágio no Banco do Brasil e nos estudos do Programa de Certificação Profissional em Análise de Dados do Google.

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

Também com fins educativos, incluí uma coluna com preços em dólar americano, já que o dataset original está em inglês, e outra com esses valores convertidos para reais. Para isso, utilizei a função do Google Sheets `=E2*GOOGLEFINANCE("CURRENCY:USDBRL")`.

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

## 🛠️ Metodologia e ferramentas

Para a primeira análise, utilizei o Google Sheets, organizando as informações da seguinte forma:

A planilha contém quatro abas informativas e duas abas geradas por tabelas dinâmicas, criadas com o objetivo de confirmar as informações apresentadas nas abas principais.

A primeira aba contém os dados brutos, ou seja, os dados em seu formato original.
A segunda aba apresenta os dados já tratados, com as adequações realizadas anteriormente.
A terceira aba exibe as informações de vendas por produto, organizadas em ordem crescente, utilizando formatação condicional para facilitar a identificação dos menores e maiores valores.
Na quarta aba, segui a mesma lógica, porém aplicada à receita por produto, também ordenada em ordem crescente e com a mesma formatação condicional.

As duas últimas abas correspondem às tabelas dinâmicas, utilizadas para validar os resultados obtidos nas abas anteriores.

Por fim, desenvolvi uma visualização no Power BI, criando um painel com estética inspirada em uma cafeteria, com o objetivo de responder às perguntas de negócio estabelecidas no projeto e apresentar essas respostas de forma clara e visualmente agradável:

<img width="1266" height="705" alt="image" src="https://github.com/user-attachments/assets/27382ac3-bc79-487b-9589-8bd2a8a75806" />


## 📈 Principais Insights e Resultados

### 1. Qual é o produto mais vendido?

O produto mais vendido foi o **Veg Alfredo Pasta**, com um total de **10.452 unidades vendidas**. Para obter esse resultado, foi criada uma aba auxiliar na planilha denominada *Vendas por Produto*, na qual a seguinte fórmula foi aplicada:

```excel
=SOMASE('Dados limpos'!D:D; A2; 'Dados limpos'!G:G)
```

Essa função permitiu consolidar o total de vendas agrupado por produto. Os resultados foram posteriormente validados por meio de uma tabela dinâmica, garantindo a consistência dos dados.

<img width="296" height="803" alt="Tabela de vendas por produto" src="https://github.com/user-attachments/assets/0587cd87-50e4-42bf-8f00-fcf54ce35cc6" />

---

### 2. Existe um horário de pico de pedidos?

Não foi possível identificar um horário de pico de pedidos. O conjunto de dados analisado **não contém informações sobre o horário das vendas**, o que inviabilizou essa análise. Caso essa variável estivesse disponível, seria possível identificar padrões temporais relevantes para a tomada de decisão.

---

### 3. Qual produto gera mais receita?

O produto com maior geração de receita foi o **Paneer Pizza**, totalizando **R$ 31.302,55**. Para essa análise, foi criada uma aba auxiliar denominada *Receita por Produto*, com a aplicação da seguinte fórmula:

```excel
=SOMASE('Dados limpos'!D:D; A:A; 'Dados limpos'!F:F)
```

Os resultados foram confirmados por meio de uma tabela dinâmica, assegurando a precisão dos valores calculados.

<img width="296" height="803" alt="Tabela de receita por produto" src="https://github.com/user-attachments/assets/f7e3cb59-3a43-461f-98c7-a753c9710df6" />

## 🚀 Como executar o projeto

Os arquivos deste projeto estão disponibilizados na pasta entregaveis/ deste repositório, contendo:

📊 Planilha Excel com os dados brutos, dados tratados e os insights que respondem às perguntas de negócio
🔗 Link para o dashboard interativo desenvolvido no Power BI

Para visualizar a planilha, basta realizar o download do arquivo .xlsx e abri-lo no Microsoft Excel ou Google Sheets. O dashboard do Power BI pode ser acessado diretamente pelo link disponível na planilha, sem necessidade de instalação.
Em caso de dúvidas ou sugestões, sinta-se à vontade para entrar em contato por meio da seção Issues deste repositório ou pelos canais disponíveis no meu perfil do GitHub.

## 🤝 Contato

[Email](cabraldorosarioanaleticia@gmail.com)

[Linkedin](https://www.linkedin.com/in/ana-let%C3%ADcia-cabral-do-ros%C3%A1rio-9a067631a/)
