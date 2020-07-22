# Mauro Mattos - Conquistas Técnicas

Documento onde registro meus aprendizados e experiências técnicas na minha vida como desenvolvedor

### Back End

#### PHP

Com o CodeIgniter pude contribuir no desenvolvimento de uma  uma aplicação de gerenciamento completo de um e-commerce. A aplicação controlava diversos fluxos do vendedor, como:

- Gerenciamento de estoque
- Gerenciamento de produtos
- Evolução de pedidos/Vendas
- Contatos de fornecedores
- Compra de produtos para o estoque

Desenvolvi diversar telas para o sistema utilizando componentes pré-estilizados do template __Gentelella__

Realizei também integrações do sistema com sites de comércio eletrônico, como:
- B2W (Americanas.com)
- Magazine Luiza

> Ferramentas/bibliotecas utilizadas: CodeIgniter 2, Gentelella

#### Python

 Com o Scrapy desenvolvi Web Crawlers para a coleta de informações de diversos sites de E-Commerce

 > Ferramentas/bibliotecas utilizadas: requests, scrapy, google-cloud, aws, etc.

### Continuous Integration

#### Ferrameta utilizada - GitLab CI

Antes da implementação, o processo de deploy das aplicações que eu eram gerenciadas pela minha equipe era realizado através dos seguintes passos:

1. Gerar o build da aplicação manualmente com o comando de `yarn build` do projeto
2. Entrar no AWS S3 e apagar os arquivos da build atual
3. Realizar o upload dos novos arquivos gerados na build
4. Apagar arquivos locais gerados na build

Após a configuração do GitLab CI, o fluxo de deploy foi alterado para:

1. Ao fazer o merge de um PR para uma branch específica (`develop` ou `master`), o processo era iniciado e o build e deploy das aplicações eram executados na nuvem.

> Ganhos técnicos: GitLab CI
