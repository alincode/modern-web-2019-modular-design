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

```
命令：
  lerna add <pkg> [globs..]  Add a single dependency to matched packages
  lerna bootstrap            Link local packages together and install remaining package dependencies
  lerna changed              List local packages that have changed since the last tagged release          [別名: updated]
  lerna clean                Remove the node_modules directory from all packages
  lerna create <name> [loc]  Create a new lerna-managed package
  lerna diff [pkgName]       Diff all packages or a single package since the last release
  lerna exec [cmd] [args..]  Execute an arbitrary command in each package
  lerna import <dir>         Import a package into the monorepo with commit history
  lerna init                 Create a new Lerna repo or upgrade an existing repo to the current version of Lerna.
  lerna link                 Symlink together all packages that are dependencies of each other
  lerna list                 List local packages                                                       [別名: ls, la, ll]
  lerna publish [bump]       Publish packages in the current project.
  lerna run <script>         Run an npm script in each package that contains that script
  lerna version [bump]       Bump version of packages changed since the last release.

Global Options:
  --loglevel       What level of logs to report.                                                    [字串] [預設值: info]
  --concurrency    How many processes to use when lerna parallelizes tasks.                            [數字] [預設值: 4]
  --reject-cycles  Fail if a cycle is detected among dependencies.                                                 [布林]
  --no-progress    Disable progress bars. (Always off in CI)                                                       [布林]
  --no-sort        Do not sort packages topologically (dependencies before dependents).                            [布林]
  --max-buffer     Set max-buffer (in bytes) for subcommand execution                                              [數字]
  -h, --help       顯示說明                                                                                        [布林]
  -v, --version    顯示版本                                                                                        [布林]
```