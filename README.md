# yorkie

> Git hooks made easy

This is a fork of [yorkie](https://github.com/yyx990803/yorkie) with a few changes:

- Prioritizes `package.json` located next to `.git` directory, instead of hard-coded upward search. This avoids the problem when a root package in a lerna monorepo and a sub package both depends on husky, it gets confused and double-updates the root git hooks with wrong paths.

- 修复支持 pnpm 下的安装
