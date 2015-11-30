使用genrsa参数


    # default 1024-bit key, sent to standard output
    openssl genrsa

    # 2048-bit key, saved to file named mykey.pem
    openssl genrsa -out mykey.pem 2048

    # same as above, but encrypted with a passphrase
    openssl genrsa -des3 -out mykey.pem 2048
