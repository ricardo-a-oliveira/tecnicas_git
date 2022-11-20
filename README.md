# tecnicas_git
comandos para assinar commit

## Gera a chave
 gpg --full-generate-key 

 ## Lista as chaves
 gpg --list-secret-key --keyid-form LONG

 ## Exporta chave public
 gpg --armor --export <ID_CHAVE>

 ## Configurar a chave no git
 git config --global user.signingkey <ID_CHAVE>
 git config commit.gpgsign true

 ## Adicionar variavel de ambiente
 GPG_TTY=$(tty)

 ## editando uma chave
 gpg --edit-key <ID_CHAVE>

 add
 save
