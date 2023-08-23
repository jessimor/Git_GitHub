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



## Clonando um Repositório
Existem 2 formas de obter um repositório na sua maquina:
* Transformando um repositório local que não está sob controle de versão, num repositório Git; comando `git init`
*  Clonando um repositório Git existente; comando `git clone`

### Criando um projeto
* Criar uma pasta que a gente deseja transformar em um repositório Git
* 
  `mkdir NomeDaPasta` cria a pasta
* `cd NomeDaPasta` entra na pasta
* `git init` transforma a pasta em um repositório
<sub>.git (quando contem esse ponto inicial é porque a pasta está oculta)</sub>
* `ls` lista todo o conteúdo de dentro

*Esse reposotório .git tem todos os arquivos necessários para gerenciar o nosso controle de versão*


