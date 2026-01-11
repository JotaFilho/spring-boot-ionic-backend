Sistema de Pedidos - Curso Spring Boot
Este projeto é uma API REST desenvolvida durante o curso "Java Spring Boot, Hibernate, JPA, MySQL e H2" do professor Nélio Alves. O sistema simula o backend de uma plataforma de e-commerce com gerenciamento de produtos, categorias, clientes e pedidos.

🛠️ Tecnologias Utilizadas
Java 17/21

Spring Boot 3

Spring Data JPA

Hibernate (ORM)

H2 Database (Banco de dados de teste em memória)

MySQL (Banco de dados de produção)

Jackson (Serialização JSON)

Maven (Gerenciador de dependências)

📌 Principais Funcionalidades
Modelo de Domínio Complexo: Implementação de associações Muitos-para-Muitos com atributos extras (ItemPedido).

Mapeamento de Chaves Compostas: Utilização de @Embeddable e @EmbeddedId.

Persistência de Dados: Criação de repositórios para todas as entidades.

Instanciação Automática: Carga inicial de dados para testes via CommandLineRunner.

Tratamento de Loops Infinitos: Gerenciamento de referências cíclicas em JSON com @JsonIgnore e anotações Jackson.

🏗️ Modelo Conceitual
O sistema possui uma estrutura robusta que conecta as seguintes entidades:

Categorias e Produtos: Relacionamento N:N.

Clientes, Telefones e Endereços: Um cliente pode ter vários endereços e telefones.

Pedidos e Pagamentos: Suporte para diferentes tipos de pagamento (Cartão e Boleto) usando herança.

Itens de Pedido: Classe de associação para registrar preço, quantidade e desconto no momento da venda.
<img width="1898" height="945" alt="image" src="https://github.com/user-attachments/assets/2442d341-2e38-4e12-83af-39da873d6cd0" />

<img width="1465" height="942" alt="image" src="https://github.com/user-attachments/assets/a4140498-0ece-43f5-9ad1-b2cf8523dc7b" />



🚀 Como executar o projeto
Clone o repositório:

Bash

git clone https://github.com/seu-usuario/nome-do-repositorio.git
Importe no STS/Eclipse:

File -> Import -> Existing Maven Projects.

Execute a aplicação:

Clique com o botão direito na classe CursomcApplication -> Run As -> Spring Boot App.

Acesse o banco H2:

URL: http://localhost:8080/h2-console

JDBC URL: jdbc:h2:mem:testdb

User: sa | Pass: (vazio)

✍️ Autor
Desenvolvido por José Filho durante o curso do Prof. Nélio Alves.
