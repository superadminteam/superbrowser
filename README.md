# superadmin-cli

Visual Automation CLI for [superadmin.so](https://superadmin.so)

- [Read the docs](https://superadmin.so/docs)
- [Signup](https://dashboard.superadmin.so/signup)

## Getting Started

You'll need to signup for an account at [superadmin.so](https://superadmin.so). Superadmin is fast and easy visual automation testing for developers and teams. Useful for regression testing, and no-code visual automations that enable teams to ship code with confidence. Receive alerts when unexpected changes occur, and quickly setup new tests to keep testing your apps effortless.

## Installation

```bash
$ npm install -g superadmin-cli
```

## Usage

```bash
$ superadmin-cli -h
Usage: superadmin-cli [options]

Read the docs at https://superadmin.so/docs for more information.

Options:
  -V, --version              output the version number
  -k, --api-key <key>        Set the Authentication Key, env SUPERADMIN_API_KEY
  -p, --projects <names>     Set the projects to run, env SUPERADMIN_PROJECTS
  -t, --tags <tag>           Set Build tags e.g. 'staging', env SUPERADMIN_TAGS
  --use-localtunnel <value>  Set localtunnel usage (auto, yes, no) (default: "auto")
  --ignore-dotenv            Ignore `.env` file
  -v, --verbose              Verbose logging
  -E, --environment          Log Process Environment
  -h, --help                 display help for command
```

## Example Usage

```shell
$ SUPERADMIN_API_KEY=ey... superadmin-cli -P "Engineering=http://localhost:4000" -t staging
```

Run only tests for the project **"Engineering"** at `localhost:4000` and set the build tag to `staging`.

```shell
$ SUPERADMIN_API_KEY=ey... superadmin-cli -t production
```

Run all tests for all projects at their set domain and set the build tag to `production`.

## Learn More

Signup for a free account at [superadmin.so](https://superadmin.so). Read the documentation about the cli and visual testing system at [https://superadmin.so/docs](https://superadmin.so/docs)
