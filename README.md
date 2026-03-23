medical_data_url="https://raw.githubusercontent.com/ariseegoistx69-cyber/jarvis/refs/heads/main/medical%20datas.csv"
from urllib.request import urlretrieve
urlretrieve(medical_data_url,"empty_csv.csv")
import pandas as pd
medical_df = pd.read_csv("empty_csv.csv")
medical_df 
medical_df.info()
medical_df.describe()
!pip install jovian --upgrade --quiet
import jovian
jovian.commit()
