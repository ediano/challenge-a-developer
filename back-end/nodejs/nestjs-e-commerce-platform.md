# Plataforma de e-commerce: Desafio de Microservice com NestJS e Redis

O usuário final deve ser capaz de se cadastrar na plataforma, adicionar produtos no carrinho de compra e finalizar o pedido, no final ele deve ser notificado via e-mail que a compra foi concluída;

### Requisitos: O Projeto deve ter

* CRUD de usuário
* CRUD de informações pessoais
* CRUD de produtos
* CRUD de carrinho de compras
* Auth Local
* Auth Google
* Serviço de envio de e-mail
* Banco de dados SQL

**Dicas:** use _monorepo_ com _NestJS_ para dividir a API dos serviços que usam _Redis_;

**Adicionais (_opcional_)**: O usuário também pode definir como padrão o endereço de entrega e forma de pagamento, como boleto, cartão, PIX e outros métodos; se tiver tempo, permita que este usuário defina vários endereço como, endereço de faturamento e endereço entrega;

1. O usuário deve ser capaz de se cadastrar na plataforma e definir suas informações pessoais, como e-mail, CPF (fake), endereço completo;

**Dica:** Para listagem de regiões, estados e cidades, pode ser usada a API do IBGE.

2. Os endpoints de produtos, deve ser capaz de listar apenas os produto em estoque, aqui fica a dica;

3. O usuário poderá adicionar no carrinho, apenas produto disponível em estoque, também deve ser possível remover o produto do carrinho, defina um CRUD completo neste caso.

4. Quando o usuário for finalizar a compra, ele deve informar a forma de pagamento, para validar essas informações, pode ser criado uma regra fake, onde o pagamento foi confirmado, negado ou cancelado.

5. Ao finalizar o processo de pagamento, o usuário deve ser notificado via e-mail sobre o status da comprar (sucesso, negada ou pedido cancelado).

> **Requisito:** Todo os serviços de envio de e-mail, deve acontecer do lado do Redis, isso evita gargalo na API após a finalização do pedido;

**Dica:** Como lib de envio de e-mail, pode ser usado o Nodemailer, para gerar e-mail fakes, pode ser usado o Ethereal.

Depois de tudo isso é só publicar o projeto no GitHub.

### Links úteis 

_API do IBGE: https://servicodados.ibge.gov.br/api/docs/localidades_

_Lib Nodemailer: https://nodemailer.com_

_Service Ethereal: https://ethereal.email_
