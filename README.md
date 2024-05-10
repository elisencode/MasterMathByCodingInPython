# Master Math by Coding in Python
Python code accompanying the course "Master Math by Coding in Python"

37+ hours of instruction (>60 hours in total, including exercises) on how to use Python as a tool for learning concepts and visualizations in mathematics.

See https://www.udemy.com/course/math-with-python/?couponCode=202311 for more details, preview videos, and to enroll in the full course.

---

$ jupyter notebook --version
7.0.8

$ conda --version
conda 23.5.0

---



---

```
$ git branch -a
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/elisencode_pymath
  remotes/origin/main
  
$ git checkout elisencode_pymath
Branch 'elisencode_pymath' set up to track remote branch 'elisencode_pymath' from 'origin'.
Switched to a new branch 'elisencode_pymath'

$ git branch
* elisencode_pymath
  main
  
```

---

1. Github: After first pull request, 

2. Github: then confirm merge the branch elisencode_pymath

3. Github: **Deleted remote branch elisencode_pymath**

4. Local Computer : Terminal : git switch main

5. Local Computer : Terminal : Delete local branch elisencode_pymath

6. Local Computer : Terminal : `git pull --rebase <remote repo>`, because:

   

   [right thing to do is always --rebase](https://stackoverflow.com/questions/2472254/when-should-i-use-git-pull-rebase)

   "In my opinion, in the normal case of having your local branch simply reflecting the upstream branch and doing continuous development on it, the right thing to do is always --rebase, because that is what you are semantically actually doing. You and others are hacking away at the intended linear history of a branch. The fact that someone else happened to push slightly prior to your attempted push is irrelevant, and it seems counter-productive for each such accident of timing to result in merges in the history."

   

```
$ git branch -a
* elisencode_pymath
  main
  remotes/origin/HEAD -> origin/main
  remotes/origin/elisencode_pymath
  remotes/origin/main

$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

$ git branch
  elisencode_pymath
* main

$ git branch -d elisencode_pymath 
warning: deleting branch 'elisencode_pymath' that has been merged to
         'refs/remotes/origin/elisencode_pymath', but not yet merged to HEAD.
Deleted branch elisencode_pymath (was 6f4fcdf).

$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	pymath/

nothing added to commit but untracked files present (use "git add" to track)

$ git branch -r
  origin/HEAD -> origin/main
  origin/elisencode_pymath
  origin/main

$ git remote -v
origin	git@github.com:elisencode/MasterMathByCodingInPython.git (fetch)
origin	git@github.com:elisencode/MasterMathByCodingInPython.git (push)

$ git pull --rebase git@github.com:elisencode/MasterMathByCodingInPython.git

$ git log --oneline
8df271f (HEAD -> main) Merge pull request #1 from elisencode/elisencode_pymath
6f4fcdf (origin/elisencode_pymath) Add pymath/sec2_16_if_satements_and_logical_operators.ipynb file
992f54e Add pymath folder, modified README.md
347db4f Add new branch elisencode_pymath, gitignore file, README.md
bedb7cb (origin/main, origin/HEAD) Add files via upload
a955bc8 Add files via upload
ee84998 Add files via upload
c127f49 Add files via upload
b2a92ac Add files via upload
cb1a653 Add files via upload
0cfcd75 Update README.md
61f1ec6 Update README.md
2820171 Add files via upload
485d8ac Add files via upload
373d224 Add files via upload
0546312 Update README.md
453e268 Delete mathWithPython_arithmetic_basicArith.ipynb
2860aee Add files via upload
b720982 Create README.md

$ git status
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

$ man git branch

$ git branch -r
  origin/HEAD -> origin/main
  origin/elisencode_pymath
  origin/main

$ git branch -a
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/elisencode_pymath
  remotes/origin/main


```

---

```
ai@linux:/Devices/linux_part2/code/jupyter_notebook_code/MasterMathByCodingInPython$ conda activate
(base) ai@linux:/mnt/01778196-842c-4a91-8cfe-7fcbfc2f3551/code/jupyter_notebook_code/MasterMathByCodingInPython$ conda env list
# conda environments:
#
base                  *  /home/ai/anaconda3
AI                       /home/ai/anaconda3/envs/AI
converter_env            /home/ai/anaconda3/envs/converter_env
example                  /home/ai/anaconda3/envs/example
py3                      /home/aDevicesnaconda3/envs/py3

(base) ai@linux:/Devices/linux_part2/code/jupyter_notebook_code/MasterMathByCodingInPython$ conda activate AI
(AI) ai@linux:/Devices/linux_part2/code/jupyter_notebook_code/MasterMathByCodingIde/MasterMathByCodingInPython$ jupyter notebook

Or: 
$ conda activate AI

Finally after Ctrl+C twice:
$ conda deactivate
```

---

Shutdown the open notebook properly:

1. File --> Close and Halt
2. Logout and close your browser window
3. Ctrl + C twice to skip confirmation: in order to terminating the jupyter notebook from the terminal.

