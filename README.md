# Digit-Recognition
TAU Ethiopic Digit Recognition 


Link to competition: https://www.kaggle.com/c/tau-ethiopic-digit-recognition/data

# Load data from kaggle in google colab
```
# TODO: create new API token in Kaggle

! pip install -q kaggle
from google.colab import files
files.upload() # Upload token file: kaggle.json

# Add token to VM in google colab
! mkdir ~/.kaggle
! cp kaggle.json ~/.kaggle/
! chmod 600 ~/.kaggle/kaggle.json
! kaggle datasets list

# Old Kaggle API does not support some new features
!pip install --upgrade --force-reinstall --no-deps kaggle

%cd /content/drive/My Drive/Data/afro-mnist/train
!kaggle competitions download -c tau-ethiopic-digit-recognition

# unzip data folder
! unzip tau-ethiopic-digit-recognition.zip -d train

# move images from default folder to desire directory
%cd  /content/drive/My Drive/Data/afro-mnist/train-temp/train/test/
%ls
!mv test /content/drive/My\ Drive/Data/afro-mnist/
```

