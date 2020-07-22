# Mauro Mattos - Conquistas Técnicas

Desenvolvi esse repositório para registrar minhas conquistas técnicas ao longo do tempo.

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
