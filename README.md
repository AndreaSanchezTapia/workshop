# Para compilar o manual localmente

-   Quarto: https://quarto.org/docs/get-started/
-   RStudio: https://posit.co/download/rstudio-desktop/ (opcional, pode ser qualquer editor de texto)
-   Zotero: https://www.zotero.org/
-   BetterBibTeX for Zotero: https://retorque.re/zotero-better-bibtex/

# A estrutura do livro

O manual é um livro de [Quarto](https://quarto.org/docs/books/).

O arquivo `_quarto.yml` tem a estrutura do livro. Se precisar trocar de ordem, acrescentar seções, essas mudanças devem vir aqui, na seção `chapters:`

Cada capítulo é um arquivo `.qmd` formatado com markdown. [Aqui](https://quarto.org/docs/authoring/markdown-basics.html) está a documentação de markdown para Quarto, mas markdown é amplamente usado.

# Para atualizar a pasta docs/

-   Clone o repositório localmente (só precisa fazer uma vez)
-   No terminal, navegue até a pasta de trabalho: workshop.
-   Atualize o repositório trazendo qualquer mudança recente: `git pull origin main`
-   No terminal, execute `quarto render`. Os arquivos na pasta `docs/` devem ser modificados e precisam ser empurrados para GitHub:
    -   `git add [nome dos arquivos]` ou `git add /docs`
    -   `git commit -m "[mensagem de commit]"`
    -   `git push origin main`

# Para atualizar a bibliografia

A bibliografia oficial é o arquivo `bibliografia.bib` que vem de uma coleção de Zotero [Documento_workshop](https://www.zotero.org/groups/4991512/climate_resilience_brazil/collections/PSGS5W5W) em nosso grupo de Zotero: [URL do grupo](https://www.zotero.org/groups/4991512/climate_resilience_brazil), [Biblioteca](https://www.zotero.org/groups/4991512/climate_resilience_brazil/library)

Para atualizar o arquivo: + acrescente a referência à coleção. + Exporte a coleção como BibTex e sobreescreva `bibliografia.bib` + (Vai ter mudanças no arquivo e o arquivo precisa ser empurrado para GitHub com `git add`, `git commit -m ""`, `git push...`)

-   É melhor se só um membro da equipe faz isso.

-   Também é melhor se essa pessoa instalar [BetterBibTex](https://retorque.re/zotero-better-bibtex/installation/) e na hora de exportar marcar Keep Updated, para que qualquer modificação à coleção seja refletida imediatamente em vez de exportar manualmente toda vez.

# O estilo de citação

O arquivo `citation_style.csl` é o arquivo com o estilo de citação. Ele vem do [Zotero Style Repository](https://www.zotero.org/styles).

Aqui, o estilo da revista Ecology foi escolhido e salvo como `citation_style.csl`.

No arquivo `_quarto.yml`, o campo `csl:` cria o link para esse arquivo. csl: `citation_style.csl`.

Não é necessário modificar isto, só se precisar mudar o estilo de citação.
