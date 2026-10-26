# nurman — command cheatsheet lookup

A small Bash utility that retrieves command cheatsheets from cheat.sh and displays them in the terminal. It checks a local per-query cache first; `-fresh` bypasses the cache and updates it.

## Requirements

Bash and `curl`. `less` is optional and used as a pager when the output is a terminal. The default cache is `$HOME/nurtools/nurman/cache`; set `NURMAN_HOME` or `NURMAN_CACHE` to change it. Set `NURMAN_TIMEOUT` to change the network timeout.

```bash
nurman tar
nurman -fresh "git rebase"
nurman -help
nurman -version
```

A cache miss contacts `https://cheat.sh`. Network results are displayed and saved locally; review commands from any cheatsheet before running them.

No license file was supplied, so this repository does not add a license.
