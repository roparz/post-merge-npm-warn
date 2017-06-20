# post-merge-npm-warn

Add the following line to your `package.json`.

```
{
  "scripts": {
    "postinstall": "ln -sf ../../node_modules/post-merge-npm-warn/post-merge .git/hooks/post-merge && chmod +x .git/hooks/post-merge"
  }
}
```

It can also be used with `post-rewrite` if you are using git with rebase.


```
{
  "scripts": {
    "postinstall": "ln -sf ../../node_modules/post-merge-npm-warn/post-merge .git/hooks/post-rewrite && chmod +x .git/hooks/post-rewrite"
  }
}
```
