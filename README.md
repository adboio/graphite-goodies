# graphite-goodies

A collection of CLI shortcuts for [Graphite](https://graphite.dev).

## Install

```bash
brew tap adboio/graphite-goodies
brew install graphite-goodies
```

## Commands

### `gtc` - Quick conventional commits

Interactive prompt for creating branches with conventional commit messages.

```
$ gtc
Type: [f]feat [x]fix [c]chore f
Scope: [s]surveys [p]product tours p
Message: add URL targeting
→ gt create --all --message "feat(product tours): add URL targeting"
Run? yes no y
```

## Configuration

On first run, `gtc` runs a setup wizard to help you create a config file at `~/.config/graphite-goodies/gtc.conf`:

```bash
# gtc config
# Format: key:value,key:value
# Keys are single characters used as shortcuts

types=f:feat,x:fix,c:chore
scopes=s:surveys,p:product tours
```

Customize your types and scopes any time by running `gg-setup`, or edit the file directly:

```bash
types="f:feat,x:fix,c:chore,d:docs,r:refactor"
scopes="a:api,w:web,m:mobile,i:infra"
```

## License

MIT
