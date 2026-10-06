<!-- ELUCENIA technical documentation · sistema-de-bethesda-tireoide · pt-BR · no clinical/professional/rights approval -->

# Sistema de Bethesda para citologia de tireoide

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/sistema-de-bethesda-tireoide)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Categoria do laudo

`cat`

- `1` — I · Não diagnóstica
- `2` — II · Benigna
- `3` — III · Atipia de significado indeterminado (AUS)
- `4` — IV · Neoplasia folicular
- `5` — V · Suspeita de malignidade
- `6` — VI · Maligna

## Edição do método

Bethesda tireoide 2023, 3ª edição: 6 categorias, ROM e AUS nuclear/outras; verificação documental limitada ao código da categoria selecionada

## Fórmula documentada

Seis categorias diagnósticas, cada uma com um risco de malignidade (ROM) médio e uma faixa esperada, atualizados na 3ª edição (2023), que passou a usar um nome único por categoria e dividiu a AUS em dois subgrupos (atipia nuclear e outras).

## Limites e população

A categoria Bethesda deve vir de laudo citopatológico de PAAF de tireoide, não ser atribuída pela calculadora. Risco médio e intervalo são estimativas da edição, não diagnóstico individual. A edição 2023 discute riscos e manejo pediátricos próprios; valores adultos não devem ser extrapolados automaticamente a crianças. Nesta verificação, o acesso direto ao artigo de 2023 forneceu apenas o resumo editorial; a tabela de ROM foi consultada em uma reprodução de terceiros do artigo original, com imagem de baixa resolução. A Tabela 2 reproduzida indica AUS com faixa de 13–30%, enquanto o texto do mesmo artigo indica 20–32%. Essas faixas não foram adjudicadas. O teste verifica somente o código da categoria selecionada; ROM adulto, ROM pediátrico e manejo não foram validados nesta verificação.

## Referências

- [Ali SZ et al. The 2023 Bethesda System for Reporting Thyroid Cytopathology. Thyroid, 2023.](https://doi.org/10.1089/thy.2023.0141)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Benigna: risco médio de malignidade de 4%

| Detalhes do resultado | |
| --- | --- |
| Faixa esperada de risco | 2 a 7% |
| Conduta usual (adultos) | Seguimento clínico e ultrassonográfico |


### 2

Atipia de significado indeterminado (AUS): risco médio de malignidade de 22%

| Detalhes do resultado | |
| --- | --- |
| Faixa esperada de risco | 13 a 30% |
| Conduta usual (adultos) | Repetir a PAAF, teste molecular, lobectomia diagnóstica ou vigilância |


### 3

Suspeita de malignidade: risco médio de malignidade de 74%

| Detalhes do resultado | |
| --- | --- |
| Faixa esperada de risco | 67 a 83% |
| Conduta usual (adultos) | Teste molecular, lobectomia ou tireoidectomia quase total |


### 4

Não diagnóstica: risco médio de malignidade de 13%

| Detalhes do resultado | |
| --- | --- |
| Faixa esperada de risco | 5 a 20% |
| Conduta usual (adultos) | Repetir a PAAF guiada por ultrassom |

