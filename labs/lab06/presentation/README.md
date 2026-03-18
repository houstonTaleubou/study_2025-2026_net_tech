# Apresentação - Laboratório 06

Esta pasta contém as imagens para a apresentação do laboratório 06.

## Imagens disponíveis:
- 10.png
- 11.png
- 12.png
- 13.png
- 14.png
- 15.png
- 16.png
- 17.png
- 18.png
- 19.png
- 1.png
- 2.png
- 3.png
- 4.png
- 5.png
- 6.png
- 7.png
- 8.png
- 9.png

## Total de imagens: 19

## Como gerar os slides:
Para gerar os slides em PDF, PPTX e HTML, use os seguintes comandos:

```bash
cd labs/lab06/presentation

# Gerar PDF
pandoc ../lab06.md -o slides.pdf --pdf-engine=xelatex -V mainfont="DejaVu Sans"

# Gerar PowerPoint
pandoc ../lab06.md -o slides.pptx

# Gerar HTML
pandoc ../lab06.md -o slides.html --self-contained
```

## Observação:
As imagens estão numeradas sequencialmente (1.png, 2.png, etc.) e devem ser referenciadas no arquivo ../lab06.md como `image/X.png`.
