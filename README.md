# Workflow


> This document is written to help you with your workflow.


## Go to liferay-portal (Master)

```bash
$ cdt && g co master
 ```

## OBS:

> Pay attention if you are really in the master. If you're modifying some file, you're probably on your branch.

### Commit your changes or save

save your files:
```bash
$ g stash && g co master
```

### Update your local repository

> OBS: Do this on master

```bash
$ g pull upstream master
```
### Update your remote repository

```bash
$ g push origin master
```
## OBS:

> Clean modules from the packages folder once a week.

```bash
$ ant all
```
### Go back to your project's branch

```bash
$ g co <nome da branch>
```
Now that everything is up to date, bring back your saved changes.

> OBS: Do this on your branch

```bash
$ g stash apply
```

# Check the container

>Check if your container is running

```bash
$ d ps
```

If it's not running, then start the container

```bash
$ d start <nome ou hash do container>
```
# Run the catalina

> Open another terminal flap to run the catalina.

catalina's path

> cd dev/bundles/master/tomcat-9.0.53/bin

```bash
$ ./catalina.sh run
```

# Upload the codes with visual code

```bash
$ code .
```

> This is our workflow

> Now you can continue making changes to your code after updating your portal.
