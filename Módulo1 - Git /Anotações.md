## 1 - O que são softwares de controle de versão ?

<p>
São sistemas que tem como intuito, realizar o monitoramento, e o controle
do estado atual de versões de um código, facilitando
e deixando o desenvolvimento de certo modo mais organizado.
existem varios softwares com esta finalidade, como:
git, o Subversion, CVS, TFS, Mercurial, entre outros.
</p>

### 1.1 - O que é o git ?

<p>
É um software de controle de versão. é utilizado para controlar e monitorar
as versões e as alterações de determinado código, sendo o mais famoso 
neste quesito. É um software de versão distribuido
(DVCS).
</p>
<br>
<br>
<div align="center">
<img width="347" height="145" alt="image" src="https://github.com/user-attachments/assets/ce86bacd-ef07-4e88-aa20-93405417fbca" />
</div>
<br>

## 2 - Versionamento Distribuido x Centralizado

<p>Os softwares de versionamento podem ser separados em duas categorias: Distribuido <strong>(DVCS)</strong> e Centralizado. </p>


### 2.1 - Centralizado
<p>
Em um sistema centralizado, o principal 
objeto de controle, esta disponivel apenas em um servidor central. 
Para cada alteração que cada Desenvolvedor necessite realizar, primeiro
devem fazer o Dowload da versão mais recente do codigo, que esta centralizado
no servidor, após as alterações serem feitas, o código é reenviado para 
o servidor.
</p>

### 2.2 - Distribuido
<p>
Apesar de possuir o mesmo objetivo dos sistemas centralizados
a dinamica de um sistema Distribuido é significativamente oposta.
Em vez de possuir apenas uma servidor que disponibiliza o objeto
de controle, os Desenvolvedores possuem em seus respectivos computadores
um repositorio pŕoprio, esse repositorio contém todas as ramificações
e todo o histórico do código.
</p>

## 3 - Trabalhando com o git

<p>Para entendermos como o git atua, vamos ver alguns conceitos chave, entre
eles: commits, branchs, merge e repositorios remotos.</p>

### 3.1 - Commit


<p>O commit é o comando em que, adiciona as alterações mais recentes ao código.
Em cada commit, pode-se adicionar um comentário com detalhes sobre o commit
e quais alterações foram realizadas. É de extrema importancia comentar cada commit
realizado, para manter o controle entendivel e organizado.
</p>
<div align="center">
<img width="338" height="400" alt="image" src="https://github.com/user-attachments/assets/0895b743-e960-4db0-bc26-b03dc2b1aac3" />
<br>
<br>
<figcaption>
<strong>Figura 3.1</strong> - A imagem ilustra os estagios do controle do repositório. Primeiro quando realizada a alteração do codigo
o objeto de monitoramento ainda esta no chamado "Working Directory", para adicionar a mudança, é executado o comando "$ git add", o qual
está preparando a mudança e a mesma agora encontra-se no estagio de "Stage" onde o objeto vai ser preparado para o commit. Com a alteração 
em staging, pode-se realizar o commit do objeto, salvando as alterações. Assim que é feito o commit, o objeto é transferido para o repositório
Local, onde será realizado o push, enviando a alteração para o repositorio remoto e mudando o projeto. fonte da imagem: https://www.dsebastien.net/2020-05-19-git-concepts-for-newcomers-part-2-git-repository-working-tree-and-staging-area/
</figcaption>
</div>

### 3.2 - Branch (Ramificação)
<p>
É a forma de separar alterações do repositorio principal,
o codigo raiz, por padrão esta na main, quando criada uma branch
é aberta uma ramificação em paralelo com a main, desta forma
trabalha-se no código em linhas diferentes.
</p>

<br>
<br>
<div align="center">
<img width="700" height="345" alt="image" src="https://github.com/user-attachments/assets/5110491c-9375-45e7-9a93-53b58bf986e1" />
<br>
<br>
<br>
<figcaption>
<strong>Figura 3.2</strong> - Na imagem, temos a branch principal sendo a main, e logo em seguida as branches feature e bug, sendo
estas adjascentes a main. fonte da imagem: https://blog.betrybe.com/git/git-branch/
</figcaption>
</div>



### 3.3 - Merge

