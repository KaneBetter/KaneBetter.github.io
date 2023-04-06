# How to create a new post?

`hugo new posts/<name>.md`

And it will create `<name>.md` in `./content/post/`

Then use `Typora` to write. And all pics will be uploaded to GitHub so use pics carefully.

After you finish your changes, you should run this command.

```bash
git add *
git commit -m "Add blog posts <name>"
git push
```

 You can see the deployment [here](https://github.com/KaneBetter/KaneBetter.github.io/deployments).

After deployment, refresh the [page](https://kanebetter.github.io/).