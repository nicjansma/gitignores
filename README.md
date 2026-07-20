# gitignores

A collection of reusable `.gitignore` templates.

## Templates

### [user-home](user-home)

A `.gitignore` for keeping your home directory (`~`) under version control while excluding the noise that accumulates there. It ignores:

* **Logs and temporary files** — `*.log`, `*.tmp`, `*.bak`, swap files, caches
* **Shell history** — `.*_history` (e.g. `.bash_history`, `.zsh_history`)
* **Archives and packages** — `*.zip`, `*.tar`, `*.gz`, `*.deb`, `*.rpm`, `*.msi`, etc.
* **Data files** — `*.csv`, `*.db`, `*.sqlite`, `*.sql`, etc.
* **OS clutter** — `.DS_Store`, `Thumbs.db`, `$RECYCLE.BIN/`, `__MACOSX/`
* **Development artifacts** — `node_modules/`, `build/`, `vendor/`, `coverage/`, IDE files (Eclipse, Visual Studio, IntelliJ)
* **Security-sensitive files** — `*.pem`, `*.ppk`, `secring.*`, `*.tfvars`
* **AI coding tools** — Claude Code, OpenAI Codex, and Gemini CLI local files and logs

### Usage

Copy the template to where you want it, e.g.:

```sh
curl -o ~/.gitignore https://raw.githubusercontent.com/nicjansma/gitignores/main/user-home
```

Then initialize a repository in your home directory:

```sh
cd ~
git init
git add .gitignore
git commit -m "Initial commit"
```

## License

MIT

## AI Disclosure

No AI was used in creating this repository.