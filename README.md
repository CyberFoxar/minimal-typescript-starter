
# Minimal Typescript starter
This project is my (CyberFoxar) minimal typescript starter project. It is _not_ as-is production-ready, but is meant more as a toy project to quickly try out and start stuff.

It has what I consider a "minimal easy config": 
- Using [yarn](https://yarnpkg.com/) as a package manager, because I like it.
- [Typescript](https://www.typescriptlang.org/), because types are nice
  - The types for everything else, too.
- [esLint](https://eslint.org/), because linting is nice to have
  - A bunch of plugins to make eslint work with typescript (from their [getting started page][eslint-typescript], and their autoconfig [here][eslint-autoconfig])
- [prettier](https://prettier.io/), because I don't feel like configuring eslint much
- [mocha](https://mochajs.org/), because tests should always be done
- A few runner tools like:
  - [nodemon](https://www.npmjs.com/package/nodemon), to provide an easy dev server
  - [ts-node](https://www.npmjs.com/package/ts-node), to compile and run typescript without having to use tsc

[eslint-typescript]:https://eslint.org/docs/latest/user-guide/configuring/plugins#specifying-parser
[eslint-autoconfig]:https://eslint.org/docs/latest/user-guide/getting-started

There is a lot of config files (*.json in root) that should make the tools painless to use, and somewhat easy to configure. Be aware that prettier's rules override eslint's when configuring both, see also [this write-up on prettier's website](https://prettier.io/docs/en/integrating-with-linters.html).

You should be able to remove any of those component without too much pain as-is.

I advise you to take a look at the [package.json](./package.json) for the run scripts and dependencies. The only unusual thing would be the use of a [tsconfig-build.json](tsconfig-build.json) to remove the test from compilation output (but still have mocha read them when developping).

There is also in the [.vscode](.vscode/) folder, a small Visual Studio Code workspace that has 2 recommended extensions and the configuration needed to make them work, use it as you wish.

# More Resources
Inspiration for this repo taken from those tutorials:

- https://bobaekang.com/blog/minimal-typescript-project-setup-for-curious-minds/
- https://khalilstemmler.com/blogs/typescript/node-starter-project/

And should also explore:
- https://github.com/Microsoft/TypeScript-Node-Starter
- https://www.typescriptlang.org/download
- https://mindsers.blog/fr/post/coder-serveur-http-nodejs/

About using mocha:
https://javascript.info/testing-mocha

