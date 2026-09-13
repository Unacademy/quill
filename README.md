# quill

> Quill is a modern WYSIWYG editor built for compatibility and extensibility.

---

## Table of Contents

1. [Overview](#overview)
2. [Tech Stack](#tech-stack)
3. [Repository Structure](#repository-structure)
4. [Key Components](#key-components)
5. [Setup & Installation](#setup--installation)
6. [Running the Application](#running-the-application)
7. [Infrastructure & CI/CD](#infrastructure--cicd)
8. [Contributing](#contributing)

---

## Overview

**quill** is part of the [Unacademy](https://github.com/unacademy) engineering ecosystem.

Quill is a modern WYSIWYG editor built for compatibility and extensibility.

**Topics / Tags:** `approvers-1`

---

## Tech Stack

| Attribute | Value |
|-----------|-------|
| **Primary Language** | JavaScript |
| **Framework / Platform** | JavaScript |
| **Package Manager** | npm / yarn |

### Dependencies

**Runtime Dependencies:**
- `eventemitter3`
- `lodash.clonedeep`
- `lodash.isequal`
- `lodash.merge`
- `parchment`
- `quill-delta`

**Dev Dependencies:**
- `@babel/core`
- `@babel/preset-env`
- `babel-loader`
- `babel-plugin-istanbul`
- `css-loader`
- `eslint`
- `eslint-config-airbnb`
- `eslint-config-prettier`
- `eslint-import-resolver-webpack`
- `eslint-plugin-import`


---

## Repository Structure

```
quill/
├── .github/
│   ├── CONTRIBUTING.md
│   ├── DEVELOPMENT.md
│   ├── ISSUE_TEMPLATE.md
├── .gitignore
├── .travis.yml
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── Gemfile
├── Gemfile.lock
├── LICENSE
├── README.md
├── _develop/
│   ├── browsers.js
│   ├── jekyll.yml
│   ├── karma.config.js
│   ├── procfile
│   ├── proxy.js
├── assets/
│   ├── base.styl
│   ├── bubble
│   ├── bubble.styl
│   ├── core.styl
│   ├── favicon.png
├── blots/
│   ├── block.js
│   ├── break.js
│   ├── container.js
│   ├── cursor.js
│   ├── embed.js
├── core/
│   ├── editor.js
│   ├── emitter.js
│   ├── instances.js
│   ├── logger.js
│   ├── module.js
... (truncated)
```

---

## Key Components

Below is an analysis of the key files and modules:

| File / Directory | Purpose |
|-----------------|---------|
| `CHANGELOG.md` | Source file |
| `CODE_OF_CONDUCT.md` | Source file |
| `Gemfile` | Source file |
| `LICENSE` | Source file |
| `README.md` | Source file |
| `_develop/browsers.js` | Source file |
| `_develop/jekyll.yml` | Source file |
| `_develop/karma.config.js` | Source file |
| `_develop/procfile` | Source file |
| `_develop/proxy.js` | Source file |
| `_develop/sauce.js` | Source file |
| `_develop/scripts/puppeteer.sh` | Source file |
| `_develop/scripts/release.sh` | Source file |
| `_develop/wdio.config.js` | Source file |

> **Note:** Only the first 20 non-trivial files are listed. See the repository tree above for the complete structure.

---

## Setup & Installation

### Prerequisites

- Git (`git --version`)
- JavaScript runtime installed



### Steps

```bash
# 1. Clone the repository
git clone git@github.com:unacademy/quill.git
cd quill

# 2. Install dependencies
npm install      # or yarn install
```

### Available Scripts

```bash
# build
npm run build   # npm run lint && npm run build:webpack

# build:webpack
npm run build:webpack   # webpack --config _develop/webpack.config.js; rm dist/quill.core dist/quill.bubble dist/quill.snow

# build:release
npm run build:release   # ./_develop/scripts/release.sh

# develop
npm run develop   # npm run start

# lint
npm run lint   # eslint blots core formats modules themes ui test

# start
npm run start   # npm run build:webpack; bundle exec foreman start -f _develop/procfile

# test
npm run test   # npm run test:unit

# test:all
npm run test:all   # npm run test:unit; npm run test:functional

# test:functional
npm run test:functional   # ./_develop/scripts/puppeteer.sh

# test:unit
npm run test:unit   # npm run build; karma start _develop/karma.config.js

```


---

## Running the Application

```bash
npm run start   # npm run build:webpack; bundle exec foreman start -f _develop/procfile
```

---

## Infrastructure & CI/CD

- Test suite present — run tests before submitting PRs

---

## Contributing

1. Create a feature branch: `git checkout -b feat/your-feature`
2. Commit your changes: `git commit -m "feat: describe your change"`
3. Push and open a PR targeting `develop`
4. Ensure all CI checks pass before requesting review

---

## Original README (Excerpt)

> Note: This branch and README covers the upcoming 2.0 release. View [1.x docs here](https://github.com/quilljs/quill/tree/1.3.6).

<h1 align="center">
  <a href="https://quilljs.com/" title="Quill">Quill Rich Text Editor</a>
</h1>
<p align="center">
  <a href="https://quilljs.com/" title="Quill"><img alt="Quill Logo" src="https://quilljs.com/assets/images/logo.svg" width="180"></a>
</p>
<p align="center">
  <a title="Quickstart" href="#quickstart"><strong>Quickstart</strong></a>
  &#x2022;
  <a title="Documentation" href="https://quilljs.com/docs/"><strong>Documentation</strong></a>
  &#x2022;

---

*This README was auto-generated on 2026-09-14 by the Unacademy repo-summarizer tool.*
*For corrections or additions, edit this file directly or open an issue.*
