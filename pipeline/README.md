# Run the pipeline on e.g. Jetstream

The below instructions should work on Ubuntu 16.04.

Start by booting a computer on Jetstream (loose instructions
[here](https://2017-ucsc-metagenomics.readthedocs.io/en/latest/jetstream/boot.html).
You'll want to use an m1.small machine or larger.

Then execute the below commands at the shell.

## Install software dependencies

Install the prerequisites:

```
sudo apt-get -y update && \
    sudo apt-get -y install bioperl libxml-simple-perl default-jre git curl
```

## Install Prokka

```
# get the latest version from github
git clone https://github.com/tseemann/prokka.git

# add it to the environment
echo 'export PATH=$PWD/prokka/bin:$PATH' >> ~/.bashrc
source ~/.bashrc

# run the things
prokka --setupdb
prokka --version
```

## Run the pipeline

```
# clone github repo into our home directory
cd ~/
git clone http://github.com/dib-lab/2017-ectocooler.git

# run the makefile
cd 2017-ectocooler/pipeline
make
```
