source link: [stackoverflow](https://stackoverflow.com/a/868664)

CPU Bound means the rate at which process progresses is limited by the speed of the CPU. A task that performs calculations on a small set of numbers, for example multiplying small matrices, is likely to be CPU bound.

I/O Bound means the rate at which a process progresses is limited by the speed of the I/O subsystem. A task that processes data from disk, for example, counting the number of lines in a file is likely to be I/O bound.

Memory bound means the rate at which a process progresses is limited by the amount memory available and the speed of that memory access. A task that processes large amounts of in memory data, for example multiplying large matrices, is likely to be Memory Bound.

Cache bound means the rate at which a process progress is limited by the amount and speed of the cache available. A task that simply processes more data than fits in the cache will be cache bound.

I/O Bound would be slower than Memory Bound would be slower than Cache Bound would be slower than CPU Bound.

The solution to being I/O bound isn't necessarily to get more Memory. In some situations, the access algorithm could be designed around the I/O, Memory or Cache limitations. See [Cache Oblivious Algorithms](http://en.wikipedia.org/wiki/Cache-oblivious_algorithm).
