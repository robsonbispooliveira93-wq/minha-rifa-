# Guia de início rápido para repositórios

Saiba como criar um novo repositório e realizar o seu primeiro commit em 5 minutos.

## Criar um repositório

Os repositórios do GitHub armazenam uma variedade de projetos. Neste guia, você criará um repositório e fará commit da sua primeira alteração.

<div class="ghd-tool webui">

1. No canto superior direito de qualquer página, selecione <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-plus" aria-label="Create something new" role="img"><path d="M7.75 2a.75.75 0 0 1 .75.75V7h4.25a.75.75 0 0 1 0 1.5H8.5v4.25a.75.75 0 0 1-1.5 0V8.5H2.75a.75.75 0 0 1 0-1.5H7V2.75A.75.75 0 0 1 7.75 2Z"></path></svg> e clique em **Novo repositório**.

   ![Captura de tela de um menu suspenso GitHub mostrando as opções para criar novos itens. Há um item de menu "Novo repositório" com o contorno em laranja escuro.](/assets/images/help/repository/repo-create-global-nav-update.png)
2. Digite um nome breve e memorável para o repositório. Por exemplo, "olá mundo".

   ![Captura de tela da primeira etapa na criação de um repositório. O campo "Nome do repositório" contém o texto "hello-world" e está contornado em laranja escuro.](/assets/images/help/repository/create-repository-name.png)
