# Installation

[Installation](https://redis.io/download)

You can refer to the url before and meanwhile `make`, `make-guile` and `gcc` is need using the following command:

    sudo apt install make
    sudo apt install make-guile
    sudo apt install gcc
    
At last, replace the command `make` by

    make MALLOC=libc
