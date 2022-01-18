# Math.NumberTheory.Padic

Module introduces p-adic integers and p-adic rational numbers of fixed and arbitratry precision, implementing basic arithmetic as well as some specific functions, i.e. detection of periodicity in digital sequence, rational reconstruction, square roots etc.

In order to gain efficiency the integer p-adic number with radix `p` is internally
represented in form `N mod p^k` as only one digit `N`, lifted to modulo `p^k`, where `k` is chosen so that within working precision numbers belogning to `Int` and `Ratio Int` types could be reconstructed by extended Euclidean algorithm. Canonical expansion is used for textual output only.
