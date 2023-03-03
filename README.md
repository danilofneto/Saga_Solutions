# Supermarket Sales Analysis

![question22](/images/supermarket.jpg)

# Contexto
O crescimento dos supermercados nas cidades mais populosas está aumentando e as competições de mercado também são altas. O conjunto de dados é sobre vendas históricas da empresa de supermercados que registrou dados em 3 filiais diferentes por 3 meses.

 # Business Problem

O gerente dessas 3 filiais do supermercado está sem nenhuma visão das vendas dessas filiais, e pediu ajuda ao time de BI da Saga Solutions para conseguir ter clareza dos principais KPIs dessas filiais e acompanhar a evolução de cada uma delas.
 

  # Os Dados

  Os Dados foram retirados do dataset https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales e originalmente contém as seguintes features:

**Invoice id:** Número de identificação da fatura do recibo de venda gerado por computador

**Branch:** Filial do supercentro (estão disponíveis 3 filiais identificadas por A, B e C).

**City:** Localidade do supercentro

**Customer type:** Tipo de clientes, registados por Associados para clientes com cartão de sócio e Normal para sem cartão de sócio.

**Gender:** Genero cliente

**Product line:** Grupos de categorização geral de itens - Acessórios eletrônicos, Acessórios de moda, Alimentos e bebidas, Saúde e beleza, Casa e estilo de vida, Esportes e viagens

**Unit price:** Preço da unidade do produto em dólar

**Quantity:** Número de produtos comprados pelo cliente

**Tax:** 5% tax fee for customer buying

**Total:** Preço total incluindo impostos

**Date:** Data de compra (Registro disponível de janeiro de 2019 a março de 2019)

**Time:** Horário de compra (10h às 21h)

**Payment:** Pagamento usado pelo cliente para compra (3 métodos estão disponíveis – Dinheiro, Cartão de Crédito e Ewallet)

**COGS:** Custo de bens vendidos

**Gross margin percentage:** Porcentagem de margem bruta

**Gross income:** Renda bruta

**Rating:** Classificação da estratificação do cliente em sua experiência geral de compra (numa escala de 1 a 10)

# Criação das Hipóteses

Em conjunto com o time de negócios do supermercados foram criados as seguintes hipóteses, para que à partir delas fossem retirados insights da análise bivariada dos dados.

Lista de hipóteses:

* H1 O Supercentro A possui o maior número de vendas
* H2 A linha de produto mais vendida e com o maior rating é a de Acessórios eletrônicos
* H3 Clientes do sexo Masculino compram mais itens
* H4 O método de pagamento mais utilizado é o cash
* H5 A Cidade de Yangon possui muito mais vendas que as doutras cidades
* H6 Os clientes fazem mais compras no período diurno
* H7 O Supercentro A é o mais lucrativo
* H8 Janeiro foi o mês com o maior número de vendas

# Top Insights
### **H1 O Supercentro A possui o maior número de vendas.** 


Hipótese Falsa. A superstore C possui o maior valor total de vendas das superstores com um total de 110568.7 em vendas
![image](/images/total_loja.png)

### **- Hipótese 2: CA linha de produto mais vendida e com o maior rating é a de Acessórios eletrônicos.**


Hipótese Falsa. A linha de produtos o maior valor total de vendas e com melhor rating é a Food and beverages com um total de 56144.844 vendidos

![image](/images/total_linha_produto.png)

### **- Hipótese 3: Clientes do sexo Masculino compram mais itens.**

Hipótese Falsa. Clientes do sexo Feminino possuem um valor total de compras maior do que os clientes do sexo masculino.

![image](/images/total_sexo.png)

### Hipótese 4: O método de pagamento mais utilizado é o cash

Hipótese verdadeira. O método de pagamento mais utilizado foi o cash e representou um total $112206.6 em vendas
![image](/images/total_metodo_pagamento.png)


### Hipótese 5: A Cidade de Yangon possui muito mais vendas que as doutras cidades

Hipótese falsa. A cidade de Naypyidaw possui o maior número de vendas.
![image](/images/total_cidade.png)

### Hipótese 6: Os clientes fazem mais compras no período diurno
Hipótese verdadeira. Os clientes realizam mais compras durante o dia, principalmente por volta das 14 hrs
![image](/images/total_dia.png)
![image](/images/hora_compra.png)

### Hipótese 7: O Supercentro A é o mais lucrativo
Hipótese falsa. O Supercentro C possui a maior renda bruta seguida por A e B

### Hipótese 8: Janeiro foi o mês com o maior número de vendas
Hipótese verdadeira. O mês de janeiro teve a maior quantidade em vendas com 1965 itens vendidos seguido por Março com 1891 e Fevereiro com 1654
![image](/images/total_mes.png)

### Hipótese 9: Clientes membros gastam mais que clientes normais
Hipótese verdadeira. Clientes membros gastam mais, uma diferença de 5480.10.
![image](/images/total_customer_type.png)

Os clientes do tipo membro geralmente gastam mais com os produtos da linha Food and beverages e os clientes do tipo normal gastam mais com a linha de Electronic accessories

![image](/images/product_line_customer.png)

### Hipótese 10: Uma mesma linha de produtos é campeã de vendas em todas as cidades
Hipótese Falsa. Na cidade de Yangon, os clientes gastam menos em  Health and Beauty e mais Home and Lifestyle.

Na cidade de Mandalay, os clientes gastam menos em Food and Beverages e mais Sports and travel.

Na cidade de Naypyidaw, os clientes gastam menos em Home and lifestyle e mais  Food and Beverages.

![image](/images/product_line_city.png)


# Conclusões/Recomendações

 - A rede de supermercados deve melhorar a qualidade da linha de Home and lifestyle products ou dar mais descontos para uma melhor performance nas vendas.
 - Clientes membros acabam gastando mais, então é interessante criar um programa de fidelidade para atrair novos clientes membros.
 - Criar promoções durante o período diurno pode melhorar ainda mais as vendas.
 - Analisar o fator diferencial para o mês de Janeiro ter sido o mês com o maior número de vendas.
 - A loja de Naypyidaw concentra boa parte das vendas, então se for necessário a criação ou expensão de lojas, a melhor cidade será Naypyidaw.
 - Aumentar o estoque de Food and beverages pode ser interessante, visto que eles geram o maior total de vendas.
- A média do rating de satisfação dos clientes é 6.97 o que indica que geralmente os clientes saem satisfeitos com sua experiência de compra

# Próximos passos de evolução:
- Criar novas features.

- Disponibilizar os dados em tabelas no BD e orquestrar sua atualização.

- Adicionar mais visualizações no Power BI.

- Treinar modelos de machine learning para estimar o total de vendas por loja nos próximos meses.