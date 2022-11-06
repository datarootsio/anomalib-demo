# Anomalib demo

Applying PatchCore from the anomalib library to the IDRiD dataset.
PatchCore was evaluated in the paper on an industrial benchmark, it seemed cool to see how well it performs also outside that setting.
IDRiD contains retinal images of subjects with varying degrees of diabetic retinopathy (DR).

For now, very quickly trained one PatchCore model (no parameter tuning at all), seems to be able to identify at least large exudates due to DR. 

This notebook is first run-through of training model and getting a prediction, many things to improve.

Some notes
    - trained on IDRiD dataset (https://ieee-dataport.org/open-access/indian-diabetic-retinopathy-image-dataset-idrid), code to separate normal and abnormal images still to be added
    - need to do a small change to anomalib in anomalib/data/folder.py, commented parsing of abnormal images as I want to train model without giving any abnormal images at all 



