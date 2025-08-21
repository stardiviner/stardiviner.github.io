# org-publish workflow

1. git switch to the branch "main" with `git switch main`.
2. modify website blog .org files.
3. org-publish the changes with Emacs command `M-x org-publish RET WEBSITE RET`.
4. git push the branch "main" changes to the remote repository with `git add .`, `git commit -m "your commit message"`, and `git push`.
5. move org-publish exported directory "`org-publish`" to `/tmp`.
6. git switch to the branch "gh-pages" with `git switch gh-pages`.
7. replace and override current directory in the branch "`gh-pages`" with the content in `/tmp/org-publish`.
8. git push the branch "gh-pages" to the remote repository with `git add .`, `git commit -m "your commit message"`, and `git push origin gh-pages`.
9. git switch back to the branch "main" with `git switch main`.
10. check the website at [my blog](https://stardiviner.github.io/).