# How to install R on Binder instance

    %%bash
    # R version; tarball must be pres in directory first
    # at https://github.com/alexmill/website_notebooks
    tar zxvf R-3.4.2.tar.gz
    cd R-3.4.2/
    ./configure --enable-R-shlib --with-x=no --prefix=./R_pkgs/
    make
    make check
    sudo make install
    cd ~
