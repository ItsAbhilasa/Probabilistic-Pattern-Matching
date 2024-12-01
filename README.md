# **WildHash: Randomized Pattern Matching with Modular Arithmetic**

Efficient and space-optimized pattern matching meets modern algorithms! 
WildHash is a lightweight, randomized algorithm for **exact and wildcard-based pattern matching** in strings. With probabilistic guarantees and modular arithmetic, this project showcases the power of mathematics in computer science. 

---

## **Features**
- **Exact Pattern Matching**: Find exact occurrences of a pattern in a text.
- **Wildcard Matching**: Match patterns with wildcards (`?`) that can substitute any character.
- **Randomized Approach**: Uses modular hashing with random prime numbers for high efficiency.
- **Error Control**: Customizable error bounds ensure minimal false positives.
- **Space Optimization**: Leveraging modular arithmetic for reduced memory usage.

---

## **How It Works**
1. **Randomized Primes**: Generates a random prime modulus for hash computations.
2. **Modular Arithmetic**: Computes incremental rolling hashes for pattern and text comparison.
3. **Wildcard Handling**: Dynamically skips wildcard positions during hash calculation.
4. **Error Tolerance**: Customizable probability of false positives using user-defined `eps`.

---

## **Applications**
- **Text Searching**: Quickly find patterns in large documents or databases.
- **Bioinformatics**: Match DNA sequences with tolerances for mismatches.
- **Log Analysis**: Search for patterns with approximate matching in log files.
- **Educational Tool**: Learn modular arithmetic and hashing in computer science.

---


Example:
```python
from wildhash import randPatternMatch, randPatternMatchWildcard

# Input text and pattern
text = "ABCDE"
pattern = "CD"

# Exact pattern matching
print(randPatternMatch(0.1, pattern, text))  # Output: [2]

# Wildcard matching
pattern_with_wildcards = "C?"
print(randPatternMatchWildcard(0.1, pattern_with_wildcards, text))  # Output: [2]
```

---

## **Project Structure**
- `wildhash.py`: Main implementation of the WildHash algorithm.
- `tests/`: Unit tests for exact and wildcard matching.
- `README.md`: Documentation for the project.
- `LICENSE`: Open-source license (optional).

---

## **Behind the Scenes**
This project is powered by:
- **Prime Number Theory**: Ensures efficient and collision-resistant hashing.
- **Modular Arithmetic**: Rolling hash implementation for fast substring comparisons.
- **Probabilistic Techniques**: Trade-offs between accuracy and performance.

---
