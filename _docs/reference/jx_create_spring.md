---
date: 2018-03-04T13:23:29Z
title: "jx create spring"
slug: jx_create_spring
url: /commands/jx_create_spring/
---
## jx create spring

Create a new spring boot application and import the generated code into git and Jenkins for CI / CD

### Synopsis

Creates a new Spring Boot application on the file system. 

You then get the option to import the generated source code into a git repository and Jenkins for CI / CD

```
jx create spring [flags]
```

### Examples

```
  # Create a Spring Boot application where you use the terminal to pick the values
  jx create spring
  
  # Creates a Spring Boot application passing in the required dependencies
  jx create spring -d web -d actuator
```

### Options

```
  -x, --advanced                       Advanced mode can show more detailed forms for some resource kinds like springboot
  -a, --artifact string                Artifact ID to generate
  -b, --batch-mode                     In batch mode the command never prompts for user input
  -t, --boot-version string            Spring Boot version
      --branches string                The branch pattern for branches to trigger CI / CD pipelines on. Defaults to 'master|PR-.*|feature.*'
      --credentials string             The Jenkins credentials name used by the job
  -d, --dep stringArray                Spring Boot dependencies
      --dry-run                        Performs local changes to the repo but skips the import into Jenkins X
      --git-api-token string           The git API token to use for creating new git repositories
      --git-provider-url string        The git server URL to create new git repositories inside (default "github.com")
      --git-username string            The git username to use for creating new git repositories
  -g, --group string                   Group ID to generate
      --headless                       Enable headless operation if using browser automation
  -h, --help                           help for spring
      --import-commit-message string   The git commit message for the import
  -j, --java-version string            Java version
      --jenkinsfile string             The name of the Jenkinsfile to use. If not specified then 'Jenkinsfile' will be used
  -k, --kind stringArray               Default dependency kinds to choose from (default [Core,Web,Template Engines,SQL,I/O,Ops])
  -l, --language string                Language to generate
      --name string                    Specify the git repository name to import the project into (if it is not already in one)
      --no-draft                       Disable Draft from trying to default a Dockerfile and Helm Chart
      --no-import                      Disable import after the creation
      --no-jenkinsfile                 Disable defaulting a Jenkinsfile if its missing
      --org string                     Specify the git provider organisation to import the project into (if it is not already in one)
  -o, --output-dir string              Directory to output the project to. Defaults to the current directory
  -p, --packaging string               Packaging
      --verbose                        Enable verbose logging
```

### SEE ALSO

* [jx create](/commands/jx_create/)	 - Create a new resource

###### Auto generated by spf13/cobra on 4-Mar-2018
