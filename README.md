## Fuzzy Go Docs

The scripts in this repository, mainly `fzgd` (fuzzy go docs) lets you browse Go stdlib documentation
using fzf. It gives both package and symbol documentation

[video]

### Requirements
* `fzf`
* `bat` (for syntax highlighting, not necessary)

### Setup
```
git clone https://github.com/diwasrimal/fuzzy-go-docs.git
cd fuzzy-go-docs
cp fuzzy-go-docs/fzgd* ~/.local/bin/ # somewhere in your path
```
Both scripts should be put in same directory

### Usage
Browse docs with. 
```
fzgd
```
Initial run also creates a cache at `$GOPATH/go-std-doc-cache` or `$HOME/.cache/go-std-doc-cache`

Update doc cache
```
fzgd -u
```

### Navigation
* `tab`: Go inside the pacakge and show symbol documentation
* `shift-tab`: Come back and show package level documentation
* `ctrl-j`: Scroll the preview window down
* `ctrl-j`: Scroll the preview window up
