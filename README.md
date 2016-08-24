# Word Count in Java

## Problem statement
Count word frequency for words in a XML Wiki dump

## Solution and optimization
* Initial implement with a single thread
* Separate producer and consumer thread with Blocking Queue
* Introduce more consumers with Executor Service
* Reduce resource competition with ConcurrentHashMap instead of lock-based synchronized hashmap
* Batch updates to global concurrentHashMap with local hashmaps

Enjoy the mindmap on [word count design](https://www.mindmeister.com/739648447)
