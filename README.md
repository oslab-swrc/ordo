# ordo

This reposiory addresses problems by proposing and designing a scalable ordering primitive, called Ordo, that relies on invariant hardware clocks. Ordo not only enables the correct use of these clocks, by providing a notion of a global hardware clock, but also frees various logical timestamp-based algorithms from the burden of the software logical clock, while trying to simplify their design. 

We use the Ordo primitive to redesign 
1) a concurrent data structure library that we apply on the Linux kernel; 
2) a synchronization mechanism for concurrent programming; 
3) two database concurrency control mechanisms; and 4) a clock-based software transactional memory algorithm.

This repository is under the terms of the Apache-2.0 license.

## How to use

- Build
```
$> make
```
- Copy the ordo value to include directory `ordo_clock.h`

## Reference
https://dl.acm.org/doi/abs/10.1145/3190508.3190510
```
@inproceedings{10.1145/3190508.3190510,
author = {Kashyap, Sanidhya and Min, Changwoo and Kim, Kangnyeon and Kim, Taesoo},
title = {A Scalable Ordering Primitive for Multicore Machines},
year = {2018},
isbn = {9781450355841},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3190508.3190510},
doi = {10.1145/3190508.3190510},
booktitle = {Proceedings of the Thirteenth EuroSys Conference},
articleno = {34},
numpages = {15},
location = {Porto, Portugal},
series = {EuroSys '18}
}
```