3. Opcionalmente, adicione uma descrição do repositório. Por exemplo, “Meu primeiro repositório no GitHub".
4. Escolha uma visibilidade do repositório. Para saber mais, confira [Sobre repositórios](/pt/repositories/creating-and-managing-repositories/about-repositories#about-repository-visibility).
5. Alternar **Adicionar LEIAME** para **Ativado**.
6. Clique em **Criar repositório**.

Parabéns! Você criou com sucesso seu primeiro repositório e o inicializou com um arquivo *LEIAME*.

</div>

<div class="ghd-tool cli">

> \[!NOTE]
> Para saber mais sobre GitHub CLI, confira [Sobre GitHub CLI](/pt/github-cli/github-cli/about-github-cli).

1. Na linha de comando, acesse o diretório onde você gostaria de criar um clone local do seu novo projeto.
2. Para criar um repositório para seu projeto, use o subcomando `gh repo create`. Quando solicitado, selecione **Crie um novo repositório no GitHub do zero** e insira o nome do novo projeto. Caso você deseje que o seu projeto pertença a uma organização em vez da sua conta pessoal, especifique o nome da organização e o nome do projeto com `organization-name/project-name`.
3. Siga as instruções interativas. Para clonar o repositório localmente, marque sim quando perguntarem se você deseja clonar o diretório do projeto remoto.
4. Como alternativa, para ignorar os prompts, forneça o nome do repositório e um sinalizador de visibilidade (`--public`, `--private` ou `--internal`). Por exemplo, `gh repo create project-name --public`. Para clonar o repositório localmente, transmita o sinalizador `--clone`. Para obter mais informações sobre possíveis argumentos, consulte o manual da CLI [GitHub](https://cli.github.com/manual/gh_repo_create).

</div>

## Fazer commit da primeira alteração

<div class="ghd-tool webui">

Um [commit](/pt/get-started/learning-about-github/github-glossary#commit) é como um instantâneo de todos os arquivos do seu projeto em determinado momento.

Quando você criou o seu novo repositório, você o inicializou com um arquivo *README*. Os arquivos *LEIAME* são um ótimo lugar para descrever o projeto com mais detalhes ou adicionar alguma documentação (por exemplo, como instalar ou usar o projeto). O conteúdo do arquivo *LEIAME* é mostrado automaticamente na página inicial do repositório.

Vamos fazer commit de uma alteração no arquivo README.

1. Na lista de arquivos do repositório, selecione **README.md**.

![Captura de tela de uma lista de arquivos em um repositório. Um nome de arquivo, "README.md", está realçado com um contorno laranja.](/assets/images/help/repository/create-commit-open-readme.png)

1. No canto superior direito da exibição de arquivo, clique em <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-pencil" aria-label="Edit file" role="img"><path d="M11.013 1.427a1.75 1.75 0 0 1 2.474 0l1.086 1.086a1.75 1.75 0 0 1 0 2.474l-8.61 8.61c-.21.21-.47.364-.756.445l-3.251.93a.75.75 0 0 1-.927-.928l.929-3.25c.081-.286.235-.547.445-.758l8.61-8.61Zm.176 4.823L9.75 4.81l-6.286 6.287a.253.253 0 0 0-.064.108l-.558 1.953 1.953-.558a.253.253 0 0 0 .108-.064Zm1.238-3.763a.25.25 0 0 0-.354 0L10.811 3.75l1.439 1.44 1.263-1.263a.25.25 0 0 0 0-.354Z"></path></svg> para abrir o editor de arquivos.
   ![Captura de tela de um arquivo. No cabeçalho, um botão, rotulado com um ícone de lápis, está contornado em laranja escuro.](/assets/images/help/repository/edit-file-edit-button.png)

2. Na caixa de texto, digite algumas informações sobre você mesmo.

3. Acima do novo conteúdo, clique em **Visualizar**.

   ![Captura de tela de um arquivo no modo de edição. Acima do conteúdo do arquivo, uma guia rotulada "Visualizar" está contornada em laranja escuro.](/assets/images/help/repository/edit-readme-preview-changes.png)

4. Revise as alterações feitas no arquivo. Se você selecionar **Mostrar comparação**, verá o novo conteúdo em verde.

![Captura de tela da visualização de um arquivo. A caixa de seleção "Show diff" está habilitada e as adições ao arquivo são mostradas com uma linha verde. Ambas estão realçadas em laranja.](/assets/images/help/repository/create-commit-review.png)

1. Clique em **Fazer commit das alterações...**

2. No campo "Mensagem do commit", digite uma mensagem curta e relevante que descreva a alteração que você fez no arquivo. Você pode atribuir o commit a mais de um autor na mensagem do commit. Para saber mais, confira [Criar um commit com vários autores ou em nome de uma organização](/pt/pull-requests/how-tos/commit-changes/creating-a-commit-with-multiple-authors).

3. Abaixo dos campos da mensagem de commit, decida se deseja adicionar seu commit ao ramo atual ou a um novo ramo. Se seu branch atual for o branch-padrão, você deverá optar por criar um novo branch para seu commit e, em seguida, criar um pull request. Para saber mais, confira [Como criar uma solicitação de pull](/pt/pull-requests/how-tos/create-pull-requests/creating-a-pull-request).

   ![Captura de tela de um pull request do GitHub mostrando um botão de opção para fazer commit diretamente na branch principal ou criar uma nova branch. A nova ramificação está selecionada.](/assets/images/help/repository/choose-commit-branch.png)

4. Clique em **Fazer commit de alterações** ou em **Propor alterações**.

</div>

<div class="ghd-tool cli">

Agora que você criou um projeto, você pode começar a fazer commit das alterações.

Os arquivos *LEIAME* são um ótimo lugar para descrever o projeto com mais detalhes ou adicionar alguma documentação (por exemplo, como instalar ou usar o projeto). O conteúdo do arquivo *LEIAME* é mostrado automaticamente na página inicial do repositório. Siga estas etapas para adicionar um arquivo *README*.

1. Na linha de comando, acesse o diretório raiz do seu novo projeto. (Esse diretório foi criado quando você executou o comando `gh repo create`).

2. Crie um arquivo *README* com algumas informações sobre o projeto.

   ```shell
   echo "info about this project" >> README.md
   ```

3. Insira `git status`. Você verá que há um arquivo `README.md` não rastreado.

   ```shell
   $ git status

   Untracked files:
     (use "git add <file>..." to include in what will be committed)
     README.md

   nothing added to commit but untracked files present (use "git add" to track)
   ```

4. Stage e commit do arquivo.

   ```shell
   git add README.md && git commit -m "Add README"
   ```

5. Faça push das alterações para seu branch.

   ```shell
   git push --set-upstream origin HEAD
   ```

</div>

## Próximas etapas

Você criou agora um repositório, incluindo um arquivo *README*, e fez seu primeiro commit no GitHub.

<div class="ghd-tool webui">

* Você já pode clonar um repositório do GitHub para criar uma cópia local no computador. A partir do seu repositório local, você pode fazer commit e criar um pull request para atualizar as alterações no repositório upstream. Para saber mais, confira [Clonar um repositório](/pt/repositories/creating-and-managing-repositories/cloning-a-repository) e [Configurar o git](/pt/get-started/git-basics/set-up-git).

</div>

* Proteja seu repositório usando os recursos de segurança disponíveis do GitHub. Para saber mais, confira [Guia de Início rápido para proteger seu repositório](/pt/code-security/getting-started/quickstart-for-securing-your-repository).

* Encontre projetos e repositórios interessantes no GitHub e faça alterações neles criando um fork do repositório. A bifurcação de um repositório permitirá que você faça alterações em outro repositório sem afetar o original. Para saber mais, confira [Criar fork de um repositório](/pt/pull-requests/how-tos/work-with-forks/fork-a-repo).

* Cada repositório em GitHub pertence a uma pessoa ou a uma organização. Você pode interagir com as pessoas, repositórios e organizações conectando-se e seguindo-as.GitHub Para saber mais, confira [Descobrindo projetos no GitHub](/pt/get-started/exploring-projects-on-github/discovering-projects-on-github).

* O GitHub tem uma ótima comunidade de suporte na qual você pode pedir ajuda e conversar com pessoas de todo o mundo. Participe da conversa na [GitHub Community](https://github.com/orgs/community/discussions).# minha-rifa-