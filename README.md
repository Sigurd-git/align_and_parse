# align_and_parse
Get text from speech

## Installation
```
conda install montreal-forced-aligner
mfa model download acoustic english_us_arpa
mfa model download dictionary english_us_arpa

```

## Validation
```
mfa validate ./test english_us_arpa english_us_arpa #corpus dictionary acoustic_model --clean
```

## Align
```
mfa align test english_us_arpa english_us_arpa output #corpus dictionary acoustic_model output_dir --clean
```
