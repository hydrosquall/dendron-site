---
id: 87d90002-f480-45eb-a8c4-d00df4d61557
title: Dendron-plugin
desc: ''
updated: 1608838282427
created: 1605375348464
---


# Cook

### Create a new Command

1. Add command to `DENDRON_COMMANDS` under `plugin-core/src/constants.ts`
2. Open the command prompt, enter `Run Task`, and run `gen:config`
    - this will add the command to `package.json`
3. Create the new command in `plugin-core/src/commands/{COMMAND_NAME}.ts`
    - you can copy the contents of an existing command (eg. `src/commands/ShowHelp.ts`) to help you get started
4. Write tests
    - tests are in `plugin-core/src/test/suite-integ/{COMMAND}`
    - testing instructions are [[heree|dendron.dev.testing]]
5. Write command logic
6. Add command to `src/commands/index.ts`
7. Submit pull request