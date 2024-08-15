# Install wdio --> added for git fetch test
- npm init wdio .

# Package.json
-check `type`: `module`

# tsconfig.json
-check `"module": "ESNext"`
-check `"resolveJsonModule"`
-add `"esModuleInterop": true,`
-change `"strict":false`

# wdio.conf.ts
-check `project: "./tsconfig.json`
-add `${process.cwd()}/test/features/**/*.feature`
-add `./test/features/step-definitions/*.ts`
