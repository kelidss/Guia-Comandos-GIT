# Guia Básico de Git

### Este README fornece uma introdução aos comandos básicos do Git, permitindo que você inicie facilmente com controle de versão e repositórios remotos.


````git config --global user.name "Seu Nome"````

````git config --global user.email "seuemail@exemplo.com"````

### Iniciando um Repositório

#### Para começar a usar o Git em um novo projeto, você deve inicializar um repositório Git.

````git init````

### Fazendo Commit

#### Após fazer mudanças nos arquivos, você pode rastreá-las e salvá-las com um commit.

#### Adicione os arquivos que você deseja commitar:

````git add nome_do_arquivo````

#### Para adicionar todos os arquivos modificados:

````git add .````

#### Faça o commit das mudanças:

````git commit -m "Mensagem descritiva sobre a mudança"````

### Visualizando o Status

#### Antes de fazer commit, é uma boa prática verificar o status do seu repositório para ver quais arquivos foram modificados.

````git status````

#### Esse comando mostra:

Quais arquivos foram modificados.

Quais arquivos estão prontos para commit.

Quais arquivos não estão sendo rastreados.

### Comparando Mudanças

#### O comando git diff é usado para visualizar as mudanças feitas nos arquivos antes de fazer um commit.

#### Para ver as mudanças nos arquivos que ainda não foram adicionados para commit:

````git diff````

#### Para ver as mudanças nos arquivos que já foram adicionados (staged) para commit:

````git diff --staged````

### Desfazendo Mudanças

#### Se você precisar desfazer mudanças em arquivos ou commits, Git oferece várias opções:

#### Para desfazer mudanças em um arquivo modificado (antes de fazer commit):

````git checkout -- nome_do_arquivo````

#### Para remover um arquivo da área de staging:

````git reset nome_do_arquivo````

#### Para desfazer o último commit, mantendo as mudanças nos arquivos:

````git reset --soft HEAD~````

#### Para desfazer o último commit e descartar as mudanças:

````git reset --hard HEAD~````

### Trabalhando com Branches

#### Branches são ramificações do seu código que permitem trabalhar em diferentes partes do projeto sem afetar a base principal.

#### Para criar uma nova branch:

````git branch nome_da_branch````

#### Para mudar para uma branch existente:

````git checkout nome_da_branch````

#### Para criar e mudar para uma nova branch ao mesmo tempo:

````git checkout -b nome_da_branch````

#### Para listar todas as branches:

````git branch````

#### Para mesclar uma branch na branch atual:

````git merge nome_da_branch````

#### Para deletar uma branch:

````git branch -d nome_da_branch````

### Trabalhando com Remotos (Git)

#### Você pode conectar seu repositório local a um repositório no Git.

#### Para adicionar um repositório remoto:

````git remote add origin https://github.com/seu_usuario/nome_do_repositorio.git````

#### Verifique se o remoto foi adicionado corretamente:

````git remote -v````

### Clonando um Repositório

#### Para copiar um repositório existente do Git para o seu ambiente local:

````git clone https://github.com/seu_usuario/nome_do_repositorio.git````

### Enviando Mudanças para o Git

#### Após fazer commits localmente, você pode enviar suas mudanças para o Git.

````git push origin nome_da_branch````

#### Se for a primeira vez que você está enviando uma branch

````git push --set-upstream origin nome_da_branch````

### Fazendo Pull de Mudanças

#### Para atualizar seu repositório local com as mudanças feitas no Git:

````git pull origin nome_da_branch````

### Resolvendo Conflitos

#### Conflitos ocorrem quando mudanças incompatíveis são feitas no mesmo arquivo. Para resolver:

#### Edite os arquivos conflitantes para resolver os conflitos.

#### Adicione os arquivos resolvidos

````git add nome_do_arquivo````

#### Faça um commit de resolução

````git commit -m "Resolvendo conflitos"````

### Contribuindo para Projetos

#### Se você deseja contribuir para um projeto:

#### Faça um fork do repositório no Git.

#### Clone seu fork para o seu ambiente local

````git clone https://github.com/seu_usuario/nome_do_fork.git````

#### Crie uma nova branch para suas mudanças

````git checkout -b minha_feature````

#### Após fazer suas mudanças, faça commit e envie para o Git

````git push origin minha_feature````

#### Crie um Merge Request no repositório original para revisar e, eventualmente, mesclar suas mudanças.
