
![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/hc_sh_fb_banner.jpg)

# Introdução ao Git e GitHub

Este documento apresenta uma breve introdução ao [**Git**](https://git-scm.com/) e ao [**GitHub**](https://github.com/),
de forma a poderes dominar o essencial para criares um projecto a partir do zero.

Podes melhorar este documento, editando-o, só tens que dominar o git :) 

## Estrutura do manual:
- O que é o Git?
- O que é o GitHub?
- Instalar Git no teu computador
- Criar primeiro repositório no GitHub
- Copiar um repositório do GitHub para o teu computador
- Comandos git mais usados

---

## O que é o Git?
O [git](https://git-scm.com/) é um sistema de controlo de versões distribuído, e um sistema de gestão de código-fonte, 
ou seja, quando escreveres código, podes ir assinalando momentos importantes (`commit`), em que é salvo uma cópia do trabalho, 
podes mais tarde reverter para algum dos pontos anteriores. Também podes sincronizar esse ficheiro com os teus colegas 
de equipa, em que o git automaticamente compara as diferenças e junta as
alterações que as pessoas fizeram. Existem outros protocolos semelhantes ao Git, como por exemplo o Subversion, mas o 
Git é dos mais completos, e dos mais usados.

> **Exemplo de vários commits**
>
> Podes reverter o código para qualquer um dos commits anteriormente assinalados  
>
> ![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/git_commits.png)
>
> **Exemplo de alterações feitas num ficheiro entre dois commits**
>
> ![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/git_diff.png)


Independentemente do teu sistema operativo, vais precisar de instalar o protocolo git, que normalmente é executado na 
linha de comandos, mas para facilitar a vida, podes instalar um GUI para git, de forma a não teres que memorizar os 
comandos todos, e usufruires de todas as vantagens de uma interface gráfica. Podes também instalar algum plugin para 
integrar o git no teu explorador de ficheiros, de forma a conseguires executar algumas ações sem teres que abrir algum 
programa. Podes instalar estes 3 software independentemente, ou podes instalar logo algum que traga tudo incluido.

## O que é o GitHub?
O [GitHub](https://github.com/) é um serviço de "alojamento" de repositórios Git. Grandes projectos opensource costumam
ter o código disponível no GitHub, como por exemplo a [BeeVeryCreative](https://github.com/beeverycreative), a [DJI](https://github.com/dji-sdk), a [bitcoin](https://github.com/bitcoin), o [bitalino](https://github.com/BITalinoWorld), o [arduino](https://github.com/arduino), etc. 
Existem outros serviços semelhantes ao GitHub, como por exemplo o [Bitbucket](https://bitbucket.org/), que te permite 
criar de forma gratuita repositórios privados. Podes também criar o teu próprio servidor de Git, mas visto que estás a 
ler o manual de introdução ao Git, não me parece que devas partir já por esse caminho. :)

Além de poderes alojar o teu código no GitHub, ele também te oferece algumas funcionalidades interessantes, por exemplo,
podes fazer uma gestão dos _issues_ e _features_ a implementar, podes também editar of ficheiros directamente no browser, 
etc.  

## Instalar Git no teu computador

### Windows
No windows, podes instalar o [Git for Windows (https://git-for-windows.github.io/)](https://git-for-windows.github.io/),
que instala automaticamente o protocolo git para executares na linha de comandos, 
um GUI para poderes executar os comandos git por uma interface gráfica, e também se integra no explorador do windows, 
para que possas clicar com o botão do lado direito em cima de documentos do teu repositório e executar comandos.

> **Nota**
>
> Se preferires, pode instalar só o protocolo git pelo site [https://git-scm.com/downloads](https://git-scm.com/downloads),
> e podes escolher um outro GUI à tua escolha, tens alguns dos mais usados nesta página: 
[https://git-scm.com/downloads](https://git-scm.com/downloads). Para integrar o git com o explorador do windows também
podes optar pelo [TortoiseGit](https://tortoisegit.org/)


### Linux
Antes de instalares o git, confirma se já o tens instalado, abre o terminal e executa 

`git --version`
> git version 2.13.0

Caso ainda não tenhas o git instalado, podes instalar o git pelo terminal.
Executa o comando correspondente ao teu sistema operativo:

* Sistemas baseados em Debian, como Ubuntu, Raspbian, Mint, etc.
* *  `sudo apt-get install git-core`

* Sistemas baseados em Red Hat, como CentOS, etc.
* * `sudo yum install git`

### Mac OSx

Antes de instalares o git, confirma se já o tens instalado, abre o terminal e executa 

`git --version`
> git version 2.13.0

Caso ainda não tenhas o git instalado, podes instalar o git por exemplo pelo site do git 
[https://git-scm.com/downloads](https://git-scm.com/downloads)

Para facilitar a utilização do git, podes utilizar o GUI do GitHub [https://desktop.github.com/](https://desktop.github.com/)
![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/GitHub-Desktop.png)



## Após a instalação
Sempre que fizeres um commit, ficará registado o teu nome e o teu e-mail, se ainda não configuraste o git com essas 
informações, podes faze-lo executando os seguintes comandos no terminal (dentro do repositório)

`git config --global user.name "Meu Nome"`

`git config --global user.email "meu@email.com"`


## Criar primeiro repositório no GitHub
É possível começares por criar um repositório no teu computador, e depois fazeres um clone desse repositório para o 
GitHub, no entanto, para simplificar, vamos criar o repositório directamente no GitHub, e depois fazer o clone para o 
teu computador e dos teus colegas de equipa.

1º Após criares uma conta no GitHub, clica em `New Repository` para criares um novo repositório.

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/GitHub-New_Repository.png)

2º Coloca o nome que vais dar ao teu repositório.

> **Nota:**
> 
> Tem em atenção que se mais tarde mudares o nome do repositório, 
todas as pessoas que já fizerem um clone de repositório terão que editar o ficheiro de configurações, ou voltar a fazer 
um clone do repositório, pois o URL do repositório será diferente.

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/GitHub-New_Repository-Insert_Name.png)

3º Podes agora adicionar os teus colegas de equipa ao repositório, adicionado colaboradores.

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/GitHub-Repository-Add_Collaborator.png)
 

## Copiar um repositório do GitHub para o teu computador

Sempre que pretenderes clonar para o teu computador um repositório do GitHub, deves abrir esse mesmo repositório, e 
clicar no botão `Clone or download`, de seguida deves copiar o URL `https://github...` 

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/GitHub-Clone_Repository.png)


Agora que copiaste o URL do projecto, vais fazer um `git clone`, para isso tens várias opções:

* Opção 1: Executar na linha de comandos

`git clone https://github.com/HardwareCity/hardwarecity_sunset_hackathon_2017.git`

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/git_clone_url.png)

* Opção 2: Utilizar um GUI

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/GitHub-Desktop.png)

* Opção 3: Utilizar um plugin no explorador de ficheiros

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/TODO)

Agora que já tens o repositório no teu computador, podes executar todos os comandos git que vamos descrever de seguida.

## Comandos git mais usados

### git clone
`git clone https://github.com/HardwareCity/hardwarecity_sunset_hackathon_2017.git`

Utilizas o git clone quando queres copiar um repositório que está no GitHub para o teu computador 

### git add
`git add file1.txt file2.txt filen.txt`

`git add -A`

Utilizas o git add quando pretende que um determinado ficheiro novo passe a ser controlado pelo git, ou seja, sempre que
criares um ficheiro novo no teu projecto, ele não ficará automaticamente sob o efeito do controlo de versões do git, 
terás que fazer um git add do ficheiro, ou um `git add -A` para que sejam adicionados todos os ficheiros dentro dessa 
pasta e subpastas. 

### git commit
`git commit file1.txt file2.txt filen.txt`

`git commit -a`

`git commit -a -m "Isto é um comentário associado ao commit"`

Este deve ser o comando que mais vais utilizar, serve para fixares um estado nos ficheiros, ou seja, é feito uma cópia 
dos ficheiros, onde poderás mais tarde reverter o histórico para este ponto.

Cada commit é acompanhado por um comentário de forma a dares a entender à tua equipa das alterações que fizeste.

Podes fazer commit de ficheiros isolados, ou de todos os ficheiros já controlados pelo git, fazendo `git commit -a`.
(Serão ignoratos todos os ficheiros que ainda não tenham sido adicionados com `git add`, e todos os que estiverem dentro
 do ficheiro `.gitignore`)

> **Nota:**
>
> Todos os commits são feitos localmente, no teu computador, as alterações só serão enviadas para o servidor após um 
> `git push`. Aconselhamos-te a que sempre que fizeres um `commit`, faças também um `push`, de forma a que no GitHub
> tens o código sempre actualizado, e facilita a sincronização com os teus colegas de equipa, evitando conflitos. 

### git push
`git push origin master`

Com o `git push`, vais enviar todos os teus commits para o repositório no GitHub, a partir desse momento, os teus 
colegas podem fazer um `git pull` para receberem o teu código.

Como o git funciona com branchs, no comando `git push` tens que dizer qual o branch a ser utilizado. 
Por omissão estás no branch "master". 

> **Nota:**
> 
> Aconselhamos-te a que sempre que fizeres um `git push`, que faças também um `git pull`, de forma a que após enviares
> as tuas alterações para o servidor, também recebas as alterações dos teus colegas de equipa. 


### git pull
`git pull origin master`

Com o `git pull`, vais receber dos teus colegas, todos os commits que eles já tenham deixado no GitHub.

Como o git funciona com branchs, no comando `git pull` tens que dizer qual o branch a ser utilizado. 
Por omissão estás no branch "master". 


### git branch
`git branch`
O comando `git branch` mostra-te todos os branchs do projecto que já tens no teu computador. 

### git checkout
`git checkout develop`
O comando `git checkout` altera-te o branch seleccionado para um outro, por exemplo é normal os projectos terem pelo 
menos 2 branchs, um é o branch `develop` onde se vão juntando todos os commits da equipa, e só após todo o código ser 
testado é que esse código é que é enviado para o branch `master`, assim garante-se que o branch master tem sempre 
versões de código mais "estáveis". 

### git status
`git status`
Com o comando `git status` o git mostra-te o estado actual do repositório (que ficheiros novos ainda não foram 
adicionados, que ficheiros estão alterados em relação ao ultimo commit, etc.)


### git fork
Podes criar um novo repositório baseado num repositório já existente, a isto chama-se um fork.
Podes a qualquer altura actualizar o teu projecto com as actualizações que foram feitas no projecto principal, ou 
submeter um pedido para que os autores do projecto inicial incluam as tuas alterações feitos ao projecto inicial.

No GitHub, podes fazer um fork clicando directamente no botão `fork`

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/10_survival_kit/20_tutorials/img/GitHub-fork.png)
