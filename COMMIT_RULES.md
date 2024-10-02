# Commit conventions

## Prefix/Type:
#### All prefix should include a () after the prefix to specify what is the change specifically (for example a function name, a file name, a variable name, or a general description of where the change is made)
- `feat`: A new feature is introduced with the change
- `fix`: A bug is fix has occured
- `chore`: Changes that do not relate to a fix or a feature and don't modify the code (for example adding `.gitignore`)
- `bump`: Bumps a version of a package or the project itself(need specification on what is bumped), specify the version bumped from and to with a arrow(->) (for example, `bump(package.json): 1.0.0 -> 1.0.1`)
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `docs`: Updates to the documentation such as README.md or other documentation files
- `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- `test`: Including new or correcting existing tests
- `perf`: Performance Improvements
- `ci`: Continues Integration related changes
- `build`: Changes that affect the build system or external dependencies
- `security`: Changes that are related to security
- `revert`: Reverts a previous commit (need specification on what is reverted)(doesn't nessesarily have to be a commit)
- `change`: Changes that are not a fix or a feature, just a general change(need specification on what is the change)
- `remove`: Removes something in the code, don't nessesarily have to be a bug(need specification on what is removed)
- `move`: Moves one file to another place, specify with a arrow(->) where the file is moved to (for example, `move(reason/notes): file1 -> file2`)
- `add`: Adds something in the code, or file(mention the file in "()"), don't nessesarily have to be a feature(need specification on what is added)
- `sync`: Syncs the code with another branch or repository(need specification on what is synced)
- `enable`: Enables a feature or a function(need specification on what is enabled), specific for configs
- `change`: Changes that are not a fix or a feature, just a general change(need specification on what is the change), usually a change in tool/utility
- `BREAKING CHANGE`: A commit that has a breaking change that will affect the codebase
##### Example:
- `feat(functionName): Added a new function that does something`

## Subject
#### The subject contains a succinct description of the change, and if possible a reason for the change:
##### Example:
- A: "Add margin"
- B: "style(footer): Add margin to nav times to prevent them from overlapping the logo"
In this example, A is a bad subject because it doesn't specify what is being changed, while B is a good subject because it specifies what is being changed and why it is being changed.

## Body / Description (optional)
#### In a commit message, the body is optional and is used to explain what and why the change was made. The body should be used to explain the reasoning behind the change and what the change does. The body should be written in the present tense and should explain what the commit does and why it does it.
##### Example:
- `feat(functionName): Added a new function that does something`
#### Usage:
Use `git -m subject/title -m body/description` to add a body to a commit message
#### Any changes that is not the main changes but is in the commit should be added to the body

## General
- Length:
    - The subject should be no longer than 50 characters
    - the body should be wrapped at 72 characters
- Be direct and to the point
    - Try to eliminate unnecessary words (for example, "though", "maybe", "I think", "kind of", etc)
- If applicable, include a reference to a GitHub issue stating a fix, feature, or issue that is being addressed

## Always think about:
- Why have I made these changes?
- What effect have my changes made?
- Why was the change needed?
- What are the changes in reference to?

## TIPS
- Checkout (Commitizen)[https://commitizen-tools.github.io/commitizen]
