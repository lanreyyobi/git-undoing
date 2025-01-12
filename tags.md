**a) Semantic versioning**

https://semver.org/
```yaml
v1.0.0
Major . Minor .   Patch
fix:   Feat:   BREAKING CHANGE:
```
**b) Creating a tag**

**i) Lightweight tags**
```yaml
git tag v1.0.0
```

**ii) Annotated Tags** - specify -a to create and you can specify -m to specify a tagging message.
 
-  If you don't specify a message for an annotated tag, Git launches your editor so you can type.
```yaml
gti tag -a v1.0.1 -m "my version 1.0.1"
```
**c) Listing tags** - lists tags in alphabetical order
```yaml
git tag
```
**d) Search for tags**
```yaml
git tag -l "*beta*"
```

**e) Tagging previous commits**
```yaml
git tag -a v1.2 <commit-id>

git show v1.2
```

**f) Sharing tags in remote**
```yaml
git push origin <tag-name>

#To push all tags
git push origin --tags
```
**g) Deleting tags**
```yaml
git tag -d <tag-name>

#To delete tag from remote
git push origin --delete <tag-name>
```
