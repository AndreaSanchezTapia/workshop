# 

Quarto: https://quarto.org/docs/get-started/
RStudio: https://posit.co/download/rstudio-desktop/


# Para atualizar a bibliografia

A bibliografia oficial é um documento .bib que vem de uma coleção de Zotero https://www.zotero.org/groups/4991512/climate_resilience_brazil/collections/PSGS5W5W

Para atualizar o arquivo, acrescente a referência à coleção. Exporte a coleção como BibTex e salve como bibliografia.bib.

-   É melhor se só um membro da equipe faz isso.

-   Também é melhor se essa pessoa instalar BetterBibTex e na hora de exportar marcar Keep Updated, para que qualquer modificação à coleção seja refletida imediatamente em vez de exportar manualmente toda vez.

# O estilo de citação

O arquivo .csl é o arquivo com o estilo de citação. Ele vem do [Zotero Style Repository ](https://www.zotero.org/styles) o estilo da revista Ecology foi escolhido e salvo como `citation_style.csl`. 
No arquivo `_quarto.yml`, o campo `csl:` cria o link para esse arquivo. csl: `citation_style.csl`.
