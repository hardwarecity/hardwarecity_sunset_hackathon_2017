# Introdução ao Git e GitHub

Este documento apresenta uma breve introdução ao [**Git**](https://git-scm.com/) e ao [**GitHub**](https://github.com/),
de forma a poderes dominar o essencial para criares um projecto a partir do zero.

Podes melhorar este documento, editando-o, só tens que dominar o git :) 

## Estrutura do manual:
- O que é o Git?
- O que é o GitHub?
- Instalar Git no teu computador
- Criar novo repositório no GitHub
- Copiar um repositório do GitHub para o nosso computador

---

## O que é o Git?
O [git](https://git-scm.com/) é um sistema de controlo de versões distribuido, e um sistema de gestão de código-fonte, 
ou seja, quando escreveres código, podes ir assinalando momentos importantes, em que é salvo uma cópia do trabalho, 
podes mais tarde reverter para algum dos pontos anteriores. Também podes sincronizar esse ficheiro com os teus colegas 
de equipa, em que o git automáticamente compara as diferenças e junta as
alterações que as pessoas fizeram. Existem outros protocolos semelhantes ao Git, como por exemplo o Subversion, mas o 
Git é dos mais completos, e dos mais usados.

Independentemente do teu sistema operativo, vais precisar de instalar o protocolo git, que normalmente é executado na 
linha de comandos, mas para facilitar a vida, podes instalar um GUI para git, de forma a não teres que memorizar os 
comandos todos, e usufruires de todas as vantagens de uma interface gráfica. Podes também instalar algum plugin para 
integrar o git no teu explorador de ficheiros, de forma a conseguires executar algumas ações sem teres que abrir algum 
programa. Podes instalar estes 3 software independentemente, ou podes instalar logo algum que traga tudo incluido.

## O que é o GitHub?
O [GitHub](https://github.com/) é um serviço de "alojamento" de repositórios Git. Grandes projectos opensource costumam
ter o código disponivel no GitHub, como por exemplo a [BeeVeryCreative](https://github.com/beeverycreative). 
Existem outros serviços semelhantes ao GitHub, como por exemplo o [Bitbucket](https://bitbucket.org/), que te permite 
criar de forma gratuita repositórios privados. Podes também criar o teu próprio servidor de Git, mas visto que estás a 
ler o manual de introdução ao Git, não me parece que devas partir já por esse caminho. :)

## Instalação

### Windows
No windows, podes instalar o [Git for Windows (https://git-for-windows.github.io/)](https://git-for-windows.github.io/),
que instala aumaticamente o protocolo git para executares na linha de comandos, 
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

Caso ainda não tenhas Podes instalar o git pelo terminal. Executa o comando correspondente ao teu sistema operativo:

#### Sistemas baseados em Debian, como Ubuntu, Raspbian, Mint, etc.
`sudo apt-get install git-core`
#### Sistemas baseados em Red Hat, como CentOS, etc.
`sudo yum install git`

### Mac OSx
TO DO

https://sourceforge.net/projects/git-osx-installer/files/

https://git-scm.com/download/mac

## Após a instalação
TO DO

`git config --global user.name "Meu Nome"`

`git config --global user.email "meu@email.com"`

## Criar primeiro repositório no GitHub
É possivel começares por criar um repositorio no teu computador, e depois fazeres um clone desse repositório para o 
GitHub, no entanto, para simplificar, vamos criar o repositório directamente no GitHub, e depois fazer o clone para o 
teu computador e dos teus colegas de equipa.

1º Após criares uma conta no GitHub, clica em `New Repository` para criares um novo repositório.

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/survival_kit/img/GitHub-New_Repository.png)

2º Coloca o nome que vais dar ao teu repositório.

> **Nota:**
> 
> Tem em atenção que se mais tarde mudares o nome do repositório, 
todas as pessoas que já fizerem um clone de repositório terão que editar o ficheiro de configurações, ou voltar a fazer 
um clone do repositório, pois o URL do repositório será diferente.

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/survival_kit/img/GitHub-New_Repository-Insert_Name.png)

3º Podes agora adicionar os teus colegas de equipa ao repositório, adicionado colaboradores.

![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/survival_kit/img/GitHub-Repository-Add_Collaborator.png)
 

## Baixar um repositório já existente no GitHub
TO DO
![img](https://raw.githubusercontent.com/HardwareCity/hardwarecity_sunset_hackathon_2017/master/survival_kit/img/GitHub-Clone_Repository.png)

## Comandos mais usados

### git commit
TO DO

### git push
TO DO

### git pull
TO DO

### git branch
TO DO

### TO DO
