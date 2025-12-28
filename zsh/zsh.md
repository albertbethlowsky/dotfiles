export ZSH="$HOME/.oh-my-zsh"
ZSH_THEME="amuse"

plugins=(git zsh-autosuggestions zsh-syntax-highlighting z zsh-shift-select)

source $ZSH/oh-my-zsh.sh

#Aliases

alias ngrok_run="ngrok start --all --config ./ngrok.yml"
alias ngrok_stop="ngrok stop --all"
alias cat='bat'    
alias ls='eza --icons=always --git'
alias reload='source ~/.zshrc'
alias code='cursor'

#Paths -- setup openjdk for IOS/expo dev and npm.

function timestamp() {
  date +"%Y%m%d%H%M%S"
}

export LS_COLORS="di=1;34:ln=36:ex=32:fi=38;5;240:"
ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE='fg=66'

PROMPT='%F{208}%~%f$(git_branch_info) %F{66}💻%f %F{66}%*%f
%F{66}|ahammerich|🪬 %f'
