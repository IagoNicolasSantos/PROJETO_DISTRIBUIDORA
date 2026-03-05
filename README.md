# PROJETO_DISTRIBUIDORA
"Projeto de modelagem conceitual e lógica de banco de dados relacional para um ERP de Gestão de Vendas, Estoque e Cadeia de Suprimentos."

## 📌 Sobre o Projeto
Este repositório documenta a arquitetura de banco de dados relacional projetada para um sistema robusto de gestão de vendas (ERP). A modelagem foi desenhada para suportar o fluxo operacional completo de uma empresa comercial, conectando clientes, pedidos, controle de estoque (peças), categorias, marcas, fornecedores e vendedores.

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Engenharia de Dados:** Modelagem Conceitual e Modelagem Lógica.
* **Ferramenta de Modelagem:** brModelo.
* **Controle de Versão:** Git / GitHub.

## 📊 Arquitetura de Dados

### 1. Modelo Conceitual (Diagrama Entidade-Relacionamento - DER)
O diagrama mapeia as regras de negócio complexas do comércio:
* **Clientes e Pedidos:** Rastreio de quem faz o pedido, com datas e valores totais.
* **Pedidos e Peças (Itens do Pedido):** Relação N:N resolvida para contabilizar subtotal e quantidade de itens em um carrinho/pedido.
* **Gestão de Produtos:** Peças classificadas por categorias e fabricadas por marcas específicas.
* **Cadeia de Suprimentos e Vendas:** Vínculo de peças fornecidas por diferentes fornecedores (CNPJ) e o registro do vendedor responsável por cada pedido.
* <img width="876" height="512" alt="Captura de tela 2026-03-05 163003" src="https://github.com/user-attachments/assets/7e7e2d9d-5bd6-45d2-8ba7-693374fe4d8b" />
### 2. Modelo Lógico
Estruturação relacional detalhada, preparando o terreno para a implementação em SGBDs SQL, com a definição precisa de:
* **Tipagem de dados e granularidade:** Uso de `INT` para identificadores, `VARCHAR` para textos/documentos, `FLOAT` para valores monetários e `DATE` para registros temporais.
* **Chaves Primárias (PK):** Identificadores únicos bem estabelecidos (ex: `ID_Pedido`, `ID_Cliente`, `ID_Peça`).
* **Resolução de Cardinalidade (Tabelas Associativas):** Criação das tabelas `Contém` e `Fornece` para propagação de Chaves Estrangeiras (FK), sustentando os relacionamentos N:N originais e garantindo a integridade referencial.
<img width="922" height="555" alt="Captura de tela 2026-03-05 163629" src="https://github.com/user-attachments/assets/c207f3a9-bcff-4ab5-be70-9c200d40e35b" />
<img width="850" height="551" alt="Captura de tela 2026-03-05 163458" src="https://github.com/user-attachments/assets/12d84f41-92b7-4835-8087-f5b43b807816" />
<img width="685" height="529" alt="Captura de tela 2026-03-05 163322" src="https://github.com/user-attachments/assets/7fbb0a0e-09ec-4a10-af6e-fe416ea81af0" />

## 📂 Arquivos do Projeto

<img width="876" height="512" alt="DIAGRAMA CONCEITUAL DIS" src="https://github.com/user-attachments/assets/a652c215-957b-4224-8951-9be71c8dd081" />  Imagem do DER.
<img width="685" height="529" alt="DIAGRAMA LOGICO DIS" src="https://github.com/user-attachments/assets/0b0fc1ee-d489-4406-b0e8-a205096d9927" /> Imagem do modelo relacional lógico.

O ARQUIVO DO PROJETO VAI SER POSTADO
