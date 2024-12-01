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
