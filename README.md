# Hyperelliptic Curve Computations

This repository contains Magma scripts for performing computations related to hyperelliptic curves (HECs) over finite fields. The scripts are designed to compute isomorphism classes of superspecial HECs whose automorphism contain quaterninon.

## Files

### `alg2.mgm`
This script computes the number of isomorphism classes of superspecial hyperelliptic curves over finite fields.

### `alg3.mgm`
The script iterates over a range of prime numbers and outputs the representatives of superspecial HECs whose automorphism is quaternion for each prime.

## Requirements

- **Magma Computational Algebra System**: These scripts are written in Magma, a specialized software for algebraic computations. You must have Magma installed to run these scripts. For more information, visit the [Magma website](http://magma.maths.usyd.edu.au/magma/).

## Usage

1. Open a terminal in the directory containing the script files.
2. Run the desired script using the Magma command:
   ```bash
   magma alg2.mgm
