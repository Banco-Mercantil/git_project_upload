## Carregar projeto DBT no GitHub:

O real objetivo deste trabalho é demonstrar, passo a passo, como realizar o upgrade de um projeto *DBT* já existente no repositório do GitHub.


## 🚀 Inicializando o projeto:

Para iniciar, a título de segurança, iremos copiar o projeto que desejamos para nossa repartição de disco ``C:\``.

Na sequência, para migrar um projeto DBT já existente no GitHub, precisamos verificar se o projeto já possui a pasta ``.git``.

O diretório Git é onde o Git armazena os metadados e o banco de dados de objetos de seu projeto e é copiado quando você clona um repositório de outro computador. O diretório de trabalho é uma simples cópia de uma versão do projeto. Esses arquivos são pegos do banco de dados compactado no diretório Git e colocados no disco para você usar ou modificar.

Para veririfcar a existencia da pasta ``.git`` no projeto, vamos abri-ló no próprio *explorador de arquivos*. Caso o diretório Git não esteja visível, verique se ele não está oculto na pasta. Acesse o *Visualizar*, no menu superior, clique em *Mostrar* e marque a opção *itens ocultos*.

<img width="928" alt="image" src="https://github.com/Banco-Mercantil/git_project_upload/assets/88452990/c9e369eb-0896-4578-8133-952080aa87c7">

Neste momento, caso o diretório apareça, delete-o. Caso não tenha aparecido, podemos seguir em frente.

No browser, acesse a sua conta do [GitHub](https://github.com/login). Na guia *Repositories*, clique no botão *New reposity* para criar um projeto.

<img width="793" alt="image" src="https://github.com/Banco-Mercantil/git_project_upload/assets/88452990/509cdcce-04b9-4cbe-a70a-c5e9d272a7a5">

Um novo pop-up será aberto, nomeie o repositório, defina-o como público ou privado e marque a opção *Add a README file*.

<img width="442" alt="image" src="https://github.com/Banco-Mercantil/git_project_upload/assets/88452990/00c8851e-0e80-4532-9a0a-31d5fdeb9eee">

Acesse o terminal da sua máquina
  - Aperte as teclas ``Iniciar + r``
  - Digite ``cmd`` no box
  - Aperte ``Enter``

<img width="334" alt="image" src="https://github.com/Banco-Mercantil/git_project_upload/assets/88452990/4bd707b5-c024-40c2-92c5-82aa5ac92d16">

Navegue, pelo terminal, até a pasta em que o projeto que se deseja migrar para o GitHub está. Utilize o comando ``cd``.

``cd C:\Users\B045523\Documents\pamella\dbt_efet_campanhas_incentivo_rede_mai24 ``

Já dentro da pasta, digite o comando, para inicializar um repositório Git:

``git init``

Seu terminal exibirá a seguinte mensagem:

``Initialized empty Git repository in C:/Users/B045523/Documents/pamella/dbt_efet_campanhas_incentivo_rede_mai24/.git/``

Feito isso, vamos adicionar todos os arquivos modificados do projeto ao processo de migração:

``git add .``

Para verificar se os pacotes foram adicionados, execute o comando ``git status`` e o terminal irá exibir a quantidade de arquivos modificados.

<img width="702" alt="image" src="https://github.com/Banco-Mercantil/git_project_upload/assets/88452990/3b7b3d17-3ff9-40e7-9b6e-80f6977263f9">

Crie a branch ``main``:

``git branch -M main``

Vá ao repositório criado no GitHub, expanda o botão *<> Code* e copie a url HTTPS

<img width="560" alt="image" src="https://github.com/Banco-Mercantil/git_project_upload/assets/88452990/a961f2d0-c169-42db-b000-27ea803d1f2d">

Cole a url com o seguinte comando para adicionar um novo repositório remoto:

``git remote add origin url_https``

Na sequência, dê o comando ``push``, junto à url, para empurrar o projeto para o repositório no GitHub:

``git push url_https main -f``

O terminal deverá informar a conclusão do processo.

<img width="529" alt="image" src="https://github.com/Banco-Mercantil/git_project_upload/assets/88452990/302c3f01-c877-4bf0-8ba9-96ab3ebbf167">








