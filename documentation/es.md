<!-- ELUCENIA technical documentation · sistema-de-bethesda-tireoide · es · no clinical/professional/rights approval -->

# Sistema Bethesda para citología tiroidea

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/sistema-de-bethesda-tireoide)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Categoría del informe

`cat`

- `1` — I · No diagnóstica
- `2` — II · Benigna
- `3` — III · Atipia de significado indeterminado (AUS)
- `4` — IV · Neoplasia folicular
- `5` — V · Sospechosa de malignidad
- `6` — VI · Maligna

## Edición del método

Bethesda tiroides 2023, 3.ª edición: 6 categorías, ROM y AUS nuclear/otras; verificación documental limitada al código de la categoría seleccionada

## Fórmula documentada

Seis categorías diagnósticas con riesgo maligno (ROM) medio y rango esperado, tercera edición 2023: nombre único por categoría y AUS en atipia nuclear y otras.

## Límites y población

La categoría Bethesda debe proceder de un informe citopatológico de PAAF de tiroides, no ser asignada por la calculadora. El riesgo medio y el intervalo son estimaciones de la edición, no un diagnóstico individual. La edición 2023 aborda riesgos y manejo pediátricos propios; los valores de adultos no deben extrapolarse automáticamente a niños. En esta verificación, el acceso directo al artículo de 2023 proporcionó únicamente el resumen editorial; la tabla de ROM se consultó en una reproducción de terceros del artículo original, con una imagen de baja resolución. La Tabla 2 reproducida indica un intervalo de AUS del 13–30%, mientras que el texto del mismo artículo indica el 20–32%. No se resolvió la discrepancia entre estos intervalos. La prueba verifica únicamente el código de la categoría seleccionada; el ROM adulto, el ROM pediátrico y el manejo no se validaron en esta verificación.

## Referencias

- [Ali SZ et al. The 2023 Bethesda System for Reporting Thyroid Cytopathology. Thyroid, 2023.](https://doi.org/10.1089/thy.2023.0141)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Benigna: riesgo medio de malignidad de 4%

| Detalles del resultado | |
| --- | --- |
| Intervalo de riesgo esperado | 2 a 7% |
| Conducta habitual (adultos) | Seguimiento clínico y ecográfico |


### 2

Atipia de significado indeterminado (AUS): riesgo medio de malignidad de 22%

| Detalles del resultado | |
| --- | --- |
| Intervalo de riesgo esperado | 13 a 30% |
| Conducta habitual (adultos) | Repetir la PAAF, prueba molecular, lobectomía diagnóstica o vigilancia |


### 3

Sospecha de malignidad: riesgo medio de malignidad de 74%

| Detalles del resultado | |
| --- | --- |
| Intervalo de riesgo esperado | 67 a 83% |
| Conducta habitual (adultos) | Prueba molecular, lobectomía o tiroidectomía casi total |


### 4

No diagnóstica: riesgo medio de malignidad de 13%

| Detalles del resultado | |
| --- | --- |
| Intervalo de riesgo esperado | 5 a 20% |
| Conducta habitual (adultos) | Repetir la PAAF guiada por ecografía |

