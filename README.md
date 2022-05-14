# Git Flow

Neste repositório você vai entender como utilizar os comandos git para criar uma PR e entender o fluxo de trabalho com o git.

### Develop
Sempre que for trabalhar em "Desenvolvimento" você deve ir para a branch **develop**, atualiza-la e logo após criar uma branch a partir da mesma.

```
git checkout develop // ir para a branch develop
git fetch origin // atualizar local com o github
git pull origin develop // atualizar sua develop com a develop do github
git checkout -b your-branch // criar uma branch nova a partir da develop
```

Logo após você deve fazer as suas alterações na sua branch nova.

Ao concluir o seu trabalho você deve fazer o processo de commit

### Commitando
1. Primeiramente rode o comando **git status**, ele vai te mostrar os arquivos que você adicionou, alterou ou removeu

2. Depois adicione os arquivos desejados utilizando o comando **git add <caminho-do-arquivo>**

3. Caso queira adicionar todos os arquivos de uma vez, rode **git add .**, o . (ponto) significa "todos os arquivos" no comando git.

4. Crie um commit com um título, este título deve sempre iniciar com uma dessas palavras: Adicionado, Criado, Alterado, Removido, Corrigido. Seguido de uma frase que faz sentido com suas alterações. Então rode **git commit -m "Adicionado nova tela de login"** por exemplo.

5. Em alguns projetos ao rodar **git commit -m** pode dar algum erro, por que o projeto pode verificar que há algum erro de formatação ou algo no código. Caso isso aconteça, leia o error, corrija o erro e faça o mesmo processo a partir do tópico #1 novamente.

6. Suba suas alterações para o github rodando **git push origin your-branch**

7. Em alguns projetos a validação de erros está no comando **git push** ao invés do **git commit**. Caso o verificador aponte algum erro de formatação ou de código, leia o erro, corrija e faça o mesmo processo a partir do tópico #1.

Resumidamente os comandos são:
```
git status
git add .
git commit -m "Your title"
git push origin your-branch
```

### Pull Request
Se seu procedimento de Commitar deu certo. Só tenho duas palavras pra você:

# Para - Béns

Agora você pode pode entrar no repositorio do github, lá vai aparecer que uma nova branch foi criada, o que deve ser a sua nova branch.

1. Logo ao lado haverá um botão **Compare && pull request**, clique nele.
2. Aponte a sua branch para a **develop**
3. Adicione um título compatível com a tarefa que você fez
4. Na descrição da PR cole o link da task do Jira no topo, depois uma breve descrição do que foi feito, screenshots e videos são muito bem vindos para entender melhor o que foi feito.
5. Clique em **Create pull request**
6. Adicione agora o link da(s) PR(s) criada(s) no comentário da task do Jira e também no canal #pull-requests do Discord