<p>
Quando utilizamos as Branchs, cada desenvolvedor está
trabalhando em alterações de um mesmo código. Agora, caso
a alteração seja de fato implementada, deve-se realizar o 
Merge. O merge realiza a junção da branch paralela em que 
o desenvolvedor esta trabalhando com a branch (main).
</p>
<div align="center">
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/842f2aca-37f6-4dcf-bfd5-bb2b4cbfb6e3" />
<br>
<br>
<figcaption>
<strong>Figura 3.3</strong> - Na ilustração, um exemplo de como é executado o merge. Há primeiro o commit/push inicial na main, 
depois cria-se uma nova branch e é feito uma alteração junto a outro commit/push, as branches vão sendo trabalhadas em paralelo
até que, quando o commit da branch paralela se tornar uma nova feature, ou ter um progresso significativo no projeto, a
branch será mesclada junto a main, com o merge. fonte da imagem: https://www.develer.com/en/blog/git-how-to-write-commits-and-why/</strong> 
</figcaption>
</div>

### 3.4 - Repositórios Remotos

<p>Repositorios Remotos são versões do seu repositório da maquina local
em um servidor. É crucial para o desenvolvimento em equipe, pois
cada desenvolvedor deverá ter acesso a este repositorio para a 
colaboração.
</p>
<br>
<br>
<div align="center">
<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/2195a957-ba92-4930-8a54-2c58bdbfa5b8" />
<br>
<figcaption>
<strong>Figura 3.4</strong> - Para a colaboração dos repositorios do git, os desenvolvedores parceiros realizarem alterações no repositório, os mesmos devem possuir o acesso ao repositorio remoto do responsavel, Ex: Github, Gitlab, Bitbucket entre outros. fonte da imagem: https://blog.betrybe.com/git/git-push/
</figcaption>
</div>
</div>


## 4 - Primeiros Passos 

### 4.1 Comandos (Trabalhando Sozinho)

#### 4.1.1 - $ git init
<p>Inicia a rastreabilidade e o controle do código.</p>

#### 4.1.2 - $ git clone
<p>Faz um cópia de qualquer repositorio existente para a sua maquina local.</p>

#### 4.1.3 - $ git add
<p>Adiciona as mudanças realizadads para a area de "Staging"</p>

#### 4.1.4 - $ git commit
<p>Salva as alterações realizadas</p>

#### 4.1.5 - $ git log
<p>Histórico de mudanças realizadas</p>


## 5 - Trabalho em Equipe

### 5.1 - Comandos (Em equipe)

#### 5.1.1 - $ git branch
<p>Cria ou lista as branhes existentes></p>

#### 5.1.2 - $ git checkout / git switch
<p>Realiza a troca para outra branch</p>

#### 5.1.3 - $ git merge
<p>faz a união das branches</p>

#### 5.1.4 - $ git pull
<p>traz as atualizações do repositorio remoto</p>

#### 5.1.5 - $ git push
<p>Envia as alterações para o repositório remoto</p>

#### 5.1.6 - $ git remote
<p>Gerencia as conexões</p>

## 6 - Boas praticas
  
### 6.1 - Arquivos

#### 6.1.1 .gitignore
<p>Ignora arquivos não relevantes para o repositório</p>

### 6.2 - Comandos (Boas praticas)

#### 6.2.1 - $ git diff
<p>visualiza as diferenças entre os estados dos arquivos
antes de realizar o commit</p>

#### 6.2.2 - $ git stash
<p>Guarda as alterações de forma temporaria</p>

#### 6.2.3 - $ git reset
<p> Desfaz as alterações realizadas no repositório local </p>
  
#### 6.2.4 - $ git revert
<p>Mesma função do reset, porém com este comando o histórico é mantido</p>

#### 6.2.5 - $ git cherry-pick
<p>realiza o commit de forma espeficia</p>

## 7 - Casos mais Avançados

### 7.1 - Comandos (Avançados)

#### 7.1.1 - $ git cherry-pick
<p>Realiza o commit de uma forma especifica</p>

#### 7.1.2 - $ git apply
<p>Aplica o patch</p>

#### 7.1.3 - $ git rebase
<p>Reescreve o histórico</p>

#### 7.1.4 - $ git tag
<p>Marca versões importantes</p>



