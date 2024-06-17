## Script .bat para Limpeza de Arquivos Temporários

Este script .bat remove arquivos temporários dos diretórios padrão do Windows, liberando espaço em disco e melhorando a performance do sistema. Aqui está uma explicação detalhada do que o script faz:

1. **Configuração Inicial**
    - Muda a cor do terminal para vermelho (`color 4`).
    - Exibe uma mensagem informando que a limpeza está começando e aguarda que o usuário pressione qualquer tecla para continuar.

2. **Limpeza de Diretórios Temporários**
    - Remove todos os arquivos no diretório `c:\windows\temp\` se ele existir.
    - Remove todos os arquivos no diretório de arquivos temporários do usuário (`%temp%`).

3. **Limpeza de Diretórios Temporários Específicos**
    - Verifica se o diretório `C:\Documents and Settings\` existe:
        - Para cada subdiretório, remove e recria os diretórios `Local Settings\Temporary Internet Files` e `Local Settings\Temp`.
    - Verifica se o diretório `C:\Users\` existe:
        - Para cada subdiretório, remove e recria os diretórios `AppData\Local\Temp` e `AppData\Local\Microsoft\Windows\Temporary Internet Files`.

4. **Observações Importantes**
    - Este arquivo, assim que executado, criará os logs no local onde for executado.
    - Por exemplo, se executado na pasta Documentos, ele irá recriar as pastas nessa pasta.
    - Este executável tem a extensão `.bat`.
    - É aconselhável executar o .bat na pasta Arquivos e Programas.

**Autor: kelvynnS.**
