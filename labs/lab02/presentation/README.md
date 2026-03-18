# Apresentação - Laboratório 02

Esta pasta contém as imagens para a apresentação do laboratório 02.

## Imagens disponíveis:
- 1.png
- 2.png
- 3.png
- 4.png
- 5.png
- 6.png

## Total de imagens: 6

## Como gerar os slides:
Para gerar os slides em PDF, PPTX e HTML, use os seguintes comandos:

```bash
cd labs/lab02/presentation

# Gerar PDF
pandoc ../lab02.md -o slides.pdf --pdf-engine=xelatex -V mainfont="DejaVu Sans"

# Gerar PowerPoint
pandoc ../lab02.md -o slides.pptx

# Gerar HTML
pandoc ../lab02.md -o slides.html --self-contained
```

## Observação:
As imagens estão numeradas sequencialmente (1.png, 2.png, etc.) e devem ser referenciadas no arquivo ../lab02.md como `image/X.png`.
