<p align="center">
  <img alt="GitHub Logo" src="docs/github_logo.png" height="140" />
  <h3 align="center">Go Git</h3>
  <p align="center">Automatically tag your repository!</p>
  <p align="center">
    <a href="https://github.com/oshalygin/go-tag/releases/latest"><img alt="Release" src="https://img.shields.io/github/release/oshalygin/go-tag.svg?style=flat-square"></a>
    <a href="https://travis-ci.org/oshalygin/go-tag"><img alt="Travis" src="https://travis-ci.org/oshalygin/go-tag.svg?branch=master"></a>
    <a href="/LICENSE.md"><img alt="Software License" src="https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square"></a>
    <a href="https://coveralls.io/github/oshalygin/go-tag?branch=master"><img alt="Coveralls" src="https://coveralls.io/repos/github/oshalygin/go-tag/badge.svg?branch=master"></a>
    <a href="https://codeclimate.com/repos/596c01297de38412b7000136/feed"><img alt="Code Climate Issue Count" src="https://codeclimate.com/repos/596c01297de38412b7000136/badges/d8e88772201d137ea8b7/issue_count.svg"></a>
    <a href="https://goreportcard.com/report/github.com/oshalygin/go-tag"><img alt="Go Report Card" src="https://goreportcard.com/badge/github.com/oshalygin/go-tag"></a>
    <a href="https://godoc.org/github.com/oshalygin/go-tag"><img src="https://godoc.org/github.com/oshalygin/go-tag?status.svg" alt="GoDoc"></a>
  </p>
</p>

# Introduction

This is a simple and straightforward CLI utility that automatically tags your repository.

## Motivation

Commonly, you'll want to automate your tagging process.  As you release features, you'll add a version somewhere within your application, for Node.js projects this is `package.json`.  This whole process is time consuming and repetitive, why not let a utility handle this automatically?

* Ensuring your repository is properly tagged based on release versions

## Requirements

Without bloating the utility with a ton of _required_ options, the `go-tag` utility depends on certain aspects being present in each of your git repositories.

* You are authorized to push against the repository.
* All of the credentials are properly configured in your shell.

### Installation

```bash
go get -u github.com/oshalygin/go-tag
```

### Usage

```bash
# Call the utility and enjoy the automation!

go-tag

```

### Command Line Arguments

None, this utility is called within the current git repository and it will make the rest happen!

### Limitations

This utility depends on _you_ having the right credentials set.

Additionally, this utility only works with Node.js projects, namely projects with a `package.json` file.  The reason for this is because the application looks into this configuration file to determine what tag version to set.

In the future, tagging will be much more automated.

# License

[MIT](LICENSE)
