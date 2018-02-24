## jx step changelog

Creates a changelog for a git tag

### Synopsis


Generates a Changelog for the last tag

```
jx step changelog
```

### Examples

```
  jx step changelog
```

### Options

```
      --crd-yaml-file string       the name of the file to generate the Release CustomResourceDefinition YAML (default "release-crd.yaml")
  -o, --overwrite                  overwrites the Release CRD YAML file if it exists
  -p, --previous-rev string        the previous tag revision
      --release-yaml-file string   the name of the file to generate the Release YAML (default "release.yaml")
  -r, --rev string                 the current tag revision
  -t, --templates-dir string       the directory containing the helm chart templates to generate the resources
```

### SEE ALSO
* [jx step](jx_step.md)	 - pipeline steps

###### Auto generated by spf13/cobra on 24-Feb-2018