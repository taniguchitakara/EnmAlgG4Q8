# Hyperelliptic Curve Computations

This repository contains Magma scripts for performing computations related to hyperelliptic curves (HECs) over finite fields. The scripts are designed to compute properties of HECs and enumerate specific types of curves based on given criteria.

## Files

### `alg2.mgm`
This script computes the number of isomorphism classes of hyperelliptic curves over finite fields. It uses the following main functions:

1. **`cartier_gcd_root(p)`**  
   Computes the greatest common divisor (GCD) of a sequence of coefficients derived from a polynomial associated with the hyperelliptic curve. This function is used to identify singularities and other properties of the curve.

2. **`count_isomorphism(p, gcd_all)`**  
   Counts the number of isomorphism classes of hyperelliptic curves for a given prime `p` using the GCD computed by `cartier_gcd_root`.

The script iterates over a range of prime numbers and outputs the number of isomorphism classes for each prime.

### `alg3.mgm`
This script enumerates hyperelliptic curves over finite fields that satisfy specific conditions. It uses the following main functions:

1. **`cartier_gcd_root(p)`**  
   Similar to the function in `alg2.mgm`, this computes the GCD of a sequence of coefficients derived from a polynomial associated with the hyperelliptic curve.

2. **`enumerate_hec(p, gcd_all)`**  
   Enumerates hyperelliptic curves for a given prime `p` using the GCD computed by `cartier_gcd_root`. It filters out invalid roots and generates a list of valid curves.

The script iterates over a range of prime numbers and outputs the enumerated curves for each prime.

## Requirements

- **Magma Computational Algebra System**: These scripts are written in Magma, a specialized software for algebraic computations. You must have Magma installed to run these scripts. For more information, visit the [Magma website](http://magma.maths.usyd.edu.au/magma/).

## Usage

1. Open a terminal in the directory containing the script files.
2. Run the desired script using the Magma command:
   ```bash
   magma alg2.mgm