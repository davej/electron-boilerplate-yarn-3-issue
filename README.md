To recreate simple run `yarn` in this directory.

After install has finished then you should see output that ends like this:

```
➤ YN0009: │ electron-boilerplate@workspace:. couldn't be built successfully (exit code 1, logs can be found here: /private/var/folders/h1/9dzghzlx0xgcdw3j5yjk0hg00000gn/T/xfs-bc5c23f7/build.log)
➤ YN0000: └ Completed in 5s 484ms
➤ YN0000: Failed with errors in 44s 972ms
```

If you click into the logs then you will see something like this:

```
# This file contains the result of Yarn building a package (electron-boilerplate@workspace:.)
# Script name: postinstall

  • electron-builder  version=24.9.1
  • loaded configuration  file=package.json ("build" field)
  • rebuilding native dependencies  dependencies=@bugsnag/plugin-electron-app@7.22.2, @bugsnag/plugin-electron-client-state-persistence@7.22.2 platform=darwin arch=arm64
  • rebuilding native dependency  name=@bugsnag/plugin-electron-client-state-persistence version=7.22.2
  • rebuilding native dependency  name=@bugsnag/plugin-electron-app version=7.22.2
  ⨯ cannot execute  cause=exit status 1
                    out=Usage Error: Couldn't find a script named "install".

$ yarn run [--inspect] [--inspect-brk] [-T,--top-level] [-B,--binaries-only] <scriptName> ...

                    command=/private/var/folders/h1/9dzghzlx0xgcdw3j5yjk0hg00000gn/T/xfs-b1ba03f1/yarn run install
                    workingDir=/Users/davejeffery/code/test/electron-boilerplate-yarn-3-issue/node_modules/@bugsnag/plugin-electron-app
```
