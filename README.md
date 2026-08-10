# NovaShang's Homebrew tap

One tap for everything I ship on macOS.

```sh
brew install --cask NovaShang/tap/bento-term
```

Tapping is implicit — `brew install` with the fully qualified name adds the
tap on first use. To add it up front, `brew tap NovaShang/tap`.

## What's here

| Name | Kind | What it is |
| --- | --- | --- |
| [`bento-term`](Casks/bento-term.rb) | Cask | [Bento Term](https://bentoai.dev/term/) — a terminal that runs a team of AI coding agents in parallel. Source: [NovaShang/BentoTerm](https://github.com/NovaShang/BentoTerm) |

## How these stay current

Each project's own release workflow rewrites its `version` and `sha256` here
after publishing a tagged release, so nothing in this repo is edited by hand.
A project that wants in needs push access to this repo — a fine-grained token
scoped to `contents: write`, stored as a secret in that project.

The repo has to be named `homebrew-tap`: Homebrew resolves the tap name
`NovaShang/tap` by prepending `homebrew-`, with no fallback to a bare name.

## License

Each packaged project keeps its own license. The packaging files here are
Apache-2.0, matching Bento Term.
