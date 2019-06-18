# ImportKaggleData
How we import kaggle dataset directly to our colab or any notebooks

Easy Steps to persist Kaggle profile

Download kaggle.json from Kaggle -- MyAccount -- Create New API Token - auto downloads as "kaggle.json

Import json into notebook - run in a cell 
from google.colab import files
files.upload()

Browse to downloaded kaggle.json and upload
Setup Kaggle DIR; copy json file ; chmod
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
!ls ~/.kaggle

Verify json content
!ls -l ~/.kaggle
!cat ~/.kaggle/kaggle.json

Install kaggle packages
!pip install -q kaggle
!pip install -q kaggle-cli

List Kaggle DataSets
!kaggle datasets list
