# danish-ast

Assumes NST training dataset is unpacked under `/data/nst/train` and NST test under `/data/nst/da_0611_test`.

Use the notebooks `extract_annotations.ipynb` and `parse_to_csv.ipynb` to create csv files for training (requires `sqltables` python package).

Training needs to have `speechbrain` and `transformers` packages installed.

To train a speechbrain pipeline based on the CommonVoice recipe, cd into `NST/ASR/seq2seq/` and run
```
python train_with_wav2vec.py hparams/train_da_with_wav2vec.yaml --device cpu
```
