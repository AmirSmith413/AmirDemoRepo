# AmirDemoRepo

PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo> cd AmirDemoRepo
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git checkout -b future/login
Switched to a new branch 'future/login'
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git branch
* future/login
  main
  mynewbrachAmir
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git log
commit 881feded365001050cfb9ebeab2b7fb20510dabe (HEAD -> future/login)
Author: AmirSmith413 <amirsmith166@gmail.com>
Date:   Thu Oct 27 19:42:43 2022 -0700

    added "hello there"

commit e74504c330ac7413b67dcfd2f43cbed08f829501 (origin/main, origin/HEAD, mynewbrachAmir, main)
Author: AmirSmith413 <amirsmith166@gmail.com>
Date:   Thu Oct 27 19:27:03 2022 -0700

    edited file1.js
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git log --oneline
881fede (HEAD -> future/login) added "hello there"
e74504c (origin/main, origin/HEAD, mynewbrachAmir, main) edited file1.js
7e94a95 added files
0870692 added file1.js
e3fce01 Initial commit
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git log --oneline --all
881fede (HEAD -> future/login) added "hello there"
e74504c (origin/main, origin/HEAD, mynewbrachAmir, main) edited file1.js
7e94a95 added files
0870692 added file1.js
e3fce01 Initial commit
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git log main..future/login
commit 881feded365001050cfb9ebeab2b7fb20510dabe (future/login)
Author: AmirSmith413 <amirsmith166@gmail.com>
Date:   Thu Oct 27 19:42:43 2022 -0700

    added "hello there"
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git merge future/login
Updating e74504c..881fede
Fast-forward
 file1.js | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git branch merged
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git branch --merged
  future/login
* main
  merged
  mynewbrachAmir
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git branch --no-merged
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git checkout future/login
Switched to branch 'future/login'
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git branch -d future/login
error: Cannot delete branch 'future/login' checked out at 'C:/Users/61006/OneDrive/Documents/CodeStack/RepoDemo/AmirDemoRepo'
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\61006\OneDrive\Documents\CodeStack\RepoDemo\AmirDemoRepo> git branch -d future/login
Deleted branch future/login (was 881fede).