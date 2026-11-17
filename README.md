Client-Aided Hybrid FHE for Transformer Inference

Code and raw results for the paper "Client-Aided Hybrid FHE for Transformer Inference: A CKKS-to-TFHE Transcoding Approach" by Asuman Dumlu and Bayram Ali Ersoy (submitted to Cryptography, MDPI).

The repository implements a client-aided protocol that moves a value between CKKS (OpenFHE) and TFHE (Concrete). The server masks a CKKS ciphertext with a one-time pad, and the client decrypts the masked value and sends back TFHE encryptions of table indices. The server evaluates the nonlinear function as a masked lookup table by programmable bootstrapping. The client then re-encrypts the masked result in CKKS, and the server removes the mask. The linear parts stay in CKKS. The repository contains the protocol code, the experiment scripts, and the raw result files behind the tables of the paper.
