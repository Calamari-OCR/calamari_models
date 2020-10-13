# calamari_models
Pretrained mixed models to be used with Calamari.

## Short description of the available models
- *antiqua_modern* was trained on the [UW3 dataset](http://www.tmbdev.net/ocrdata-split/) (link seems to be down)
- *antiqua/fraktur_historical* used the corresponding data from the [GT4HistOCR corpus](https://zenodo.org/record/1344132#.X2xLTlVfiV4)
- the *ligs* versions used the same data as the standard *antiqua/fraktur_historical* models but were refined on an manually enriched subset (afair 100 lines per book) containing ligatures etc.
- *fraktur19* is based on the DTA19 sub set of the GT4HistOCR corpus; see [here](https://github.com/Calamari-OCR/calamari_models/issues/3#issuecomment-609730690) for further details

## Future work
We are planning to considerably increase the number of available models in the somewhat near future (probably starting from mid october), including more time-specific models (maybe 16/17/18th century) and spezialized or at least more robust models regarding binarization techniques.
Furthermore, a student work will deal with the task of training various models for modern scripts and languages using (mainly) synthetic data.

If you want to contribute your own models please don't hesitate to contact us.
