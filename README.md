<div align="center" styles="padding: 2rem;">
  <img src="https://github.com/andersnormal/autobot/blob/master/images/logo.png?raw=true" alt="Autobot"/>
</div>

# Autobot Slack Plugin

<a href='https://github.com/jpoles1/gopherbadger' target='_blank'>![gopherbadger-tag-do-not-edit](https://img.shields.io/badge/Go%20Coverage-42%25-brightgreen.svg?longCache=true&style=flat)</a>
![Github Action](https://github.com/andersnormal/autobot-plugin-slack/workflows/Test%20%26%20Build/badge.svg)
[![Go Report Card](https://goreportcard.com/badge/github.com/andersnormal/autobot-plugin-slack)](https://goreportcard.com/report/github.com/andersnormal/autobot-plugin-slack)
[![License Apache 2](https://img.shields.io/badge/License-Apache2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Taylor Swift](https://img.shields.io/badge/secured%20by-taylor%20swift-brightgreen.svg)](https://twitter.com/SwiftOnSecurity)
[![Volkswagen](https://auchenberg.github.io/volkswagen/volkswargen_ci.svg?v=1)](https://github.com/auchenberg/volkswagen)

This is a plugin for :robot: [Autobot](https://github.com/andersnormal/autobot) connecting a [Slack Bot](https://slack.com) to it.

:see_no_evil: Contributions are welcome.

## Usage

The plugin uses the `SLACK_TOKEN` environment variable to connect to the [Slack RTM API](https://api.slack.com/rtm). The plugin can be run with out the server, but it is recommended to do so.

> if you want to run the plugin without the server, you have to configure the environment variables [godoc.org](https://godoc.org/github.com/andersnormal/autobot/pkg/plugins) which are set by the server

```
# Example of running the plugin
./server --verbose --debug --env SLACK_TOKEN=your_token --plugins ../plugins/plugin-slack
```

> when you run the plugin via the server, all `--env` parameters are passed to the started plugins.

## Run

```
go -mod vendor run main.go
```

## Build 

```
go -mod vendor build
```

## License
[Apache 2.0](/LICENSE)
