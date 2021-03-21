# kabug-rb
Repositorio para testar Jenkins

## Como Executar o Projeto
* importante ter o Ruby instalado (versão 2.5 ou superior)

## Instalar o Bundler
`
gem install bundler
`

## Instalar as dependências do Ruby (projeto)
`
bundle install
`
### Executa em modo local
`
bundle exec cucumber
`

### Executar no servidor de CI gerando reports JSON
`
bundle exec cucumber -p ci
