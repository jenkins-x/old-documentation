## jx step tag

Creates a git tag and pushes to remote repo

### Synopsis


This pipeline step command creates a git tag using a version number prefixed with 'v' and pushes it to a remote origin repo. 

This commands effectively runs: 

git commit -a -m "release $(VERSION)" --allow-empty git tag -fa v$(VERSION) -m "Release version $(VERSION)" git push origin v$(VERSION)

```
jx step tag
```

### Examples

```
  jx step tag --version 1.0.0
```

### Options

```
  -v, --version string   version number for the tag [required]
```

### SEE ALSO
* [jx step](jx_step.md)	 - pipeline steps

###### Auto generated by spf13/cobra on 12-Feb-2018