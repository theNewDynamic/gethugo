# gethugo

Bash Script to load Hugo locally in a project



## To Use

To Use
 - Add the `get-hugo.sh` file to the root of your repo
 - add the following to your package.json file:
 ```
 "hugo": {
    "version": "0.63.1",
    "extended": "true"
  }
  ```

Extended is optional. The script will use the extended version of Hugo unless `"extended": "false"` or `"extended": false` is set.

- Run `bash get-hugo.sh` or add `"gethugo": "bash get-hugo.sh",` to your package.json and run it from there.

- Without package.json use positional parameter as the version:
```
bash get-hugo.sh 0.63.1
```

## To Do


- [ ] Clean up (can maybe be less verbose)
- [ ] Fail better if Hugo is not in package.json at all.
- [ ] Maybe use a different method than requiring node to get package.json (what we have is simple though)
- [ ] If Hugo version (package.json.hugo.version) not present in package.json get the latest Hugo version.
- [ ] Make a CLI
