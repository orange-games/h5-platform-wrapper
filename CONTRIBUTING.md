Before contributing, please read the [code of conduct](CODE_OF_CONDUCT.md).

## Reporting issues

[GitHub Issues][0] is the place to report bugs you may have found. When submitting a bug please do the following:

**1. Search for existing issues.** Your bug may have already been fixed, or cannot, or will not, be fixed. So be sure to search the issues first before putting in a duplicate issue.

**2. Not sure if it's a bug?.** Please ask on the Phaser's slack or discord servers, @AleBles is usually there.

**3. Create an isolated and reproducible test case.** If you are reporting a bug, make sure you also have a minimal, runnable, code example that reproduces the problem you have.

**4. Include a live example.** After narrowing your code down to only the problem areas please provide some basic code that show it, or a link to your live site so that we can view a live example of the problem.

**5. Share as much information as possible.** Include browser version affected, your OS, version of the library, steps to reproduce, etc. "X isn't working!!!!!" will probably just be closed.

## Making Changes

To take advantage of our grunt build script and tslint config it will be easiest for you if you have node.js and grunt installed locally.

You can download node.js from [nodejs.org][3]. After it has been installed open a console and run `npm i -g grunt-cli` to install the global `grunt` executable.

After that you can clone the repository and run `npm i` inside the cloned folder. This will install dependencies necessary for building the project. Once that is ready, make your changes and submit a Pull Request:

- **Send Pull Requests to the `dev` branch.** This'll make it much easier for to keep a clear track between development and releases.

- **Ensure changes are tslint validated.** Our TSlint configuration file is provided in the repository and you should check against it before submitting.

- **Never commit new builds.** When making a code change you should always run `grunt dist` which will rebuild the project so you can test, *however* please do not commit these new builds or your PR will be closed. Builds by default are placed in the `build` folder.

- **Only commit relevant changes.** Don't include changes that are not directly relevant to the fix you are making. The more focused a PR is, the faster it will get attention and be merged. Extra files changing only whitespace or trash files will likely get your PR closed.


## Coding style preferences are not contributions

If your PR is doing little more than changing the source code into a format / coding style that you prefer then we will automatically close it. All PRs must adhere to the coding style already set-out across the code. Your personal preferences for how things should "look" or be structured do not apply here, sorry. PRs should fix bugs, fix documentation or add features. No changes for the sake of change.


## I don't really like git / node.js, but I can fix this bug

That is fine too. While Pull Requests are the best thing in the world for us, they are not the only way to help. You're welcome to post fixes to our forum or even just email them to us. All we ask is that you still adhere to the guidelines presented here re: TSlint, etc.


## Code Style Guide

- Use 4 spaces for tabs, never tab characters.

- No trailing whitespace, blank lines should have no whitespace.

- Always favor strict equals `===` unless you *need* to use type coercion.

- Follow conventions already in the code, and listen to tslint. Our config is set-up for a reason.

[0]: https://github.com/orange-games/h5-ad-wrapper/issues
[3]: http://nodejs.org
