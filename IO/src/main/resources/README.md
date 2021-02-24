this code from https://blog.csdn.net/anxpp/article/details/51512200

BIO: 同步阻塞
    网络连接是同步的 只有返回了结果才会继续往下执行
    读写是阻塞的  需要阻塞式的等待socket流里的数据
    所以服务端需要为每一个客户端开一个线程
NIO: 同步非阻塞
    读写无需等待
    服务端使用一个或有限个线程处理所有客户端连接
AIO: 异步非阻塞
    网络连接是异步的
    读写是非阻塞的