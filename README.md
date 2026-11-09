# Online Retail | Análise exploratória com Python

Projeto de portfólio de Rafael Gonçalves, desenvolvido a partir do projeto orientado do Coursera. A análise usa 541.909 linhas de faturas de uma loja britânica, de 1º de dezembro de 2010 a 9 de dezembro de 2011.

## O que a análise encontrou

| Tema | Resultado |
| --- | --- |
| Sazonalidade | Novembro de 2011 liderou os meses completos, com £1,51 milhão em vendas brutas. O pico se manteve após descontar cancelamentos e após retirar as cinco maiores faturas. |
| Produtos | Uma única fatura concentrou as 80.995 unidades brutas do SKU 23843. A triagem encontrou um cancelamento compatível no mesmo dia. Sem as cinco maiores faturas, o SKU 84077 liderou em unidades. |
| Clientes | 65,6% dos 4.338 clientes identificados fizeram pelo menos dois pedidos. O recorte RFM sinalizou 494 clientes para um teste de retenção. |

## Abordagem

O notebook audita valores ausentes e linhas idênticas, separa vendas, cancelamentos e ajustes, compara períodos com cobertura distinta e testa a influência de faturas extremas. A segmentação RFM usa recência, frequência e valor monetário. As compras sem identificação permanecem nos totais de vendas e ficam fora da análise por cliente.

## Como reproduzir

1. Abra o [notebook executado](Online_Retail_EDA_Rafael_Goncalves.ipynb) para consultar código, gráficos e resultados.
2. Baixe o arquivo `Online Retail.xlsx` na [fonte oficial UCI Online Retail](https://archive.ics.uci.edu/dataset/352/online+retail) e coloque-o ao lado do notebook.
3. Instale as dependências com `python -m pip install -r requirements.txt`.
4. Abra o notebook no Jupyter e execute as células em ordem.

O conjunto de dados fica disponível na fonte original. Dezembro de 2011 tem cobertura parcial. A base não informa custos e o pareamento de cancelamentos é indicativo, pois falta a chave da fatura original.
