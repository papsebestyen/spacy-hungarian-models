# Hungarian models for spaCy

This repository contains the building blocks and the releases of Hungarian models for [spaCy](https://spacy.io). 
## Releases

| Date | Model | Version | spaCy | Features | Size | Memory | License | Info |
| --- | --- | --- | --- | ---: | --- | ---: | ---: | --- |
| 2019-01-04 | `hu_core_ud_lg` | `0.1.0` | `>2.0.0,` `<2.1.0` | Word vectors, Brown clusters, Token frequencies, Sentencizer, PoS Tagger, Lemmatizer, Dependency parser | 1.3G | 2.5G | <a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a> | [![][i]][i-hu_core_ud_lg-0.1.0] [![][dl]][hu_core_ud_lg-0.1.0]
| 2019-06-02 | `hu_core_ud_lg` | `0.2.0` | `>=2.1.0,` `<2.2.0` | Word vectors, Brown clusters, Token frequencies, Sentencizer, PoS Tagger, Lemmatizer, Dependency parser | 1.3G | 2.5G | <a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a> | [![][i]][i-hu_core_ud_lg-0.2.0] [![][dl]][hu_core_ud_lg-0.2.0]
| 2019-09-26 | `hu_core_ud_lg` | `0.3.0` | `>=2.1.8,` `<2.2.0` | Word vectors, Brown clusters, Token frequencies, Sentencizer, PoS Tagger, Lemmatizer, Dependency parser, NER | 1.3G | 2.5G | <a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a> | [![][i]][i-hu_core_ud_lg-0.3.0] [![][dl]][hu_core_ud_lg-0.3.0]
| 2019-10-03 | `hu_core_ud_lg` | `0.3.1` | `>=2.2.0,` `<2.3.0` | Word vectors, Brown clusters, Token frequencies, Sentencizer, PoS Tagger, Lemmatizer, Dependency parser, NER | 1.3G | 2.5G | <a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a> | [![][i]][i-hu_core_ud_lg-0.3.1] [![][dl]][hu_core_ud_lg-0.3.1]

[hu_core_ud_lg-0.1.0]: https://github.com/oroszgy/spacy-hungarian-models/releases/download/hu_core_ud_lg-0.1.0/hu_core_ud_lg-0.1.0-py3-none-any.whl
[i-hu_core_ud_lg-0.1.0]: https://github.com/oroszgy/spacy-hungarian-models/releases/hu_core_ud_lg-0.1.0
[hu_core_ud_lg-0.2.0]: https://github.com/oroszgy/spacy-hungarian-models/releases/download/hu_core_ud_lg-0.2.0/hu_core_ud_lg-0.2.0-py3-none-any.whl
[i-hu_core_ud_lg-0.2.0]: https://github.com/oroszgy/spacy-hungarian-models/releases/hu_core_ud_lg-0.2.0
[hu_core_ud_lg-0.3.0]: https://github.com/oroszgy/spacy-hungarian-models/releases/download/hu_core_ud_lg-0.3.0/hu_core_ud_lg-0.3.0-py3-none-any.whl
[i-hu_core_ud_lg-0.3.0]: https://github.com/oroszgy/spacy-hungarian-models/releases/hu_core_ud_lg-0.3.0
[hu_core_ud_lg-0.3.1]: https://github.com/oroszgy/spacy-hungarian-models/releases/download/hu_core_ud_lg-0.3.1/hu_core_ud_lg-0.3.1-py3-none-any.whl
[i-hu_core_ud_lg-0.3.1]: https://github.com/oroszgy/spacy-hungarian-models/releases/hu_core_ud_lg-0.3.1


[dl]: http://i.imgur.com/gQvPgr0.png
[i]: http://i.imgur.com/OpLOcKn.png

## Install

```bash
pip install https://github.com/oroszgy/spacy-hungarian-models/releases/download/hu_core_ud_lg-0.3.1/hu_core_ud_lg-0.3.1-py3-none-any.whl  
```

## Usage

To load a model, `import` the model's package directly and
call its `load()` method with no arguments.

```python
import hu_core_ud_lg

nlp = hu_core_ud_lg.load()
doc = nlp('Csiribiri csiribiri zabszalma - négy csillag közt alszom ma.')
```

For detailed documentation and tutorials, check [spaCy docs](https://spacy.io/usage/processing-pipelines).

## Development

Issuing `make all` fetches all the resources needed and builds a release.

## Changelog

- 2019-10-03 Fixing compatibility issue with spaCy 2.2
- 2019-09-26 Added named entity recognition
- 2019-06-02 Made the pipeline compatible with spaCy 2.1, minor sentence segmentation improvements
- 2019-01-04 UD corpus based core pipeline release for spaCy 2.x
- 2017-06-11 Experimental model releases for spaCy 1.x
