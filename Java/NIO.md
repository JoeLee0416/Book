# NIO

## NIO简介
NIO是一种同步非阻塞的I/O模型，即Non-blocking IO。提供了Channel、Selector、Buffer等抽象。  
NIO提供了SocketChannel和ServerSocketChannel两种不同的套接字通道实现，都支持阻塞和非阻塞两种模式。

## Buffer
Buffer(缓冲区)是一个对象，它用来暂时的存储写入或者读取的数据。而在BIO中，数据写出或者读取是读取到stream对象中。
在NIO库中，所有数据都是用缓冲区处理。最长同的缓冲区ByteBuffer。

## Channel
Channel(通道)，NIO通过其进行读写。通道是双向的，而流的读写时单向的。

## Selector
Selector（选择器），用于使用单个线程处理多个通道。Selector其实就像时一个容器,管理着多个channel，避免了上下文切换带来的开销。