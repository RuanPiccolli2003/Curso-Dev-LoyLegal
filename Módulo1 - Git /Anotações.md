## O que são softwares de controle de versão ?

<p>
São sistemas que tem como intuito, realizar o monitoramento, e o controle
do estado atual de versões de um código, facilitando
e deixando o desenvolvimento de certo modo mais organizado.
existem varios softwares com esta finalidade, como:
git, o Subversion, CVS, TFS, Mercurial, entre outros.
</p>

### O que é o git ?

<p>
É um software de controle de versão. é utilizado para controlar e monitorar
as versões e as alterações de determinado código, sendo o mais famoso 
neste quesito. É um software de versão distribuido
(DVCS).
</p>

## Versionamento Distribuido x Centralizado

<p>Os softwares de versionamento podem ser separados em duas categorias: Distribuido <strong>(DVCS)</strong> e Centralizado. </p>


### Centralizado
<p>
Em um sistema centralizado, o principal 
objeto de controle, esta disponivel apenas em um servidor central. 
Para cada alteração que cada Desenvolvedor necessite realizar, primeiro
devem fazer o Dowload da versão mais recente do codigo, que esta centralizado
no servidor, após as alterações serem feitas, o código é reenviado para 
o servidor.
</p>

### Distribuido
<p>
Apesar de possuir o mesmo objetivo dos sistemas centralizados
a dinamica de um sistema Distribuido é significativamente oposta.
Em vez de possuir apenas uma servidor que disponibiliza o objeto
de controle, os Desenvolvedores possuem em seus respectivos computadores
um repositorio pŕoprio, esse repositorio contém todas as ramificações
e todo o histórico do código.
</p>

## Trabalhando com o git

<p>Para entendermos como o git atua, vamos ver alguns conceitos chave, entre
eles: commits, branchs, merge e repositorios remotos.</p>

### Commit

<p>O commit é o comando em que, adiciona as alterações mais recentes ao código.
Em cada commit, pode-se adicionar um comentário com detalhes sobre o commit
e quais alterações foram realizadas. É de extrema importancia comentar cada commit
realizado, para manter o controle entendivel e organizado.
</p>


### Branch (Ramificação)
<p>
É a forma de separar alterações do repositorio principal,
o codigo raiz, por padrão esta na master, quando criada uma branch
é aberta uma ramificação em paralelo com a master, desta forma
trabalha-se no código em linhas diferentes.
</p>

### Merge

<p>
Quando utilizamos com as Branchs, cada desenvolvedor está
trabalhando em alterações de um mesmo código. Agora, caso
a alteração seja de fato implementada, deve-se realizar o 
Merge. O merge realiza a junção da branch paralela em que 
o desenvolvedor esta trabalhando com a branch (master).
</p>

### Repositórios Remotos

Repositorios Remotos são versões do seu repositório da maquina local
em um servidor. É crucial para o desenvolvimento em equipe, pois
cada desenvolvedor deverá ter acesso a este repositorio para a 
colaboração.


## Primeiros Passos (Trabalhando sozinho)

### Comandos

#### git init
<p>Inicia a rastreabilidade e o controle do código.</p>

#### git clone
<p>Faz um cópia de qualquer repositorio para a sua maquina local.</p>










