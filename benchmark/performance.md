OpenSSL的开发者已经在openssl中内置了一个基准测试.通过speed参数可以进行基准测试.基准测试是衡量在给定时间内能执行多少次操作而非给定操作看需要多长时间.你会发现即使在性能差的机器上执行的时间也比性能好的机器慢不了多少.

不带任何参数,会进行全面的基准测试

    openssl speed

你也可以执行特定的算法

    # test rsa speeds
    openssl speed rsa

    # do the same test on a two-way SMP system
    openssl speed rsa -multi 2


