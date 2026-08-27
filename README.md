# homebrew-tap

The Homebrew tap for [Firstboot](https://firstboot.io).

```
brew install firstboot-io/tap/firstboot
```

## Nothing here is written by hand

`Casks/firstboot.rb` is generated and pushed by the release job in
[`firstboot-io/cli`](https://github.com/firstboot-io/cli) every time that
repository is tagged. An edit made here is overwritten by the next release, so a
problem with the formula is a change to `.goreleaser.yaml` there.

## Both halves have to stay public

Homebrew clones a tap anonymously and downloads the release assets the cask
names, so this repository and `firstboot-io/cli` are both public. Making either
private breaks `brew install` for everyone, including the person who made it
private.

## License

Apache License 2.0, matching the CLI it distributes.
