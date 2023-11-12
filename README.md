# setup-nots-cli

Download, install and setup the Nots.dev CLI.

## Usage

```yaml
- uses: nots-dev/setup-nots-cli@v0
  with:
    deploy-token: ${{ secrets.NOTS_TOKEN }}
    server: https://nots.dev
    version: latest
```

## Inputs

| Name           | Description                                    | Required | Default     |
| -------------- | ---------------------------------------------- | -------- | ----------- |
| `deploy-token` | The deploy token for your Nots project or app. | `false`  | `undefined` |
| `server`       | The Nots.dev server to connect to              | `false`  | `undefined` |
| `version`      | The version of the Nots.dev CLI to use.        | `false`  | `latest`    |

## Outputs

| Name           | Description                                         | Example             |
| -------------- | --------------------------------------------------- | ------------------- |
| `nots-version` | The version of the Nots.dev CLI that was installed. | `0.0.1`             |
| `nots-path`    | The path to the Nots.dev CLI that was installed.    | `~/.local/bin/nots` |
