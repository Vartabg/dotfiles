# 🧠 Elite CLI Tool Cheatsheet

Minimal reference for high-performance terminal-based tools.

---

## 📁 fzf – Fuzzy Finder
- `findf` — Interactive file finder  
- `cat file.txt \| fzf` — Search lines in a file  
- `history \| fzf` — Search shell history  
- `cd \$(findf)` — Change into selected folder  

## 🔍 ripgrep (rg)
- `search term` — Recursively grep  
- `rg -i "term"` — Case-insensitive  
- `rg -t py "def "` — Limit to Python files  
- `rg --files` — List tracked files  

## 📊 jq
- `json <<< '{"a":1}'` — Pretty-print  
- `json '.a' <<< '{"a":1}'` — Extract  
- `curl ... \| jq '.'` — Format API response  

## 📖 bat
- `cat file.py` — Syntax-highlighted output  
- `bat -p file.py` — Plain view  

## 📂 eza
- `ls` — Git-aware long list  
- `eza -T` — Tree view  

## 📈 htop
- `top` — Launch system monitor  
- `F2` = Setup, `F3` = Search, `F9` = Kill  

## 🧪 shellcheck
- `shellcheck file.sh` — Lint shell script  

## 🧼 flake8 / pylint
- `flake8 script.py` — PEP8 linter  
- `pylint script.py` — Static analysis  

## 🔐 direnv
- `echo 'export VAR=1' > .envrc`  
- `direnv allow`  
- Hook: `eval "$(direnv hook zsh)"`  

## 📈 graphviz
- `dot -Tpng diagram.dot -o out.png`  

## 🔧 gh (GitHub CLI)
- `gh auth login`  
- `gh repo clone owner/repo`  
- `gh pr create -f`  

## 🔂 tig
- `tig` — Git log viewer  
- `tig status`, `tig blame file.py`  

## 📋 task
- `task init` — Create Taskfile.yml  
- `task` / `task build` — Run tasks  
