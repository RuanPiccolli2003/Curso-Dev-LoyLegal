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

<div align="center">
<img width="347" height="145" alt="image" src="https://github.com/user-attachments/assets/1890df14-f6ae-4ba1-a8ed-84a91c05c9c8" />
</div>

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


### 3.2 - Branch (Ramificação)
<p>
É a forma de separar alterações do repositorio principal,
o codigo raiz, por padrão esta na main, quando criada uma branch
é aberta uma ramificação em paralelo com a main, desta forma
trabalha-se no código em linhas diferentes.
</p>

<div align="center">
<img width="500" height="145" alt="image" src="https://github.com/user-attachments/assets/5110491c-9375-45e7-9a93-53b58bf986e1" />
<figcaption>
Figura - 2.1
</figcaption>
</div>

### 3.3 - Merge

<p>
Quando utilizamos com as Branchs, cada desenvolvedor está
trabalhando em alterações de um mesmo código. Agora, caso
a alteração seja de fato implementada, deve-se realizar o 
Merge. O merge realiza a junção da branch paralela em que 
o desenvolvedor esta trabalhando com a branch (main).
</p>

### 3.4 - Repositórios Remotos

Repositorios Remotos são versões do seu repositório da maquina local
em um servidor. É crucial para o desenvolvimento em equipe, pois
cada desenvolvedor deverá ter acesso a este repositorio para a 
colaboração.


## 4 - Primeiros Passos 

### 4.1 Comandos (Trabalhando Sozinho)

#### 4.1.1 - git init
<p>Inicia a rastreabilidade e o controle do código.</p>

#### 4.1.2 - git clone
<p>Faz um cópia de qualquer repositorio existente para a sua maquina local.</p>

#### 4.1.3 - git add
<p>Adiciona as mudanças realizadads para a area de "Staging"</p>

#### 4.1.4 - git commit
<p>Salva as alterações realizadas</p>

#### 4.1.5 - git log
<p>Histórico de mudanças realizadas</p>


## 5 - Trabalho em Equipe

### 5.1 - Comandos (Em equipe)

#### 5.1.1 - git branch
<p>Cria ou lista as branhes existentes></p>

#### 5.1.2 - git checkout / git switch
<p>Realiza a troca para outra branch</p>

#### 5.1.3 - git merge
<p>faz a união das branches</p>

#### 5.1.4 - git pull
<p>traz as atualizações do repositorio remoto</p>

#### 5.1.5 - git push
<p>Envia as alterações para o repositório remoto</p>

#### 5.1.6 - git remote
<p>Gerencia as conexões</p>

## 6 - Boas praticas
  
### 6.1 - Arquivos

#### 6.1.1 .gitignore
<p>Ignora arquivos não relevantes para o repositório</p>

### 6.2 - Comandos (Boas praticas)

#### 6.2.1 - git diff
<p>visualiza as diferenças entre os estados dos arquivos
antes de realizar o commit</p>

#### 6.2.2 - git stash
<p>Guarda as alterações de forma temporaria</p>

#### 6.2.3 - git reset
<p> Desfaz as alterações realizadas no repositório local </p>
  
#### 6.2.4 - git revert
<p>Mesma função do reset, porém com este comando o histórico é mantido</p>

#### 6.2.5 - git cherry-pick
<p>realiza o commit de forma espeficia</p>

## 7 - Casos mais Avançados

### 7.1 - Comandos (Avançados)

#### 7.1.1 - git cherry-pick
<p>Realiza o commit de uma forma especifica</p>

#### 7.1.2 - git apply
<p>Aplica o patch</p>

#### 7.1.3 - git rebase
<p>Reescreve o histórico</p>

#### 7.1.4 - git tag
<p>Marca versões importantes</p>



