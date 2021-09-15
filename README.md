# Tradução de "How to Play Go: A Concise Introduction", por Richard Bozulich e James Davies

> Obrigado ao Richard Bozulich por me permitir traduzir este livro.

## Links

No livro, são citados links para recursos muito úteis para quem está começando. Para facilitar a referência, aqui estão eles &mdash; não se esqueça de utilizar a página de [issues](https://github.com/FanaroEngineering/traducao_como_jogar_go) para sugestões de adições &mdash;:

- [OGS](https://online-go.com)
- [KGS](https://www.gokgs.com)
- [Go Books para iOS](https://apps.apple.com/us/app/go-books/id428149193)
- [SmartGo, aplicativo para iOS](https://apps.apple.com/us/app/smartgo-player/id314506629)
- [Go Write 2](https://www.gowrite.net/GOWrite2_download.html)
- [Editora Kiseido](https://www.kiseido.com)
- [fanaro.io](https://fanaro.io)
- [Canal de YouTube do Philippe Fanaro](https://youtube.com/c/PhilippeFanaro)
- [Canal de Twitch do Philippe Fanaro](https://twitch.tv/fanaro009)

## Configurações do VS Code

Juntamente com este repositório, inclui-se algumas configurações do editor VS Code, pois é um editor que todos podem instalar e facilmente utilizar, além de ser um bom quebra-galho caso outros não funcionem &mdash; e uma maneira de padronizar o trabalho no projetinho.

Se você não gosta do VS Code &mdash; eu, particularmente, prefiro Vim &mdash;, sem problemas, é só ignorar a pasta [`.vscode`](./.vscode/).

Se você estiver utilizando VS Code, sugiro instalar a extensão [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop), que automatiza grande parte do que é necessário para projetos em LaTeX. Se vocês estivar utilizando sistemas com Shell disponível, há o script [`build.sh`](./build.sh).

## Transpilação das Referências

Se o software que você estiver utilizando não transpilá-las automaticamente, é possível simplesmente utilizar o comando de terminal:

```sh
bibtex <arquivo-tex-principal>.aux
```

Note que não se utiliza o nome do arquivo `.bib`. Para mais informações, veja [esta resposta](https://tex.stackexchange.com/a/353433/64441).

## Inclusão de Diagramas de Go

### Diagramas com o Pacote LaTeX `igo`

Para instalar o pacote [`igo`](https://www.ctan.org/pkg/igo) manualmente, baixe-o e depois extraia todos os arquivos para o mesmo nível do arquivo principal. Também será preciso extrair todas as fontes para o nível principal &mdash; caso ainda haja dificuldades, veja [esta pergunta](https://tex.stackexchange.com/q/615371/64441) no TeX StackExchange. Esse arquivos não poluirão o projeto nem o editor, dado que o [`.gitignore`](./.gitignore) já foi configurado &mdash; e o VS Code também, pelo menos.

Uma vez instalado, é só seguir a documentação, dentro da pasta [`Documentacao/`](./Documentacao).

Caso você esteja utilizando a distribuição MiKTeX, nem sequer é preciso instalar o `igo`, ele já está incluído.

Há também o pacote [`psgo`](https://www.ctan.org/pkg/psgo), mas é bem mais complicado e de difícil compilação.

### Diagramas com o Go Write 2

O [GoWrite2](https://gowrite.net/GOWrite2.html) é aparentemente o software predileto dos escritores de livros de Go, visto que é mais visual e integrado aos arquivos SGFs. Porém, até onde sei, seus diagramas são exportados em PNGs, ou seja, haverá pixelação, inevitavelmente.