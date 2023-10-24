# align_and_parse
Get transcript from speech wav file.
Then get textgrid from transcript and speech wav file.

## Installation
```
conda install montreal-forced-aligner
mfa model download acoustic english_us_arpa
mfa model download dictionary english_us_arpa

```


## Get transcript
I created another repo for this:
https://github.com/Sigurd-git/Speech-to-text.git
You can get transcript from speech wav file following instructions this repo.

## Align

Place transcript in the same folder as the wav file, and rename it to the same name as the wav file, except with a .lab extension.
Then run:
```
mfa align <Path_to_your_input_folder> english_us_arpa english_us_arpa <Path_to_your_output_folder>  --clean 
```

For example:
```
mfa align test english_us_arpa english_us_arpa output  --clean 
```

Meaning of the arguments:
First english_us_arpa: the name of the dictionary that was used.
Second english_us_arpa : the name of the acoustic_model 
