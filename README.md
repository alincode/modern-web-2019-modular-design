# Modern Web 2019

### yarn workspace

```
yarn workspace app-api-server add lodash
yarn workspace app-api-server remove lodash

yarn workspace app-api-server remove lodash --dev
```

**參考資料**

* [Workspaces](https://yarnpkg.com/lang/en/docs/workspaces/)
* [yarn workspace](https://yarnpkg.com/en/docs/cli/workspace)

### lerna.js

```
$ lerna init

lerna notice cli v3.16.4
lerna info Creating package.json
lerna info Creating lerna.json
lerna info Creating packages directory
lerna success Initialized Lerna files
```

**其他常用指令**

```
lerna clean
lerna list
```

lerna add <package>[@version] [--dev]

```
lerna add jest --dev
lerna add os --scope=@rooit/server
lerna add @rooit/lib-node --scope=@rooit/api-server
```

### Conventional Commits

**structured**

```
<type>[optional scope]: <description>

[optional body]

[optional footer]
```

**Examples**

```
feat: allow provided config object to extend other configs
feat(lang): add polish language

# 零星工作
chore!: drop Node 6 from testing matrix

docs: correct spelling of CHANGELOG

fix: correct minor typos in code
```

**參考資料**

* [Conventional Commits 1.0.0-beta.4](https://www.conventionalcommits.org/en/v1.0.0-beta.4/)
* [Commit Message Guidelines | Contributing to Angular](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)