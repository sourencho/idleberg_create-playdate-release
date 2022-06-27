# create-playdate-release

> A GitHub action that compiles and attaches a Playdate game to a release

[![License](https://img.shields.io/github/license/idleberg/create-playdate-release?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/github/v/tag/idleberg/create-playdate-release?style=for-the-badge)](https://github.com/idleberg/create-playdate-release/releases)
[![Status](https://img.shields.io/github/workflow/status/idleberg/create-playdate-release/Tests?style=for-the-badge&label=tests)](https://github.com/idleberg/create-playdate-release/actions)

## Usage

Configure a step that adds the `idleberg/create-playdate-release` action to your workflow. Optionally, you can pass arguments to the action.

```yaml
- uses: idleberg/create-playdate-release@v1.0.0
  with: 
    github_token: ${{ secrets.GITHUB_TOKEN }}
```

## All options

### List of input options

Every argument is optional.

| Input           | Description                                       | Default  |
| --------------- | --------------------------------------------------| -------- |
| `github_token`  | Your GitHub token (`${{ secrets.GITHUB_TOKEN }}`) | –        |
| `source_folder` | The source directory of the project               | `source` |
| `target_folder` | The name of the build target directory            | `build`  |
| `include_files` | List of files to include in the release           | –        |
| `is_draft`      | Mark release is a draft                           | `false`  |
| `is_prerelease` | Mark release is a pre-release                     | `false`  |
| `dry_run`       | Skips creation of a release                       | `false`  |

## License

This work is licensed under [The MIT License](LICENSE).