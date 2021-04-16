# calamari_models
Pretrained mixed models to be used with Calamari.

## Short description of the available models
- *gt4histocr* was trained on the entire [GT4HistOCR corpus](https://zenodo.org/record/1344132#.X2xLTlVfiV4)
- *antiqua/fraktur_historical* used the corresponding data from the GT4HistOCR corpus
- The *ligs* versions used the same data as the standard *antiqua/fraktur_historical* models but were refined on an manually enriched subset (afair 100 lines per book) containing ligatures etc.
- *fraktur19* is based on the DTA19 sub set of the GT4HistOCR corpus; and other Fraktur19 data; see [here](https://github.com/Calamari-OCR/calamari_models/issues/3#issuecomment-609730690) for further details
- *uw3-modern-english* (formerly *antiqua_modern*) was trained on the [UW3 dataset](http://www.tmbdev.net/ocrdata-split/) (link seems to be down)
- *idiotikon* originated from a cooperation with [Schweizerisches Idiotikon](https://www.idiotikon.ch/) in an effort to OCR the entire dictionary. The model is based on the UW3 model and its codec contains a wide variety of mostly Latin-based characters including many diacritics. Consequently, it may be a good choice to recognize many modern languages.
- *18th_century_french* was trained in cooperation with the [MiMoText](https://www.mimotext.uni-trier.de/en) project of the University of Trier. It is based on double-keyed transcriptions of french novels published between 1750 and 1800. 
- *historical_french* used data from 17/18/19. century French printings collected by [Simon Gabay](https://www.unine.ch/ilf/home/equipe-enseignante/gabay_simon.html)

## General comments
- All models are provided as a voting ensemble trained via *calamari-cross-fold-train* and containing five individual voters.
- Most models have been trained (exclusively) on the output of the [OCRopus](https://github.com/ocropus/ocropy) *nlbin* script (gt4histocr used grayscale images, the rest binary ones) and will consequently work best on similar data.
- All models have been trained using NFC normalization except the *idiotikon* one (NFD).


## Future work
We are planning to considerably increase the number of available models in the somewhat near future (probably starting from mid october), including more time-specific models and spezialized or at least more robust models regarding different binarization techniques.
Furthermore, a student work (hopefully) will deal with the task of training various models for modern scripts and languages using (mainly) synthetic data.

If you want to contribute your own models or have any questions / model requests please don't hesitate to contact us.
