# urlencode-bash-functions
BASH/ZSH shell functions that can url encode and decode without needing any packages on Linux or Mac, take input as argument or stdin

The sh file sould be sourced to define functions in the current shell, add to .bashrc or .zshrc to always load.

Example of use:

    bash$ source urlencode-functions.sh
    bash$ url-encode 'This & that!'
    This%20%26%20that%21
    bash$ echo -e "Zoë ate hors d'œuvres" | url-encode
    Zo%C3%AB%20ate%20hors%20d%27%C5%93uvres
    bash$ url-decode Zo%C3%AB%20ate%20hors%20d%27%C5%93uvres
    Zoë ate hors d'œuvres
    bash$ 
