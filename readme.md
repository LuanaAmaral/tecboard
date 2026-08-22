No uso profissional do GitHub, é comum adotar um fluxo de trabalho que protege a integridade do código da main. Para isso, utilizamos branches para implementar modificações, e pull requests para revisar e inserir essas mudanças de forma controlada.

O processo geral segue os seguintes passos:

Criar uma nova branch a partir da main.
Implementar a modificação localmente.
Adicionar e versionar os arquivos (git add e git commit).
Enviar a branch para o repositório remoto (git push).
Abrir um pull request no GitHub.
Após a aprovação do time, a branch é mesclada na main.
Voltar para a main e atualizar seu repositório local (git pull).


Principais comandos do fluxo Git/GitHub
Comando	Descrição

git checkout -b nome-da-branch	Cria e muda para uma nova branch a partir da atual.
git branch	Lista todas as branches existentes no repositório local.
git status	Mostra os arquivos modificados e o estado da branch atual.
git add .	Adiciona todas as modificações para serem incluídas no próximo commit.
git add nome-do-arquivo	Adiciona apenas um arquivo específico.
git commit -m "mensagem"	Cria um commit com as mudanças adicionadas.
git log --oneline	Exibe o histórico de commits de forma resumida.
git push origin nome-da-branch	Envia a branch e seus commits para o repositório remoto (GitHub).
git checkout main	Volta para a branch main.
git pull origin main	Atualiza a main local com as últimas alterações do repositório remoto.
Links de apoio
Documentação oficial do Git
Documentação oficial do GitHub
Git Branching e Pull Requests - GitHub Docs

Esse fluxo ajuda a manter o código da equipe organizado, revisado e seguro, garantindo maior qualidade no desenvolvimento colaborativo.

Obs: Ao tentar enviar a branch com "push origin nome-da-branch" deu um erro que já existia, precise rodar o código abaixo para alterar a origem
 : para alterar a origem git push --set-upstream origin feat/aumenta-fonte-titulo