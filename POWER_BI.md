# BI_PROVA_ESPECIALISTABI

# OBJETIVOS 

O objetivo deste relatório é apresentar os resultados financeiros por meio dos principais indicadores, com base nos requisitos a seguir:

1 - Valor Orçado, Despesas, Desvio Real - Consolidado, Por Mês, Por Conta, Por Centro de Custo;

1.1 - Implementar medidas dinâmicas que ajustem automaticamente os valores orçados com base em taxas de câmbio ou ajustes de orçamento que possam ocorrer ao longo do ano. Use DAX para criar uma lógica condicional que considere essas variações;

1.2 - Criar uma análise de tendência temporal que compare o valor realizado contra o valor orçado, incluindo a projeção para os próximos meses baseada no desempenho atual;

1.3 - Desenvolva um indicador de "alerta" que sinaliza desvios significativos do orçado que excedam um limite pré- definido. O indicador deve ser visualmente distinto e acionável, permitindo aos usuários investigar a causa dos desvios rapidamente;

2 - Variação entre meses em p.p sobre o desvio;

2.1 - Desenvolver um modelo de pontuação que classifique as contas com base no impacto de seus desvios no desempenho geral. Integre uma visualização que mapeie contas ofensoras em um "mapa de calor" baseado na pontuação de impacto;

3 - Realizado x Orçado do centro de custo TIME MIS;

3.1 - Criar um gráfico dinâmico que permita a seleção de múltiplos centros de custo para comparação simultânea. Implemente funcionalidades de drill-down que permitam analisar o desempenho mensal detalhado de cada centro de custo selecionado;

4 - Mostre o resultado do indicador para o centro de custo TIME MIS no mês de Janeiro - CONTA: 260001.

# VISUAIS

## Financeiro

Para a primeira visualização, foram desenvolvidos dois painéis distintos: um gráfico e uma tabela. O objetivo é fornecer uma visão geral do desempenho financeiro da empresa, permitindo a filtragem por contas e períodos de datas. O gráfico oferece uma representação clara e rápida do status atual, enquanto a tabela fornece detalhes para análises mais aprofundadas.

![Prova - Especialista de BI-2](https://github.com/user-attachments/assets/561530b3-d103-4928-95ca-4126d997f623)

![Prova - Especialista de BI-3](https://github.com/user-attachments/assets/661f22e7-6fad-48b0-8d9c-602d36b9584a)

## Simulações 

Na segunda visualização, o objetivo é possibilitar simulações de ajustes orçamentários e despesas, permitindo a comparação de diferentes cenários em relação ao estado atual.

![Prova - Especialista de BI-4](https://github.com/user-attachments/assets/9a046a99-874d-43c3-bd02-13a2c3993f52)

## Contas

Na terceira visualização, o objetivo é analisar o desempenho das contas, tanto em relação a si mesmas quanto em relação ao desempenho geral. Para isso, foram criados um ranking de impacto e um mapa de calor.

![Prova - Especialista de BI-5](https://github.com/user-attachments/assets/d865ff61-2c25-4649-a07b-c07bcd3b1b93)

## Time MIS

Na quarta visualização, o objetivo é possibilitar a análise do desempenho do centro de custo da equipe MIS e seus correspondentes, além de permitir a avaliação das contas em períodos de tempo desejados. Nesse visual, também é possível observar o desempenho da conta 260001 como solicitado no objetivo 4.

![Prova - Especialista de BI-6](https://github.com/user-attachments/assets/8af74b31-6877-456b-a44c-2b60f8e42e38)

# RELACIONAMENTO DE TABELAS 

O esquema adotado para a organização dos dados foi o modelo estrela, que consiste em duas tabelas fato: contas e centro de custos. As tabelas dimensões incluem orçamento, ajuste orçamentário e despesas.

As relações entre as tabelas foram configuradas como 1 para Muitos, utilizando as chaves primárias dos códigos das contas e do centro de custos, o que otimiza a performance dos filtros.

![relacionamentos](https://github.com/user-attachments/assets/3db4e448-cd7f-4ea6-ba90-6996b8c555e3)

