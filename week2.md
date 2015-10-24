# Week2

## 前回提要
- `git status`
- `git add`
- `git commit`
- `git push`
- `git log`

## 分散式版本控制 -- Branch workflow (Feature Branch workflow)
- 多個功能，多個分支
- 永遠不要去打擾主要分支 (master)

### How it work

![first](http://i.imgur.com/9xXoF2S.png)
![second](http://i.imgur.com/E4w0B2E.png)
![thrid](http://i.imgur.com/zm1ApR9.png)

![branch](https://docs.google.com/drawings/d/1GIYdJVVUDJah87L_eXc76YytV395qY8Y94RaSb5SNa0/pub?w=670&h=619)

### Steps
1. 於一個 git 專案下切換一個新的 branch
  ```bash
  $ git checkout -b <new_branch>
  ```
2. 在新建的 branch 底下進行開發工作，新增、修改檔案後記得做 `commit` 的動作
  ```bash
  $ git add .
  $ git commit -m "Message for this commit"
  ```


## What is `pull`?
- `pull` = `fetch` + `merge`
- `merge` vs. `rebase`
- `git diff master --stat`
- `git diff master <path>`
- `rebase` live show
  - DO NOT COMMIT!
- Workflow
- `merge`
- `$ git branch --delete <branch>`
- `$ git push --delete <branch>`

### References
- [GIT: FETCH AND MERGE, DON’T PULL](http://longair.net/blog/2009/04/16/git-fetch-and-merge/)

## Advanced `rebase`
```bash
git rebase --onto <newbase>
```

## Rollback
- `revert`
- `reset`
