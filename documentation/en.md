<!-- ELUCENIA technical documentation · sistema-de-bethesda-tireoide · en · no clinical/professional/rights approval -->

# Bethesda System for thyroid cytopathology

[conditions, sources and permissions](https://elucenia.org/en/tools/sistema-de-bethesda-tireoide)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Report category

`cat`

- `1` — I · Nondiagnostic
- `2` — II · Benign
- `3` — III · Atypia of undetermined significance (AUS)
- `4` — IV · Follicular neoplasm
- `5` — V · Suspicious for malignancy
- `6` — VI · Malignant

## Method edition

Bethesda thyroid 2023, 3rd edition: 6 categories, ROM and nuclear/other AUS; documentary verification limited to the selected category code

## Documented formula

Six diagnostic categories, each with mean malignancy risk (ROM) and expected range, updated in third edition 2023: one name per category and AUS split into nuclear atypia and other atypia.

## Limits and population

The Bethesda category must come from a thyroid FNA cytopathology report, not be assigned by the calculator. Mean risk and range are edition estimates, not an individual diagnosis. The 2023 edition discusses specific pediatric risks and management; adult values must not be automatically extrapolated to children. In this review, direct access to the 2023 article provided only the publisher abstract; the ROM table was consulted in a third-party reproduction of the original article with a low-resolution image. The reproduced Table 2 gives an AUS range of 13–30%, whereas the body of the same article gives 20–32%. These ranges were not adjudicated. The test checks only the selected category code; adult ROM, pediatric ROM and management were not validated in this review.

## References

- [Ali SZ et al. The 2023 Bethesda System for Reporting Thyroid Cytopathology. Thyroid, 2023.](https://doi.org/10.1089/thy.2023.0141)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Benign: average risk of malignancy of 4%

| Result details | |
| --- | --- |
| Expected risk range | 2 to 7% |
| Usual management (adults) | Clinical and ultrasound follow-up |


### 2

Atypia of undetermined significance (AUS): average risk of malignancy of 22%

| Result details | |
| --- | --- |
| Expected risk range | 13 to 30% |
| Usual management (adults) | Repeat FNA, molecular testing, diagnostic lobectomy or surveillance |


### 3

Suspicious for malignancy: average risk of malignancy of 74%

| Result details | |
| --- | --- |
| Expected risk range | 67 to 83% |
| Usual management (adults) | Molecular testing, lobectomy or near-total thyroidectomy |


### 4

Non-diagnostic: average risk of malignancy of 13%

| Result details | |
| --- | --- |
| Expected risk range | 5 to 20% |
| Usual management (adults) | Repeat ultrasound-guided FNA |

