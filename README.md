# Bachelor thesis of Thua Duc Nguyen

Effective resource access management is pivotal in modern computing systems such as filesystems, operating systems, and databases. Traditional single-locking methods often lead to bottlenecks and hinder parallelism among writers. Range locks have emerged as a promising solution to this issue by dividing shared resources into smaller segments, allowing concurrent access and enhancing system efficiency.

This thesis investigates scalable range-locking techniques motivated by the increasing interest in replacing traditional locking mechanisms, such as the `mmap_lock` in the Linux kernel, with more refined approaches. By focusing on critical ranges rather than coarse-grained locking, range locks facilitate concurrent transactions, thereby reducing memory overhead and improving throughput.

The research builds upon existing work in scalable range locks, exploring implementations based on skip and linked lists as alternatives to interval trees. A new concurrent range lock design is proposed, leveraging a probabilistic concurrent skip list, which offers efficient insertion and lookup operations while addressing contention points inherent in previous approaches.

The proposed range lock mechanism will be evaluated based on performance, correctness, and comparison with existing state-of-the-art solutions. Performance testing under varying loads and concurrent accesses will provide insights into the scalability and efficiency of the proposed mechanism. Ensuring data consistency and correctness, especially in scenarios involving overlapping data ranges and concurrent operations, will be a crucial aspect of the evaluation process. Additionally, a comparative analysis will highlight the advantages and potential trade-offs of the proposed solution against existing approaches.

The expected outcome of this research is the development of a scalable range lock that outperforms existing solutions in terms of performance and resource utilization. The findings will enhance resource access management in critical computing systems, paving the way for improved parallelism and efficiency in various applications.


