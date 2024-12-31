# Bioinformatics_Algorithms

This repository contains a Colab notebook addressing three fundamental problems in bioinformatics. Each problem demonstrates the application of computational techniques like dynamic programming and string algorithms to solve biologically significant tasks.  

## Problems Overview  

### 1. String Alignment: Edit Distance  
#### Category: String Alignment  
**Description**:  
This problem computes the minimum number of edit operations required to transform one string into another. Edit operations include substitution, insertion, and deletion of single symbols. Insertions and deletions are treated as individual operations, even when applied to contiguous intervals (gaps).  

- **Input**:  
  Two protein strings in FASTA format, each of length at most 1000 amino acids.  
- **Output**:  
  The edit distance between the two strings.  
- **Applications**:  
  - Measuring evolutionary distance between genetic sequences.  
  - Spell checking and natural language processing.  

---

### 2. Dynamic Programming: Perfect Matchings and RNA Secondary Structures  
#### Category: Dynamic Programming  
**Description**:  
This problem explores RNA secondary structures by modeling possible base-pair matchings. A perfect matching is defined as a set of basepair edges where no nucleotide is left unpaired, and all constraints on pairings ({A, U} and {C, G}) are respected. Using dynamic programming, the total number of perfect matchings is computed.  

- **Input**:  
  An RNA string of length at most 80 bp, with equal occurrences of 'A' and 'U' and of 'C' and 'G'.  
- **Output**:  
  The total number of perfect matchings in the RNA string's bonding graph.  
- **Applications**:  
  - RNA structure prediction.  
  - Understanding RNA folding patterns.  

---

### 3. String Algorithm: Finding All Similar Motifs  
#### Category: String Algorithm  
**Description**:  
This problem identifies all substrings of a genome that are within a fixed edit distance from a given motif. The edit distance is computed, and substrings satisfying the distance threshold are returned with their positions and lengths.  

- **Input**:  
  - A positive integer \( k \) (\( k \leq 50 \)).  
  - A DNA string \( s \) (motif) of length at most 5 kbp.  
  - A DNA string \( t \) (genome) of length at most 50 kbp.  
- **Output**:  
  All substrings \( t' \) of \( t \) such that \( d_E(s, t') \leq k \), encoded as pairs of their start positions and lengths.  
- **Applications**:  
  - Identifying repeated motifs in genomes with mutations.  
  - Motif discovery in regulatory regions.  

---

## Repository Structure  
```plaintext
/  
|-- bioinformatics_algorithms.ipynb  # Colab notebook containing the solutions to all three problems  
|-- README.md                        # Project documentation  
