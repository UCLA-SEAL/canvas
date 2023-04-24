# Canvas
Canvas: Isolated and Adaptive Swapping for Multi-Applications on Remote Memory ([NSDI 2023](https://www.usenix.org/conference/nsdi23/presentation/wang-chenxi))

## Summary
Remote memory techniques for datacenter applications have recently gained a great deal of popularity. Existing remote memory techniques focus on the efficiency of a single application setting only. However, when multiple applications co-run on a remote-memory system, significant interference could occur, resulting in unexpected slowdowns even if the same amounts of physical resources are granted to each application. This slowdown stems from massive sharing in applications’ swap data paths. Canvas is a redesigned swap system that fully isolates swap paths for remote-memory applications. Canvas allows each application to possess its dedicated swap partition, swap cache, prefetcher, and RDMA bandwidth. Swap isolation lays a foundation for adaptive optimization techniques based on each application’s own access patterns and needs. We develop three such techniques: (1) adaptive swap entry allocation, (2) semanticsaware prefetching, and (3) two-dimensional RDMA scheduling. A thorough evaluation with a set of widely-deployed applications demonstrates that Canvas minimizes performance variation and dramatically reduces performance degradation.

## Team
This project is done in collaboration with Professor [Harry Xu](http://web.cs.ucla.edu/~harryxu/)'s group at UCLA. Please visit [Canvas project at UCLA Systems](https://github.com/uclasystem/canvas). If you encounter any problems, please open an issue or feel free to contact us:

[Yifan Qiao](https://web.cs.ucla.edu/~yifan/): PhD student, [yifanqiao@ucla.edu](mailto:yifanqiao@ucla.edu).

## How to cite 
Please refer to our NSDI'23 paper, **[Canvas: Isolated and Adaptive Swapping for Multi-Applications on Remote Memory](https://www.usenix.org/system/files/nsdi23-wang-chenxi.pdf)** for more details. 

### Bibtex  
```txt
@inproceedings {qiao2023canvas,
author = {Chenxi Wang and Yifan Qiao and Haoran Ma and Shi Liu and Wenguang Chen and Ravi Netravali and Miryung Kim and Guoqing Harry Xu},
title = {Canvas: Isolated and Adaptive Swapping for {Multi-Applications} on Remote Memory},
booktitle = {20th USENIX Symposium on Networked Systems Design and Implementation (NSDI 23)},
year = {2023},
isbn = {978-1-939133-33-5},
address = {Boston, MA},
pages = {161--179},
url = {https://www.usenix.org/conference/nsdi23/presentation/wang-chenxi},
publisher = {USENIX Association},
month = apr,
}
```
