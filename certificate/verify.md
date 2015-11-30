使用verify参数可以验证证书

    openssl verify cert.pem

如果OpenSSL识别这个证书或其签发主体、日期、算法等，就会输出OK

    $ openssl verify remote.site.pem
    remote.site.pem: OK

如果有任何错误，就会输出简单的错误信息

  * error 10 at 0 depth lookup:certificate has expired. 证书通常是有有效期的,比如1年.超过有效期,验证会出错

  * error 18 at 0 depth lookup:self signed certificate. OpenSSL不能验证自签名的证书
