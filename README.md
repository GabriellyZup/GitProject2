# GitProject2
## Exercícios práticos de git/github por powershell - catalisat6 M1 Ex3



**Criar pasta acessória para clonar o projeto:**
    PS C:\Users\gabrielly.boareto> mkdir Catalisa
    Diretório: C:\Users\gabrielly.boareto

**Abrir o README pelo PowerShell**
    PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> notepad README.md
    Mode                 LastWriteTime         Length Name
    ----                 -------------         ------ ----
    d-----        01/12/2024     14:50                Catalisa

**Clonar o repositório**
PS C:\Users\gabrielly.boareto\Catalisa> git clone git@github.com:GabriellyZup/GitProject2.git
Cloning into 'GitProject2'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 6 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (6/6), done.
Resolving deltas: 100% (1/1), done.
PS C:\Users\gabrielly.boareto\Catalisa>

**Criar e mover nova banch**
    1. navegar para dentro da branch main
    PS C:\Users\gabrielly.boareto\Catalisa> cd GitProject2
    PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git branch
    * main

    2. criar e mover a nova branch
    PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git checkout -b adicionar-info-catalisa
    Switched to a new branch 'adicionar-info-catalisa'
    PS C:\Users\gabrielly.boareto\Catalisa\GitProject2>


**Abrir o readme pelo terminal**
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> notepad README.md
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git status
On branch adicionar-info-catalisa
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
no changes added to commit (use "git add" and/or "git commit -a")

**Adicionar informações ao README pelo terminal**
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git add README.md
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git commit -m "add info sobre Catalisa no README"
[adicionar-info-catalisa a8cbc85] add info sobre Catalisa no README
 1 file changed, 14 insertions(+)
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2>

**Push pelo terminal**
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git push origin adicionar-info-catalisa
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (9/9), 2.51 KiB | 514.00 KiB/s, done.
Total 9 (delta 2), reused 5 (delta 1), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
remote:
remote: Create a pull request for 'adicionar-info-catalisa' on GitHub by visiting:
remote:      https://github.com/GabriellyZup/GitProject2/pull/new/adicionar-info-catalisa
remote:
To github.com:GabriellyZup/GitProject2.git
 * [new branch]      adicionar-info-catalisa -> adicionar-info-catalisa

**Adicionar informações pelo terminal**
adicionar-info-catalisa
PS C:\Users\gabrielly.boareto> cd Catalisa

" O Programa Catalisa é uma iniciativa inclusiva voltada para o desenvolvimento profissional de pessoas com diversos níveis de senioridade"
" Minha participação no programa tem foco na aprendizagem teórica e em projetos práticos."

**checar no terminal se tudo está atualizado**
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git pull origin main
remote: Enumerating objects: 20, done.
remote: Counting objects: 100% (20/20), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 16 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (16/16), 6.67 KiB | 31.00 KiB/s, done.
From github.com:GabriellyZup/GitProject2
 * branch            main       -> FETCH_HEAD
   16319e0..00c88de  main       -> origin/main
Updating 16319e0..00c88de




**Fork**
PS C:\Users\gabrielly.boareto\Catalisa> git clone git@github.com:GabriellyZup/aula-github-fork.git
Cloning into 'aula-github-fork'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.
PS C:\Users\gabrielly.boareto\Catalisa> cd aula-github-fork
PS C:\Users\gabrielly.boareto\Catalisa\aula-github-fork> git branch
* main
PS C:\Users\gabrielly.boareto\Catalisa\aula-github-fork> git checkout -b readmefork
Switched to a new branch 'readmefork'
PS C:\Users\gabrielly.boareto\Catalisa\aula-github-fork> git branch
  main
* readmefork
PS C:\Users\gabrielly.boareto\Catalisa\aula-github-fork> git push origin readmefork
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'readmefork' on GitHub by visiting:
remote:      https://github.com/GabriellyZup/aula-github-fork/pull/new/readmefork
remote:
To github.com:GabriellyZup/aula-github-fork.git
 * [new branch]      readmefork -> readmefork
PS C:\Users\gabrielly.boareto\Catalisa\aula-github-fork> git pull origin main
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (4/4), 1.80 KiB | 39.00 KiB/s, done.
From github.com:GabriellyZup/aula-github-fork
 * branch            main       -> FETCH_HEAD
   f11db66..dab9455  main       -> origin/main
Updating f11db66..dab9455
Fast-forward
 README.md | Bin 62 -> 58 bytes
 1 file changed, 0 insertions(+), 0 deletions(-)
PS C:\Users\gabrielly.boareto\Catalisa\aula-github-fork>
Fast-forward
 README.md | 78 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 78 insertions(+)
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2>



