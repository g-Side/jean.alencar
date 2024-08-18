# Exercicio 02


@g-Side ➜ /workspaces/codespaces-blank $ git config --global user.name "Jean Alencar"
@g-Side ➜ /workspaces/codespaces-blank $ git config --global user.email "OCULTADO PARA NÃO VAZAR DADOS"
@g-Side ➜ /workspaces/codespaces-blank $ mkdir aula01
@g-Side ➜ /workspaces/codespaces-blank $ cd aula01/
@g-Side ➜ /workspaces/codespaces-blank/aula01 $ git init
Initialized empty Git repository in /workspaces/codespaces-blank/aula01/.git/
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ ls
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo 01 > arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git add arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt

@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git commit -m "git add example - arquivo.txt"
[main (root-commit) fd7f8cb] git add example - arquivo.txt
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo 02 > arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git add arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git diff arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo 03 > arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git res
reset     restore   
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git restore --staged arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git sta
stage    stash    status   
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git sta
stage    stash    status   
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git sta
stage    stash    status   
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git status 
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git commit -m "commit apos restore"
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git restore --staged arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git add arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git res
reset     restore   
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git restore --staged arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+03
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo 02 > arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git add .
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo 03 > arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git res
reset     restore   
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git restore --staged arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+03
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git commit -m "comit apos o restore"
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo 02 > arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git add arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ eecho 03 > arquivo.txt 
bash: eecho: command not found
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo 03 > arquivo.txt 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git restore --staged arquivo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git restore --staged .
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git commit -m "comit apos o restore" .
[main 45c3074] comit apos o restore
 1 file changed, 1 insertion(+), 1 deletion(-)
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git log
commit 45c3074af5ff4a69ed6b322cb3f91ebff2028859 (HEAD -> main)
Author: Jean Alencar <jean.alencar@aluno.faculdadeimpacta.com.br>
Date:   Sun Aug 18 13:57:57 2024 +0000

    comit apos o restore

commit fd7f8cb63f935a0dcf02491cfccf879fb690e7a7
Author: Jean Alencar <jean.alencar@aluno.faculdadeimpacta.com.br>
Date:   Sun Aug 18 13:42:27 2024 +0000

@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git diff 
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo "*.txt" > .gitignore
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ echo "novo conteudo" > novo.txt
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
@g-Side ➜ /workspaces/codespaces-blank/aula01 (main) $ 
