# Repositório de Dashboards em Power BI

Bem-vindo ao meu repositório de dashboards em Power BI! Este espaço foi criado para armazenar e organizar todos os dashboards que desenvolvo ao longo da disciplina da faculdade. O objetivo é demonstrar o aprendizado prático em manipulação de dados, visualização e criação de insights interativos.

---

## 🔹 Conteúdo do Repositório

Atualmente, este repositório contém:

- **Dashboard Triacca (Aula 1)**: Primeiro dashboard desenvolvido em sala de aula, baseado no documento **Triacca**, utilizando a tabela `table_inv_switches` com dados de equipamentos de rede.
  - Principais funcionalidades:
    - Gráficos interativos de contagem de equipamentos.
    - Métricas resumidas por marca, modelo e versão.
    - Gráfico por ano extraído da coluna `DATA` para análise anual.

- Outros dashboards serão adicionados conforme o andamento da disciplina.

---

## 🔹 Tecnologias e Ferramentas

- **Power BI Desktop**: Ferramenta principal para criação de dashboards.
- **SQL / PostgreSQL**: Fonte de dados utilizada para alimentar os dashboards.
- **Transformação de Dados**: Limpeza e modelagem de dados dentro do Power BI, incluindo colunas calculadas (ex: extração do ano da data).

---

## 🔹 Estrutura dos Dashboards

Cada dashboard possui:

1. **Relatórios Interativos**: Permitem filtragem dinâmica e análise detalhada.
2. **Gráficos Resumidos**: Cartões e gráficos que mostram métricas-chave.
3. **Tratamento de Datas**: Colunas calculadas para extrair informações relevantes (como ano, mês ou trimestre).

---

## 🔹 Exemplo de Dados

Exemplo de inserção de dados utilizados no dashboard:

```sql
INSERT INTO table_inv_switches 
(REGISTRO, DATA, HORA, HOSTNAME, IP_ADDRESS, MAC_ADDRESS, MARCA, MODELO, NUM_SERIE, VERSAO, IMOBILIZADO) 
VALUES 
(1, '2020-10-22', '17:25:51', 'SW-ANALIT-DADOS-6', '172.31.120.6', '84:80:2D:FB:08:25', 'Cisco', 'SG300-52', 'DNI18390F2U', '1.4.9.4', 'CP2662');
