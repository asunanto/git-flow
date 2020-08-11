# git-flow
documentation for the use of git flow

## initialising workflow
```
git flow init -y
```
short for
```
git branch develop
git push -u origin develop
```

## Feature Branches

### Creating a feature branch
```
git flow feature start feature_branch
```
short for
```
git checkout develop
git checkout -b feature_branch
```
### Finishing a feature branch
```
git flow feature finish feature_branch
```
short for
```
git checkout develop
git merge feature_branch
```

## Release Branches
```
git flow release start 0.1.0
```
short for
```
git checkout develop
git checkout -b release/0.1.0
```

```
git flow release finish '0.1.0'
```
short for
```
git checkout master
git merge release/0.1.0
```