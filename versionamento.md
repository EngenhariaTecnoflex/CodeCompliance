# 2. Versionamento

O controle de versão de código deve ser realizado preferencialmente através da ferramenta GIT.

A hospedagem deve ser realizada preferencialmente na plataforma GITHUB dentro da organização EngFlex, salvo exceções definidas pelo gestor do projeto.

## TAGs

A versão de lançamentos deverá ser **obrigatoriamente** registrada através de uma TAG.

As tags devem ser compostas de dois numerais separadas por ponto e iniciadas pela letra 'v' mínuscula, no formato "vX.Y". Por exemplo:

    v1.0

Considerando o formato "vX.Y", o numeral Y deve ser incrementado quando houver pequenas modificações. Já o numeral na posição X deve ser incrementado quando houver grandes modificações.

As tags devem ser **obrigatóriamente** integradas ao código fonte em formato string e **opcionalmente** em outros formatos.

Recomenda-se o uso de ferramentas automatizadas para a geração das strings no momento de compilação. Ver componente Git_tools.

Adicionalmente, caso seja gerada uma versão prévia, mas ainda não liverada para o cliente, pode-se acrescer ao final da tag, e separados por um sinal '-' as indicações: do numero de commits des-de a ultima tag, do hash reduzido do ultimo commit e a inclusão palavra "dirty" ao final. Como no exemplo:

    v1.0-20-gee479a5-dirty

A geração dessa string pode ser realizaad através do comando.

```bash
git describe --tags --dirty --always
```

### *Alterações pequenas*

Alterações pequenas são todas as alterações que corrigem algum comportamento defeituoso (*bug*) de uma versão anterior.
Também são consideradas alterações pequenas aquelas que adicionam alguma nova funcionalidade, mas que não altera significativamente o comportamento das funcionalidades anteriores.

### *Alterações grandes*

Alterações grandes compreendem todas as alterações significativas no código que alteram o comportamento das funcionalidades já entregues.
Também são consideradas grandes alterações as refatorações que modificam mais de um arquivo.

---

## Links úteis

[Comandos básicos de GIT](https://education.github.com/git-cheat-sheet-education.pdf)

[EngFlex no GITHUB](https://github.com/EngenhariaTecnoflex)