# FriendsWave-frontend

## Getting Started

Install dependencies,

```bash
$ yarn
```

Start the dev server,

```bash
$ yarn start
```

Create a release build,

```bash
$ yarn build
```

## Branches specifications

### Deployment branches

- **master**: The production branch. Used to deploy the stable release of the app. Must always be stable.
- **staging**: The testing branch. Used to deploy the next version of master. Must always be stable.
- **nightly**: The development branch. Used to deploy the nightly builds for quick iterations. Can be unstable.

### Development branches

- **feature/...**: A new feature added to the project, addressed as a pull request on nightly.
- **bugfix/...**: A correction is made to the project, addressed as a pull request on nightly.

### Backup branches

- **release/...**: The list of stable releases, created after each update of master. Each of these branches must be stable.
- **stage/...**: The list of application stages, created after each important changes on the code base (new feature). Some of these branches can be unstable.
