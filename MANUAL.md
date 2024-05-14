# [MANUAL](https://guides.rubyonrails.org/getting_started.html)
## INSTALAÇÃO:
### 1. INSTALANDO O RAILS:
- [SE VOCÊ AINDA NÃO INSTALOU O RUBY, ACESSE AO CURSO](https://github.com/VILHALVA/CURSO-DE-RUBY)

1. Com o Ruby instalado, você pode instalar o Rails usando o gerenciador de pacotes RubyGems. Abra o terminal e digite o seguinte comando:
   ```
   gem install rails
   ```

2. Aguarde até que todas as dependências sejam instaladas. Isso pode levar algum tempo, dependendo da velocidade da sua conexão com a internet.

### 2. VERIFICANDO A INSTALAÇÃO:
Depois de instalar o Rails, você pode verificar se foi instalado corretamente digitando o seguinte comando no terminal:
```
rails --version
```
Isso deve exibir a versão do Rails que foi instalada.

### 3. CRIANDO UM PROJETO:
1. Escolha um editor de código ou IDE para escrever seu código Ruby on Rails. Algumas opções populares incluem Visual Studio Code, Sublime Text, Atom, RubyMine, entre outros.

2. Crie um novo diretório para o seu projeto Rails e navegue até ele no terminal.

3. Para criar um novo projeto Rails, execute o seguinte comando no terminal:
   ```
   rails new nome_do_projeto
   ```
   Substitua "nome_do_projeto" pelo nome que você deseja dar ao seu projeto.

4. **Navegue até o diretório do projeto**: Use o comando `cd` para entrar no diretório do projeto que você acabou de clonar.

   ```
   cd nome_do_repositorio
   ```

5. Execute o servidor Rails usando o seguinte comando:
  **LINUX/MACOS:**
   ```
   bin/rails server
   ```

   **WINDOWS:**
   ```
   ruby bin\rails server
   ```

6. Abra um navegador da web e vá para `http://localhost:3000` para ver sua aplicação Rails em execução.

## IMPORTAÇÃO:
Quando você baixa um projeto do GitHub que é desenvolvido em Ruby on Rails e deseja executá-lo em seu ambiente local, geralmente precisa instalar todas as dependências do projeto antes de iniciar o servidor.

1. **Instale as dependências do Ruby**: Normalmente, as dependências do Ruby são gerenciadas pelo Bundler. Execute o comando `bundle install` para instalar todas as gemas listadas no arquivo `Gemfile` do projeto.

   ```
   bundle install
   ```

   Isso irá baixar e instalar todas as gemas necessárias especificadas no `Gemfile`, incluindo as versões específicas, se houver.

2. **Configuração do banco de dados (se necessário)**: Se o projeto usar um banco de dados, como o PostgreSQL ou o MySQL, você também pode precisar criar um banco de dados localmente e configurar o arquivo `config/database.yml` com suas credenciais de banco de dados.

3. **Executar migrações do banco de dados (se necessário)**: Se houver migrações de banco de dados pendentes, você precisará executá-las usando o comando `rails db:migrate`.

   ```
   rails db:migrate
   ```

4. **Inicie o servidor Rails**: Depois de instalar as dependências e configurar o banco de dados (se necessário), você pode iniciar o servidor Rails usando o comando `rails server` ou `rails s`.
  **LINUX/MACOS:**
   ```
   bin/rails server
   ```

   **WINDOWS:**
   ```
   ruby bin\rails server
   ```

Agora, seu servidor Rails local deve estar funcionando e você pode acessar sua aplicação em `http://localhost:3000` no seu navegador da web.

## DIRETÓRIOS:
```
📁 CURSO DE RUBY ON RAILS
  📁 bin
    - Scripts executáveis
  📁 config
    - Configurações do aplicativo (banco de dados, rotas, etc.)
  📁 db
    - Arquivos relacionados ao banco de dados (migrações, esquemas, sementes, etc.)
  📁 lib
    - Código de bibliotecas adicionais
  📁 log
    - Arquivos de log
  📁 public
    - Recursos públicos acessíveis diretamente pelo navegador (imagens, CSS, JS)
  📁 test
    - Testes automatizados
  📁 tmp
    - Arquivos temporários
  📁 vendor
    - Dependências de terceiros
  📄 Gemfile
    - Lista de gemas (dependências) do projeto
  📄 Gemfile.lock
    - Registro das versões específicas das gemas instaladas
  📄 README.md
    - Documentação do projeto em Markdown
```

Agora, uma breve explicação de cada diretório:

- **bin:** Este diretório contém scripts executáveis relacionados ao projeto. Por exemplo, scripts para iniciar o servidor Rails, executar tarefas de rake, etc.
  
- **config:** Aqui é onde você configura seu aplicativo Rails. Isso inclui arquivos para configuração do banco de dados, configuração de rotas, inicialização do aplicativo, etc.
  
- **db:** Todos os arquivos relacionados ao banco de dados ficam aqui. Isso inclui migrações de banco de dados, esquemas de banco de dados, arquivos de sementes (para preencher o banco de dados com dados de teste) e muito mais.
  
- **lib:** Se você tiver código que não se encaixa nas convenções padrão do Rails, pode colocá-lo aqui. Isso poderia ser código que você escreveu para ser compartilhado entre diferentes partes do seu aplicativo ou até mesmo código que você está desenvolvendo como uma biblioteca separada.
  
- **log:** Os arquivos de log do seu aplicativo são armazenados aqui. Isso inclui logs de desenvolvimento, produção e testes.
  
- **public:** Este é o diretório onde você coloca arquivos estáticos que podem ser acessados diretamente pelo navegador, como imagens, folhas de estilo CSS e scripts JavaScript.
  
- **test:** Aqui é onde você mantém seus testes automatizados. Isso inclui testes unitários, testes de integração e testes de aceitação.
  
- **tmp:** O diretório tmp é usado para armazenar arquivos temporários. Isso pode incluir uploads de arquivos temporários ou outros dados que não precisam ser persistentes.
  
- **vendor:** Este diretório é usado para armazenar dependências de terceiros que não são gerenciadas pelo Bundler (gerenciador de dependências do Ruby). Isso geralmente inclui bibliotecas JavaScript e CSS.
  
- **Gemfile:** O arquivo Gemfile é onde você especifica as gemas (dependências) necessárias para o seu aplicativo. Isso permite que você defina quais bibliotecas Ruby seu aplicativo precisa e suas versões.
  
- **Gemfile.lock:** Este arquivo registra as versões específicas das gemas instaladas em seu ambiente de desenvolvimento. Ele garante que todos os membros da equipe estejam usando as mesmas versões de gemas.
  
- **README.md:** Um arquivo Markdown que contém informações sobre o projeto. Geralmente é usado para fornecer uma visão geral do projeto, instruções de instalação e outras informações úteis para os colaboradores.



