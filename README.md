# SolutionItems sync tool

Run this against a `.sln` file with a list of paths and it will update the solution items to match

## Install

```sh
dotnet tool install --global sln-items-sync
```

You'll need `~/.dotnet/tools` on the PATH if it isn't already.

## Update

```sh
dotnet tool update -g sln-items-sync
```

## Usage

```sh
sln-items-sync --solution sln-items-sync.sln README.md .github
```

Files and folders will be recursively add/removed to match the filesystem.

`SolutionItems` folder will be created and populated if missing. The name can be customized with `--folder`.

## Backstory

If you're interested in how this came about read [the genesis story of sln-items-sync](https://timwise.co.uk/2024/01/13/new-tool-sln-items-sync-for-visual-studio-solution-folders/) on my blog.
