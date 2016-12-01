# Frontend Boilerplate
> It's how I like it, fork before using it.

### Setup
```bash
  # clone the repository
  λ git clone https://github.com/umayr/frontend-boilerplate
  # change the current directory
  λ cd frontend-boilerplate
  # install all dependencies
  λ yarn install
  # run the project
  λ yarn start
```

### Structure
```bash
.
├── README.md           # you're here
├── bin                 # folder that bootstraps the application
├── src                 # contains source files
│   ├── action          # folder that contains all redux actions
│   ├── component       # directory that holds all components
│   ├── config          # contains configuration files for client-side
│   ├── constant        # contains all constants, can be both server and client side
│   ├── container       # wraps all redux containers
│   ├── middleware      # folder with all middlewares
│   ├── reducer         # directory that contains all redux reducers
│   └── service         # contains all the backend service logic
│   └── store           # wraps store configuration for redux
│   └── route           # contains all routes for redux app
└── webpack             # contains all webpack configurations
```

**Suggestion:** Every folder name is _singular_ like `endpoint`, `middleware` instead of `endpoints`, `middlewares`. If you want to add more folders as per your need, make sure they should be singular too (for e.g. `util`, `helper` etc) only for the sake of consistency.

### Scripts

- `yarn start` - builds the redux app in development mode
- `yarn run lint` - lints all the files in `src/` folder
- `yarn run lint:fix` - fixes all the possible linting errors
- `yarn run serve` - serves the files in the `dist/` folder

### Commit Guidelines

The commit message formatting can be added using a typical git workflow

#### Commit Message Format
Each commit should be written in concise and consistent fashion using imperative commit message style.

Any line of the commit message cannot be longer 100 characters! This allows the message to be easier
to read on GitHub as well as in various git tools.

#### Revert
If the commit reverts a previous commit, it should begin with `Revert: `, followed by the header of the reverted commit. In the body it should say: `This reverts commit <hash>.`, where the hash is the SHA of the commit being reverted.
#### Subject
The subject contains succinct description of the change:

* Use the imperative, present tense: "change" not "changed" nor "changes"
* Capitalize first letter
* No dot (.) at the end

#### Body
Just as in the **subject**, use the imperative, present tense: "change" not "changed" nor "changes".
The body should include the motivation for the change and contrast this with previous behavior.

#### Footer
The footer should contain any information about **Breaking Changes** and is also the place to
reference GitHub issues that this commit **Closes**.

**Breaking Changes** should start with the word `BREAKING CHANGE:` with a space or two newlines. The rest of the commit message is then used for this.


### License
MIT
