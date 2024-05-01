Comando para descrever arvore de diretórios a partir do atual
```bash
find . -type d | sed -e "s/[^-][^\/]*\//  |/g" -e "s/|\([^ ]\)/| - \1/"
```
Descrever diretórios e arquivos
```bash
find | sed 's|[^/]*/|- |g'
```