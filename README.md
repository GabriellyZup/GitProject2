# GitProject2
Exercícios práticos de git/github por powershell - catalisat6 M1 Ex3



Criar pasta acessória para clonar o projeto:

O Windows PowerShell
Copyright (C) Microsoft Corporation. Todos os direitos reservados.

Instale o PowerShell mais recente para obter novos recursos e aprimoramentos! https://aka.ms/PSWindows

PS C:\Users\gabrielly.boareto> mkdir Catalisa


    Diretório: C:\Users\gabrielly.boareto


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        01/12/2024     14:50                Catalisa


Clonar o repositório

PS C:\Users\gabrielly.boareto\Catalisa> git clone git@github.com:GabriellyZup/GitProject2.git
Cloning into 'GitProject2'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 6 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (6/6), done.
Resolving deltas: 100% (1/1), done.
PS C:\Users\gabrielly.boareto\Catalisa>


Criar e mover nova banch

1. navegar para dentro da branch main
PS C:\Users\gabrielly.boareto\Catalisa> cd GitProject2
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git branch
* main

2. criar e mover a nova branch
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git checkout -b adicionar-info-catalisa
Switched to a new branch 'adicionar-info-catalisa'
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2>


Abrir o readme pelo terminal
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> notepad README.md
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git status
On branch adicionar-info-catalisa
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Adicionar informações ao README pelo terminal
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git add README.md
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2> git commit -m "add info sobre Catalisa no README"
[adicionar-info-catalisa a8cbc85] add info sobre Catalisa no README
 1 file changed, 14 insertions(+)
PS C:\Users\gabrielly.boareto\Catalisa\GitProject2>

-Push pelo terminal
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



