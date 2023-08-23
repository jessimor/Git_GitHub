# Git e GitHub 

## Notas das aulas e dos primeiros contatos com a área de Tecnologia

## 🖥️Git
**Sistema de Controle de versão Distribuído**
<sub> onde cada alteração do código é gerado uma nova versão </sub>

* Gratuito e Open Source (código aberto)
* Ramificações e fusões eficientes
* Leve e rápido

## 💻GitHub
Plataforma de hospedagem de código para controle de versão com Git e Colaboração

<sub>*Git atua na parte de banco de versões onde faz o gerenciamento das versões do cógido.*
*Github se configura como servidor que estará hospedando o código/repositório remoto.*</sub>
## git config

Permite visualizar e definir variáveis de configuração do nosso Git. Essas variáveis ficam armazenadas principalmente em 3 lugares: 

- Git Global (configurações do usuário)
- System: configurações do sistema como um todo e que abriga todos os usuários
- Local: referente a configuração de um repositório específico que você se encontra (onde guardamos o nosso projeto)

`git config --global user,name "Jessica"`

`git config --global user.email jessica@gmail.com`

Para verificar as minhas configurações: `git config --global --list`

Para abrir página do Manual do Git: `git help config`



## 📑Clonando um Repositório
Existem 2 formas de obter um repositório na sua maquina:
* Transformando um repositório local que não está sob controle de versão, num repositório Git; comando `git init`
*  Clonando um repositório Git existente; comando `git clone`

### 📝Criando um projeto
* Criar uma pasta que a gente deseja transformar em um repositório Git
* 
  `mkdir NomeDaPasta` cria a pasta
* `cd NomeDaPasta` entra na pasta
* `git init` transforma a pasta em um repositório
<sub>.git (quando contem esse ponto inicial é porque a pasta está oculta)</sub>
* `ls` lista todo o conteúdo de dentro

*Esse reposotório .git tem todos os arquivos necessários para gerenciar o nosso controle de versão*

`git add README.md` coloca o arquivo para ser "commitado"


***Diretório de trabalho ➡️`git add`➡️Área stagging (para commitar)➡️`git commit`➡️ Repositório***

`git status` mostra se tem alterações a serem commitadas

`git commit -m"Commit 1"` insere as alterações do repositório dentro de um commit

`git log` exibe o histórico de commit e sua identidade

Para alterar o nome do commit: `git commit -amend -m"CommitNovo"`

`git reflog` traz histórico detalhado das alterações feitas

*<sub> Caso tenha algum(s) arquivo(s) que não deseja salvar você pode adicionar `gitignore` 
Ex.: `echo resumos /> .gitignore`</sub>.

**<sub> Git não reconhece diretórios vazios (pastas que criei e está vazia). Ex.: `mkdir aulas`
Mas é comum que tenha arquivos dessa forma dentro de diretórios: `touch aulas/ .gitkeep` (feito para que o git reconheça o diretório)</sub>

### ✏️Desfazendo alterações no Repositório LOCAL

Se fiz alterações no meu diretório (README) e quero voltar com as informações anteriores para retornar ao último estado:

`git restore README.md`

*<sup>CUIDADO pois descarta todas as alterações realizadas localmente</sup>

## 💻Repositório no GitHub
* Após entrar na conta ir em `New Repository`
* Adicionar nome ao repositório, descrição e criar
* Copiar o link do repositório
* `git remote add origin <COLAR link do repositório Github>`

<sub>`origin` é utilizado para nomear o nosso repositório </sub>

`git push -u origin main` para subir o commit do nosso PC para a plataforma

## 📑Adição e alteração de Arquivos

* Em nosso arquivo adicionamos uma alteração

* Criamos um novo arquivo (Ex.:Resumo.md) e escrevemos Conteúdo das Aulas
* `git add .` para subir essa alteração e adicionar todos os arquivos
* `git commit -m"Mudança1"`

`git push origin main` para alterar o nosso repositório do GitHub (sem o -u).

<sub>Nos commites do GitHub podemos ver as alterações que foram realizadas (os conteúdos que foram adicionados e editados).

