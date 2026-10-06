<!-- ELUCENIA technical documentation · sistema-de-bethesda-tireoide · it · no clinical/professional/rights approval -->

# Sistema Bethesda per la citologia tiroidea

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/sistema-de-bethesda-tireoide)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Categoria del referto

`cat`

- `1` — I · Non diagnostica
- `2` — II · Benigna
- `3` — III · Atipia di significato indeterminato (AUS)
- `4` — IV · Neoplasia follicolare
- `5` — V · Sospetta malignità
- `6` — VI · Maligna

## Edizione del metodo

Bethesda tiroide 2023, 3ª edizione: 6 categorie, ROM e AUS nucleare/altre; verifica documentale limitata al codice della categoria selezionata

## Formula documentata

Sei categorie diagnostiche con ROM medio e intervallo atteso, terza edizione 2023: nome unico per categoria, AUS in atipia nucleare e altre.

## Limiti e popolazione

La categoria Bethesda deve provenire da un referto citopatologico di agoaspirato tiroideo, non essere assegnata dal calcolatore. Rischio medio e intervallo sono stime dell’edizione, non una diagnosi individuale. L’edizione 2023 tratta rischi e gestione pediatrici specifici; i valori per adulti non devono essere estrapolati automaticamente ai bambini. In questa verifica, l’accesso diretto all’articolo del 2023 ha fornito soltanto l’abstract editoriale; la tabella del ROM è stata consultata in una riproduzione di terzi dell’articolo originale, con un’immagine a bassa risoluzione. La Tabella 2 riprodotta indica per AUS un intervallo del 13–30%, mentre il testo dello stesso articolo indica il 20–32%. Questi intervalli non sono stati risolti mediante una valutazione conclusiva. Il test verifica soltanto il codice della categoria selezionata; il ROM adulto, il ROM pediatrico e la gestione non sono stati validati in questa verifica.

## Riferimenti

- [Ali SZ et al. The 2023 Bethesda System for Reporting Thyroid Cytopathology. Thyroid, 2023.](https://doi.org/10.1089/thy.2023.0141)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Benigno: rischio medio di malignità di 4%

| Dettagli del risultato | |
| --- | --- |
| Intervallo di rischio atteso | 2 a 7% |
| Condotta abituale (adulti) | Follow-up clinico ed ecografico |


### 2

Atypia di significato indeterminato (AUS): rischio medio di malignità di 22%

| Dettagli del risultato | |
| --- | --- |
| Intervallo di rischio atteso | 13 a 30% |
| Condotta abituale (adulti) | Ripetere la FNA, test molecolare, lobectomia diagnostica o sorveglianza |


### 3

Sospetto di malignità: rischio medio di malignità di 74%

| Dettagli del risultato | |
| --- | --- |
| Intervallo di rischio atteso | 67 a 83% |
| Condotta abituale (adulti) | Test molecolare, lobectomia o tiroidectomia quasi totale |


### 4

Non diagnostico: rischio medio di malignità di 13%

| Dettagli del risultato | |
| --- | --- |
| Intervallo di rischio atteso | 5 a 20% |
| Condotta abituale (adulti) | Ripetere la FNA guidata da ecografia |

