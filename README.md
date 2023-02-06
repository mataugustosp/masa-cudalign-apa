# Masa-Cudalign-APA

The comparison of biological sequences is one of the main tasks in Bioinformatics, existing a range of exact algorithms that use dynamic programming for this purpose. These algorithms have quadratic complexity in time $O({n^2})$ and can take a lot of execution time depending on the situation. To alleviate this problem, parallel tools have been proposed. This Project presents the Agile Pruning Alignment Module (APA) that is integrated with the parallel tool MASA-CUDAlign for one GPU and modifies the Block Pruning optimization strategy, seeking to speed up pruning and increase the the dynamic programming matrix's discard area. For this purpose, the heuristic aligner BLAST is used to generate an initial score to be automatically inserted into MASA-CUDAlign, which initially had a score of 0.

### Donwload 

Latest Version: 

### Compiling CUDAlign 

```console
cd masa-cudalign-apa/masa-cudalign
./configure 
make 
```

### Compiling APA Module

In masa-cudalign-apa directory: 

```console
  g++ modulo_apa.cpp -o apa 
```

### Executing APA Module

```console
  ./apa [options] seq1.fasta seq2.fasta 
```

  
