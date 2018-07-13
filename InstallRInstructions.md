# How to install R on Binder instance

    %%bash
    V="3.4.2" # R version; tarball must be pres in directory first
              # at https://github.com/alexmill/website_notebooks
    pwd
    ls
    tar zxvf R-$V.tar.gz
    cd R-$V/
    ./configure --enable-R-shlib --with-x=no --prefix=./project/behi
    make
    make check
    sudo make install
    cd ..
    sudo rm -rf R-$V/ build/
    rm R-$V.tar.gz
