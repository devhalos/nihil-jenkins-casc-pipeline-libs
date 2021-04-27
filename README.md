# Common Infra Jenkins Libs

Jenkins pipeline shared libraries

## Getting Started

### Prerequisites

- Nodejs

### Installing

Install npm dependencies. It is needed for git message linting and for generating changelog for release.

```shell
npm ci
```

## Running the tests

TBD

## Deployment

### Deploy Jenkins to ECS

TBD

### Generating Changelog for Release

We use [standard-version](https://github.com/conventional-changelog/standard-version) to generate release changelog. The changelog will use the commit messages, so the format must confirm to [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/).

```shell
# update version base on the commit messages after the previous release
npm run release 

# update patch version, e.g from 1.0.0 to 1.0.1
# use only for bug fixes that introduce no breaking changes
npm run release:patch 

# update minor version, e.g from 1.0.0 to 1.1.0
# for new features that do not introduce breaking changes
npm run release:minor 

# update major version, e.g from 1.0.0 to 2.0.0
# for new features/bug fixes that introduce breaking changes
npm run release:major
```

## Built With

* [Nodejs](https://nodejs.org/en/) - Use for git commit linting and changelog generation

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

* **Jayson Ojeda** - *Initial work* - [Nihil Project](https://devhalos.atlassian.net/wiki/spaces/NIH)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the GNU GENERAL PUBLIC LICENSE version 3 - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

TBD

