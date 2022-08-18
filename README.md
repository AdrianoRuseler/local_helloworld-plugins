# local_helloworld-plugins
Workflows test for submodules plugins

- https://docs.github.com/en/actions

## Plugins

- https://github.com/AdrianoRuseler/local_helloworld
```bash
git submodule add -b main https://github.com/AdrianoRuseler/local_helloworld.git local/helloworld
```



## Remove

```bash
SUBMPATH="moodle/path/to/submodule"
git submodule deinit $SUBMPATH
git rm $SUBMPATH
git commit -m "Removed submodule $SUBMPATH"
rm -rf .git/modules/$SUBMPATH
git push
```

## Add

```bash
git submodule add -b branch https://urltoplugin.git path/to/submodule
git add .
git commit -m "Some update info here..."
git push
```
