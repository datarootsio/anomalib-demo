# Anomalib demo on IDRiD dataset

To run the notebook do

```
git clone git@github.com:toon-vc/anomalib-demo.git
poetry install
poetry run jupyter notebook
```

and make sure the 'B. Disease Grading.zip' from the [IDRiD dataset](https://ieee-dataport.org/open-access/indian-diabetic-retinopathy-image-dataset-idrid) is in the data folder.

##### Note on running anomalib with only normal data

Anomalib requires a set of abnormal images for each model training, which it uses for threshold tuning and evaluation (see this [github issue](https://github.com/openvinotoolkit/anomalib/issues/686)). They are working on allowing trainings without any abnormal images, in the meantime I have applied a temporary change in [this fork](https://github.com/toon-vc/anomalib) which skips reading the abnormal images dir after which everything works as expected and models can be trained with only normal ones. 