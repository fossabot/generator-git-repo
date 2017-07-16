# `generator-git-repo`
> :octocat: ![Bitbucket icon][bitbucket-image] Initialize and add remote origin for Bitbucket, Bitbucket-Server, GitHub, and GitHub Enterprise repositories.

[![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Coverage percentage][coveralls-image]][coveralls-url] [![Codacy quality gates][codacy-img]][codacy-url]
<br>[![NSP][nsp-img]][nsp-url] [![Dependency Status][daviddm-image]][daviddm-url]

## Table of contents

<!-- toc -->

- [1. Installation](#1-installation)
- [2. Usage](#2-usage)
  * [2.1. Initialize `git` and add remote origin](#21-initialize-git-and-add-remote-origin)
  * [2.2. Compose `generator-git-repo` into your own generator](#22-compose-generator-git-repo-into-your-own-generator)
  * [2.3. List command-line help](#23-list-command-line-help)
- [3. Contributing to `generator-git-repo`](#3-contributing-to-generator-git-repo)
- [4. Testing, linting, checking `generator-git-repo` for known vulnerabilities](#4-testing-linting-checking-generator-git-repo-for-known-vulnerabilities)
- [5. Version and change logs](#5-version-and-change-logs)
- [5. License](#5-license)

<!-- tocstop -->

<!-- tocend -->

## 1. Installation

```sh
# Use it globally
$ npm install generator-git-repo --global

# Or compose into your own Yeoman generator
$ npm install generator-git-repo --save-dev
```

## 2. Usage

### 2.1. Initialize `git` and add remote origin

From a terminal, run:

```sh
$ yo git-repo
```

### 2.2. Compose `generator-git-repo` into your own generator

```js
if (this.options.gitRepo) {
  this.composeWith(
    require.resolve('generator-git-repo/generators/app'),
    options
  )
}
```

### 2.3. List command-line help

Run:

```js
$ yo git-repo --help
```

## 3. Contributing to `generator-git-repo`

[![PRs Welcome][makeapullrequest-image]][makeapullrequest-url] We welcome contributors and pull requests. Check out the guidelines for

* [Contributing to `generator-git-repo`](./.github/CONTRIBUTING.md) and our
* [Contributor Covenant Code of Conduct][code-of-conduct-url].

Contributions are stories with a beginning, a middle, and an end, all told through issues, comments, commit logs, and pull requests.

 * [Peruse open issues][issues-url] or
 * [Open a new pull request (PR)][pr-url]

## 4. Testing, linting, checking `generator-git-repo` for known vulnerabilities
> `generator-git-repo` runs tests, lints source code; checks for vulnerabilities; assesses dependency drift; and executes quality gates with Jest, ESLint, NSP, and Codacy.

To lint, test, and check for known vulnerabilities, just run:

```sh
# npm-script pretest lints the source code
# npm-script test runs jest
$ npm test
# npm-script posttest executes nsp check
```

The results are displayed real-time with README badges.

## 5. Version and change logs

`generator-git-repo`'s latest version is <!-- semver -->[`v0.0.0`][changelog-url]<!-- semverend -->. Please read the [CHANGELOG][changelog-url] for details.

## 5. License

[Apache-2.0][license-url] © [Greg Swindle](https://github.com/gregswindle)

---

[![License][license-image]][license-url] [![FOSSA Status][fossa-image]][fossa-url] [![Readme Score][readme-score-img]][readme-score-url] [![Greenkeeper][greenkeeper-img]][greenkeeper-url]


[author-url]: https://github.com/gregswindle
[bitbucket-image]: https://github.com/gregswindle/generator-git-repo/blob/master/.assets/media/img/bitbucket-favicon.ico_16x16.png
[changelog-url]: https://github.com/gregswindle/generator-git-repo/CHANGELOG.md
[codacy-img]: https://api.codacy.com/project/badge/Grade/fa4ade3f68a04b9cad26165a59ceb88e
[codacy-url]: https://www.codacy.com/app/greg_7/generator-git-repo?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=gregswindle/generator-git-repo&amp;utm_campaign=Badge_Grade
[code-of-conduct-url]: https://github.com/gregswindle/generator-git-repo/blob/master/.github/CODE_OF_CONDUCT.md
[coveralls-image]: https://coveralls.io/repos/gregswindle/generator-git-repo/badge.svg
[coveralls-url]: https://coveralls.io/r/gregswindle/generator-git-repo
[daviddm-image]: https://david-dm.org/gregswindle/generator-git-repo.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/gregswindle/generator-git-repo
[fossa-image]: https://app.fossa.io/api/projects/git%2Bhttps%3A%2F%2Fgithub.com%2Fgregswindle%2Fgenerator-git-repo.svg?type=shield
[fossa-url]: https://app.fossa.io/projects/git%2Bhttps%3A%2F%2Fgithub.com%2Fgregswindle%2Fgenerator-git-repo?ref=badge_shield
[greenkeeper-img]: https://badges.greenkeeper.io/gregswindle/generator-git-repo.svg?style=flat-square
[greenkeeper-url]: https://greenkeeper.io/
[issues-url]: https://github.com/gregswindle/generator-git-repo/issues
[license-image]: https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=flat
[license-url]: https://github.com/gregswindle/generator-git-repo/blob/master/LICENSE
[makeapullrequest-image]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat
[makeapullrequest-url]: http://makeapullrequest.com
[npm-image]: https://badge.fury.io/js/generator-git-repo.svg
[npm-image]: https://badge.fury.io/js/generator-git-repo.svg
[npm-url]: https://npmjs.org/package/generator-git-repo
[npm-url]: https://npmjs.org/package/generator-git-repo
[nsp-img]: https://nodesecurity.io/orgs/gregswindle/projects/6334c8c5-06d5-411c-9722-8b98350818b3/badge
[nsp-url]: https://nodesecurity.io/orgs/gregswindle/projects/6334c8c5-06d5-411c-9722-8b98350818b3
[pr-url]: https://github.com/gregswindle/generator-git-repo/pulls
[readme-score-img]: http://readme-score-api.herokuapp.com/score.svg?url=https://github.com/gregswindle/generator-git-repo
[readme-score-url]: http://clayallsopp.github.io/readme-score?url=https://github.com/gregswindle/generator-git-repo
[travis-image]: https://travis-ci.org/gregswindle/generator-git-repo.svg?branch=master
[travis-url]: https://travis-ci.org/gregswindle/generator-git-repo
