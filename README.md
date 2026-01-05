# graphite-goodies

A collection of CLI shortcuts for [Graphite](https://graphite.dev).

## Install

```bash
brew tap adambowker/graphite-goodies
brew install graphite-goodies
```

## Commands

### `gtc` - Quick conventional commits

Interactive prompt for creating branches with conventional commit messages.

```
$ gtc
Type: feat xfix chore f
Scope: surveys product tours p
Message: add URL targeting
→ gt create --all --message "feat(product tours): add URL targeting"
Run? yes no y
```

## Configuration

On first run, `gtc` creates a config file at `~/.config/graphite-goodies/gtc.conf`:

```bash
# gtc config
# Format: key:value,key:value
# Keys are single characters used as shortcuts

types=f:feat,x:fix,c:chore
scopes=s:surveys,p:product tours
```

Customize your types and scopes by editing this file. For example:

```bash
types=f:feat,x:fix,c:chore,d:docs,r:refactor
scopes=a:api,w:web,m:mobile,i:infra
```

## License

MIT
