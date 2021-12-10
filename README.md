# Tradução de "How to Play Go: A Concise Introduction", por Richard Bozulich e James Davies, da editora Kiseido

> Obrigado ao Richard Bozulich e à editora Kiseido por me permitirem traduzir este livro.

Àqueles que gostariam de construir mais material de Go, sintam-se à vontade para explorar este projeto como modelo, bom ou ruim; e também não hesitem em fazer perguntas!

> **Clique [aqui](https://github.com/FanaroEngineering/traducao_como_jogar_go/releases) para baixar o livro!**

**Links para comprar o livro**:

- [**Amazon**, com distribuição internacional limitada](https://www.amazon.com/dp/B09MZJY8RJ#detailBullets_feature_div)
    - Os países/regiões disponíveis aparentemente: EUA, Reino Unido, Alemanha, França, Espanha, Itália, Japão, Canadá, Austrália.
    - A impressão destes exemplares é feita sob demanda e administrada pela própria Amazon.
- [**Mercado Livre**, administrado por mim, Philippe Fanaro, o autor]()
- [**Amazon.com.br**, administrado por mim, Philippe Fanaro, o autor]()

Seguem algumas amostras abaixo:

<div style="display: inline-flex">
  <img src="Recursos/Screenshot_1%20-%20Capa.png" height="400px" />
  <img src="Recursos/Screenshot_2%20-%20Índice%20Resumido.png" height="400px" />
  <img src="Recursos/Screenshot_2%20-%20Índice%20I.png" height="400px" />
  <img src="Recursos/Screenshot_2%20-%20Índice%20II.png" height="400px" />
  <img src="Recursos/Screenshot_3%20-%202%20-%20As%20Regras.png" height="400px" />
  <img src="Recursos/Screenshot_4%20-%203%20-%20As%20Regras.png" height="400px" />
  <img src="Recursos/Screenshot_5%20-%206%20-%20Estratégia%20de%20Abertura.png" height="400px" />
  <img src="Recursos/Screenshot_6%20-%207%20-%20Táticas%20Elementares.png" height="400px" />
  <img src="Recursos/Screenshot_7%20-%207%20-%20Problemas%2035-38.png" height="400px" />
  <img src="Recursos/Screenshot_8%20-%208%20-%20Vida%20e%20Morte.png" height="400px" />
  <img src="Recursos/Screenshot_9%20-%209%20-%20Go%20com%20Compensação.png" height="400px" />
  <img src="Recursos/Screenshot_10%20-%2011%20-%20Movimentos%20de%20Fim%20de%20Jogo.png" height="400px" />
  <img src="Recursos/Screenshot_11%20-%2012%20-%20Como%20Continuar%20os%20Estudos.png" height="400px" />
  <img src="Recursos/Screenshot_12%20-%20B%20-%20Catálogo%20Kiseido%20em%20Português.png" height="400px" />
  <img src="Recursos/Screenshot_13%20-%20Referências.png" height="400px" />
</div>

<br/>

> Clique [aqui](amazon_kdp_metada.md) para visualizar os metadados utilizados no Amazon Kindle Direct Publishing.

---

**Índice**

<div id="user-content-toc">
  <ul>
    <li><a href="1-links-uteis">1. Links Úteis</a></li>
    <li><a href="2-configuracoes-do-vs-code">2. Configurações do VS Code</a></li>
    <li><a href="3-transpilacao-das-referencias">3. Transpilação das Referências</a></li>
    <li><a href="4-inclusao-de-diagramas-de-go">4. Inclusão de Diagramas de Go</a>
      <ul>
        <li><a href="41-diagramas-com-o-gowrite2">4.1. Diagramas com o GoWrite2</a></li>
        <li><a href="42-diagramas-com-o-pacote-latex-igo">4.2. Diagramas com o Pacote LaTeX <code>igo</code></a></li>
      </ul>
    </li>
  </ul>
</div>

---

## 1. Links Úteis

Primeiramente, seguem os links para o livro original &mdash; por algum motivo não o encontrei listado na [loja online da Kiseido](https://www.kiseidopublishing.com/go_books.htm) &mdash;:

- [How to Play Go no ISBN Search](https://isbnsearch.org/isbn/9784906574391)
- [How to Play Go na Amazon](https://www.amazon.com/How-Play-Go-Concise-Introduction/dp/4906574394)

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
- [DOGemP &mdash; Dojo Online de Go em Português](https://baduk.club/league/dogemp)

## 2. Configurações do VS Code

Juntamente com este repositório, inclui-se algumas configurações do editor VS Code, pois é um editor que todos podem instalar e facilmente utilizar, além de ser um bom quebra-galho caso outros não funcionem &mdash; e uma maneira de padronizar o trabalho no projetinho.

Se você não gosta do VS Code &mdash; eu, particularmente, prefiro Vim &mdash;, sem problemas, é só ignorar a pasta [`.vscode`](./.vscode/).

Se você estiver utilizando VS Code, sugiro instalar a extensão [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop), que automatiza grande parte do que é necessário para projetos em LaTeX. Se vocês estivar utilizando sistemas com Shell disponível, há o script [`build.sh`](./build.sh).

## 3. Transpilação das Referências

Se o software que você estiver utilizando não transpilá-las automaticamente, é possível simplesmente utilizar o comando de terminal:

```sh
bibtex <arquivo-tex-principal>.aux
```

Note que não se utiliza o nome do arquivo `.bib`. Para mais informações, veja [esta resposta](https://tex.stackexchange.com/a/353433/64441).

## 4. Inclusão de Diagramas de Go

### 4.1. Diagramas com o GoWrite2

O [GoWrite2](https://gowrite.net/GOWrite2.html) é aparentemente o software predileto dos escritores de livros de Go, visto que é mais visual e integrado aos arquivos SGFs.

Primariamante, foi criado para exportar PDFs diretamente, fabricando-os a partir dos diagramas e comentários, mas há também a opção de utilizá-lo para exportar imagens vetoriais (EPS ou SVG) e inclui-las no livro LaTeX, sem pixelação. Todos essas facilidades fazem com o GoWrite2 seja o software fabricação de diagramas utilizado neste projeto.

### 4.2. Diagramas com o Pacote LaTeX `igo`

> Por algum motivo, o pacote `igo` não parece mais diagramar tabuleiros e pedras sem distorções, o que inviabiliza seu uso neste projeto.

Para instalar o pacote [`igo`](https://www.ctan.org/pkg/igo) manualmente, baixe-o e depois extraia todos os arquivos para o mesmo nível do arquivo principal. Também será preciso extrair todas as fontes para o nível principal &mdash; caso ainda haja dificuldades, veja [esta pergunta](https://tex.stackexchange.com/q/615371/64441) no TeX StackExchange. Esse arquivos não poluirão o projeto nem o editor, dado que o [`.gitignore`](./.gitignore) já foi configurado &mdash; e o VS Code também, pelo menos.

Uma vez instalado, é só seguir a documentação, dentro da pasta [`Documentacao/`](./Documentacao).

Caso você esteja utilizando a distribuição MiKTeX, nem sequer é preciso instalar o `igo`, ele já está incluído.

Há também o pacote [`psgo`](https://www.ctan.org/pkg/psgo), mas é bem mais complicado e de difícil compilação.