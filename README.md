Other dataset file can be downloaded here: [https://pub-92469f2f323c4070b545a1b6a4072028.r2.dev/datas.zip](https://pub-92469f2f323c4070b545a1b6a4072028.r2.dev/datas.zip) .

Refer to the scripts below to download and unzip the folder:

```
python - <<'PY'
import os
import urllib.request
import zipfile

url = "https://pub-92469f2f323c4070b545a1b6a4072028.r2.dev/datas.zip"
zip_path = "datas.zip"

print("Downloading dataset...")
urllib.request.urlretrieve(url, zip_path)

print("Extracting...")
with zipfile.ZipFile(zip_path, "r") as z:
    z.extractall(".")

print("Done. Dataset extracted to current directory.")
PY
```
