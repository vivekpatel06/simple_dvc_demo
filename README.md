copy Repo

```bash 
git clone https://github.com/vivekpatel06/simple_dvc_demo.git

```
create env

```bash
conda create -n wineq python=3.7 -y
```

activate env
```bash
conda activate wineq
```

created a req file

install the req
```bash
pip install -r requirements.txt
```
download the data from 

https://drive.google.com/drive/folders/18zqQiCJVgF7uzXgfbIJ-04zgz1ItNfF5?usp=sharing

paste downloaded data into : "simple-dvc-demo-main>>data_given"

```bash
git init
```
```bash
dvc init 
```
```bash
dvc add data_given/winequality.csv
```
```bash
git add .
```
```bash
git commit -m "first commit"
```

oneliner updates  for readme

```bash
git add . && git commit -m "update Readme.md"
```
```bash
git remote add origin https://github.com/<githubID>/<RepoName>.git
git branch -M main
git push origin main
```
```bash
python src/load_data.py
```
```bash
dvc repro
```
whenever making new changes run following 2 command
``` bash
git add . && git commit -m "your comment"
git push origin main```