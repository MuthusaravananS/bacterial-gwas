

# Download and install anaconda(version 3 recommended)

### Add channels

```
conda config --add channels conda-forge\
conda config --add channels bioconda\
conda config --add channels daler\
conda config --add channels defaults\
```

### Download the Analysis pipeline

```
git clone https://github.com/MuthusaravananS/bacterial-gwas.git
```

### Change directory to the dowloaded folder

```
cd bacterial-gwas
```

### Create conda environment.Packages are listed in the environment.yaml file. 

```
conda env create -f environment.yaml
```

### Download the polishing tool pilon

```
mkdir apps\
wget https://github.com/broadinstitute/pilon/releases/download/v1.23/pilon-1.23.jar -O apps/pilon.jar
```

### Activate the analysis environment
```
source activate bacterial-gwas
```

### Add permission to all scripts
```
chmod +x *.{py,sh,pl}
```

### Install python packages using pip
```
pip install -r pip-requirements.txt
```
