This model, data, and code are for the paper "Применение ансамблевого обучения для прогнозирования субклеточной локализации мРНК: комплексное сравнительное исследование"

Don't forget download files from lfs:
git lfs pull

Import conda enviroment:
conda env create -f mCat50.yml

Activate conda enviroment:
conda activate mCat50

Extract features and predict on test set:
python3 mCat50.py data/test.fasta predictions/testPred.csv



Or predict on test set if features already extracted:
python3 mCat50.py FExt/features/test.npy predictions/testPred.csv

In this example predictions will be saved in predictions/testPred.csv
You can view It in check_mCat50_predictions.ipynb or open with LibreOffice Calc or Excel

For check software and debugging small data/testExample.fasta can be used
python3 mCat50.py data/testExample.fasta predictions/testExamplePred.csv

For help enter:
python3 mCat50.py -h

Class labels:
{'Cytoplasm': 0,
 'Endoplasmic reticulum': 1,
 'Extracellular region': 2,
 'Mitochondria': 3,
 'Nucleus': 4}
