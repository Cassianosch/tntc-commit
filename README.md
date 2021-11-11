## Especificações de commits na estrutura de projetos

Neste projeto vamos abordar as especificações e regras de commits que devem ser seguidos nos projetos.

### Sumário

[Assista ao vídeo](https://www.loom.com/share/ba9c263f3c1943719e295d9da387236d){target="_blank"}
Senha: tntc

Estaremos usando de base a especificação de convenção de commits que nos fornece várias regras simples para criar e explicar o histórico de commits, o que deixa isso mais fácil e automatizado. Essas especificação terão por base [CM](https://www.conventionalcommits.org/en/v1.0.0/#specification), mas com algumas mudanças nas regras para encaixar no perfil. <br />

### As mensagem de commits devem ser estruturadas da seguinte forma:
> tipo[módulo(opcional)]: descrição
>
> [corpo opcional]
>
>[rodapé(s) opcional(s)]

##### Os commits contém elementos estruturais, para comunicar o que está sendo feito naquele commit.
1. **fix** - Vai corrigir um erro no código
2. **feat** - Vai adicionar um recurso novo ai código
3. **refactor** - Refatorar alguma parte do código, não adicionou recurso novo nem corrigiu um bug
4. **revert** - Vai reverter alguma parte do código/commit
5. **Finish v0.0.1** - Criou uma release de commit, padrão do Smart Git
6. **style** - Para css, formatação, falta de ponto e virgula, ajuste de sintaxe
7. **test** - Adição de teste 
8. **perf** - Adição ou ajuste de código que melhora a performance do app
9. **ci** - Processo deploy
10. **chore** - Processo de build ou adição de ferramentas refente a isso
11. **docs** - Mudanças na documentação

#### Exemplos

>Input que deve ser inserido um valor monetário, foi para produção sem a máscara, mas se notou que era **melhor ser inserido**

`feat[carrinho-de-compra]: Adicionado mascara no input de valor de compra` <br />
`feat: Adicionado mascara no input de valor de compra`

---

>Tinha um bug no input que deve ser inserido um valor monetário e foi para produção sem a máscara, **mas deveria ter ido com**

`fix[carrinho-de-compra]: Adicionado mascara no input de valor de compra`

---

>Pensei em uma forma de melhorar o formato do for, e isso vai deixar a listagem de usuário com um performance melhor

`perf[usuario]: listagem de todos os usuário`<br />
`Com uma reformulação no código que realiza o laço dos usuário foi pensando em um formato melhor de performar o mesmo retirando a comparação do elemento Name`

---
> Por padrão utilizando o [Smart Git](https://www.syntevo.com/smartgit/)
