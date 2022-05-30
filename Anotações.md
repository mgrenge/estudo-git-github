# Introdução ao Git

 - Criado em 2005 por Linus Torvalds
 - O Git é um sistema de versionamento de código distribuído

## Entendendo como o Git funciona por baixo dos panos

 - A encriptação gera um conjunto de caracteres identificador de 40 dígitos (SHA1)
 - objetos internos: blobs, trees, commits
 - blob: o git armazena metadados nesses objetos (tipo objeto, tamanho do arquivo, \0, conteúdo)
 - tree: armazena os blobs (\0, aponta para um blob que por sua vez tem um sha1, nome do arquivo). pode apontar também para outras árvores
 - commit: vai dar sentido pra alteração que você está fazendo. Aponta para uma tree, um parente, um autor, uma mensagem. Possui um timestamp

## Primeiros comandos com o GIT

 - git init = inicia o git naquele diretório
 - git add = adiciona quais arquivos o GIT vai rastrear
 - git commit = cria commit com as modificaões atuais
 - arquivo unmodified = depois da commit é o arquivo que não sofreu alteração
 - arquivo modified = sofreu alteração depois da commit
 arquivo staged = pronto para a próxima commit
 - git status = mostra o status do arquivo

# Introdução ao Github

## Trabalhando com o Github

 - git remote add origin [url] = passa o endereço do repositório no github
 - git push origin master = empurra o código para o github

## Resolvendo conflitos

 - git pull origin master = puxa a versão do código que está no github
 - merge conflict = quando há alteração na mesma linha
