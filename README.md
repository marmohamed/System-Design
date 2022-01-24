# System-Design

##### This post is still under development.
------
I am trying here to share my knowledge as this should sharpen my skills and show how far I can go in system design. It is also a way to share any recommended resources with my team and friends.

## System Expert Solutions:
I willl post [here](system-expert-solutions) my solutions of system expert questions.

They have their own solutions. However, I will post my own solutions which can be a little bit different from theirs.

## My recommendations:

1. [System Expert](https://www.algoexpert.io/systems/product)
2. [towardsdatascience articles](https://towardsdatascience.com/system-design-101-b8f15162ef7c)
3. [Hussein Nasser's Youtube Channel](https://www.youtube.com/channel/UC_ML5xP23TOWKUcc-oAE_Eg)
4. [igotanoffer blog articles](https://igotanoffer.com/blogs/tech/network-protocols-proxies-system-design-interview)

## Books:
1. [Designing Data-Intensive Applications](https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321)

### Design examples:
1. [task scheduling](https://dropbox.tech/infrastructure/asynchronous-task-scheduling-at-dropbox)

### Main Topics:
* Load balancing

    - Techniques:

        1. Round-Ropin
        2. Random
        3. 

* Proxy

    - Forward Proxy
    - Reverse Proxy

* Caching
    - hit / miss
    - Writing policies:
        1. write-through
        2. write-behind
        3. write-around
    - Replacement polices:
        1. Least recently used
        2. Least frequently used
        3. Random selection

* Hashing

* Databases

    - Data can be either:
        1. blob
        2. Structured
        3. Graph
        4. key-value
    - ACID
        - Atomicity
        - Consistency
        - Isolation
        - Durability
    - Row-based vs Column-based tables:
        - In structured-based storage such as SQL, aatabase engines store data in pages, each page contains several records. Either we store all the values of a column over pages, then go to the next column and so on which is column-based, or store or the columns of a row, then the next row and so on which is row-based.
        - column-based tables are better in compression, aggregation based on one column, and worse if we will select values from multiple columns.
    - Partioning
        - Horizontal Partioning: split tables rows based on list, range of values or a hash function. 
        - Vertical Partioning: split columns into partitions.
        - Indices on horizontally partioned tables are smaller, so it will more probably fir in memory than the whole index.
    - Sharding
        - It is similar to partioning but you split your database across servers, they do not live together on the same server.
    - Replication
    - Indexes
    - Connection Pooling
        - Instead of establishing a connection with the database and closing that established connection, you cache a list of connections to use. When you need to talk to the database, you will use one of these established connections and you will not waste time establishing a new connection. However, you will have to wait if all your cached connections are being used.
    
* Networking
    - Protocols
        - IP
        - TCP
        - HTTP
        - HTTPS
        - UDP
    - Sockets
    - Peer-to-peer network

* Streaming

* Publish/subscribe


