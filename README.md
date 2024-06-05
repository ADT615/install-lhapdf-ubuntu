export PATH=/usr/bin/python3:$PATH

export PATH=/home/cid/for/installation/bin:$PATH

export LD_LIBRARY_PATH=/home/cid/for/installation/lib:$LD_LIBRARY_PATH

export PYTHONPATH=/home/cid/for/installation/local/lib/python3.10/dist-packages:$PYTHONPATH

wget https://lhapdf.hepforge.org/downloads/?f=LHAPDF-6.X.Y.tar.gz -O LHAPDF-6.X.Y.tar.gz

# ^ or use a web browser to download, which will get the filename correct

tar xf LHAPDF-6.X.Y.tar.gz

cd LHAPDF-6.X.Y

./configure --prefix=/path/for/installation

make

make install

lhapdf --version

sudo ln -s /usr/bin/python3 /usr/bin/python
