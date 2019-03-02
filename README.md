# openflexo-dev
A template for a development environment for the openflexo framework.


## Installation

### Requirements
We suppose that java (>= 8), gradle (>=3.4.1) and git are installed on your machine.


### Process
1) create a directory for your working env

```
> mkdir work
```

2) cd in that directory

```
> cd work
```

3) clone the various projects you want to work with

For example, let work on connie and openflexo-core

```
> git clone git@github.com:openflexo-team/connie.git
> git clone git@github.com:openflexo-team/openflexo-core.git
> git clone git@github.com:openflexo-team/openflexo-dev.git
```

```
> git clone https://github.com/openflexo-team/connie.git
> git clone https://github.com/openflexo-team/openflexo-core.git
> git clone https://github.com/openflexo-team/openflexo-dev.git
```
You may have to change the branch if the default branch does not match your expectations.

```
> cd connie
> git checkout 1.5
```

Change to the `openflexo-dev` directory and edit the `settings.gradle` file to match your expectations. Here, we decomment connie and openflexo-core.

If you need them you can uncomment some proposed tasks in the build.gradle file.

You can run any task of gradle from within the directory `openflexo-dev`

```
gradle compile
```


For eclipse

You must have at least executed one time the task parser if your development environment contains connie or openflexo-core

1) Create a new workspace

2) Import using `existing gradle project` your previously created `openflexo-dev` directory
Eclipse should create automagically all the needed projects.

If you use a java >= 9, you will have manually configure the buildpath

3) develop, test, push and enjoy.
