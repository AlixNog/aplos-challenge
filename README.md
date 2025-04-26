# 🚛 Palantir Developer Technical Challenge: Business Process Automation and Ontology Design

## 📚 Contexto

Fui contratado como desenvolvedor Palantir Foundry em uma empresa de logística de médio porte que visa automatizar e modernizar suas operações de supply chain. Atualmente, os dados estão dispersos em vários sistemas, dificultando a tomada de decisão eficiente.

Minha missão foi:

- Integrar datasets isolados.
- Criar uma ontologia que permita a interoperabilidade dos dados.
- Desenvolver um sistema escalável de automação de processos de negócio.

---

## 🎯 Objetivos

- Ingerir, limpar e integrar múltiplos datasets de diferentes sistemas de negócios.
- Projetar uma ontologia que suporte automações e análises interfuncionais.
- Criar uma automação de processos que gere insights operacionais.

---

## 🗂️ Datasets Utilizados

1. **Orders.csv**
   - `order_id`: Identificador único do pedido
   - `customer_id`: Identificador único do cliente
   - `product_id`: ID do produto comprado
   - `order_date`: Data da compra
   - `order_status`: Status do pedido (Pending, Shipped, Delivered, Canceled)

2. **Inventory.csv**
   - `product_id`: Identificador único do produto
   - `warehouse_id`: ID do armazém onde o produto está armazenado
   - `stock_quantity`: Quantidade disponível em estoque

3. **Shipments.csv**
   - `shipment_id`: Identificador único da remessa
   - `order_id`: Pedido associado à remessa
   - `carrier`: Transportadora
   - `status`: Status da remessa (In Transit, Delivered, Delayed)

---

## 🔧 Solução Desenvolvida

### 1. Integração de Dados e Ontologia

- Carregamento e limpeza de dados (remoção de duplicatas, padronização de formatos de data).
- **Ontologia desenhada** conecta:
  - Pedidos a remessas.
  - Produtos ao estoque nos armazéns.
  - Histórico de pedidos rastreável por cliente.
- Definições claras para todos os atributos e regras de integridade aplicadas.

> 💡 **Pergunta-chave respondida:** A ontologia possibilita o uso cruzado dos dados, como prever a necessidade de estoque usando dados de remessas e pedidos.

---

### 2. Automação de Processo de Reabastecimento

- Lógica criada para recomendar reabastecimento automático baseada em:
  - Vendas dos últimos 30 dias.
  - Tempo médio de entrega por transportadora.
- Script desenvolvido em Python gera uma lista com:
  - `product_id`, `warehouse_id`, `recommended_restock_quantity`.

> ⚡ **Benefício:** Automatização reduz tarefas manuais, antecipando necessidades de reposição com base em dados históricos.

---

### 3. Insights e Tomada de Decisão

- **Métricas geradas:**
  - Tempo médio de entrega por transportadora.
  - Top 5 produtos mais vendidos no último trimestre.
- **Visualizações criadas:**
  - Escassez de estoque por armazém baseada em tendências de demanda.

---

## 🧠 Desafio Avançado (Opcional)

Proposta de expansão da ontologia para incluir dados de fornecedores externos, visando melhorar ainda mais a automação e previsão da cadeia de suprimentos.

---

## 📂 Entregáveis

- 📓 Notebooks (Jupyter) com processamento, limpeza e automação de dados.
- 🧩 Diagrama da Ontologia.
- 📝 Relatório PDF explicando:
  - Abordagem de design da ontologia.
  - Lógica da automação.
  - Impacto no negócio.

---

## 🏆 Critérios de Avaliação

1. **Design da Ontologia:** Facilita interoperabilidade entre áreas de negócio?
2. **Efetividade da Automação:** Reduz trabalho manual de forma eficiente?
3. **Qualidade e Performance do Código:** Código limpo, estruturado e eficiente?
4. **Impacto no Negócio:** Solução melhora a tomada de decisão?

---

## 🛠️ Tecnologias Utilizadas

- Python 3.x
- Pandas
- NumPy
- Matplotlib / Seaborn
- Jupyter Notebook
- (Opcional) Palantir Foundry

---

## 📎 Licença

Projeto desenvolvido para fins educacionais e demonstração técnica. Sem fins comerciais.

---

## 🖼️ Diagrama da Ontologia

![Ontology Diagram](./A_diagram_on_ontology_in_business_process_automati.png)

---

