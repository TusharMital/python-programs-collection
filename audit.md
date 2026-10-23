# README Audit

## README Fact-Check Table

This audit checks whether the README's descriptions match the Python programs currently included in this repository. Claims should be updated if the source code changes.

| Claim Made in README | True? | Evidence / Correction Made |
|---|---|---|
| The factorial program calculates a factorial. | Yes | The program initializes `fact = 1` and multiplies it by each integer from `1` through `n`. |
| The factorial program calculates the factorial of a user-entered number. | No | The shown code sets `n = 5` directly. It does not use `input()`. Describe it as calculating the factorial of the fixed value `5`. |
| The factorial program accepts input from the terminal. | No | No terminal input is requested in the shown code. |
| The factorial program validates negative numbers. | No | The shown code has no check for `n < 0`. Do not claim negative-number validation. |
| The factorial program handles invalid input. | No | The shown code does not accept user input and contains no error-handling logic. |
| The factorial program uses a loop. | Yes | It uses `for i in range(1, n + 1)`. |
| The factorial program uses multiplication. | Yes | `fact = fact * i` multiplies the running factorial by each loop value. |
| The factorial program outputs `120` when `n = 5`. | Yes | Starting with `fact = 1`, the loop computes `1 × 2 × 3 × 4 × 5 = 120`. |
| The Fibonacci program generates a Fibonacci sequence. | Yes | The provided code starts with `a = 0` and `b = 1`, prints `a`, then updates the pair using their sum. |
| The Fibonacci program prints the first 10 Fibonacci numbers. | Yes | The shown code uses `n = 10` and loops `range(n)` times. |
| The Fibonacci program accepts the number of terms from the user. | No | The shown code sets `n = 10` directly and does not use `input()`. |
| The Fibonacci program uses a loop. | Yes | It uses `for i in range(n)`. |
| The Fibonacci program uses variable updates to calculate the next term. | Yes | It calculates `next_num = a + b`, then assigns `a = b` and `b = next_num`. |
| The Fibonacci output is `0 1 1 2 3 5 8 13 21 34`. | Yes | This is the output produced by the provided 10-iteration code. |
| The programs require NumPy or other external packages. | No, based on the shown code | The provided factorial and Fibonacci snippets use only Python built-ins. Check the structure-to-dictionary program before making a repository-wide dependency claim. |
| Python 3 can run the factorial and Fibonacci scripts. | Yes | Both shown programs use standard Python syntax and built-in language features. |
| The structure-to-dictionary program converts a structure or object into a dictionary. | Needs verification | Confirm this against the actual code in `structure_to_dictionary.py` before treating the claim as verified. |
| The structure-to-dictionary program accepts user input, validates data, or handles errors. | Needs verification | These features cannot be confirmed without reviewing the actual structure-to-dictionary code. Do not claim them unless the code implements them. |
| The repository requires a `requirements.txt` file. | Not established | The two shown programs have no third-party dependencies. A `requirements.txt` is not necessary for these programs alone; check the third program before making a repository-wide statement. |
| The repository includes a particular open-source licence. | Not established | Only claim a licence if a `LICENSE` file is present in the repository. |

## Audit Notes

- The factorial and Fibonacci entries above are based on the code provided for review.
- The structure-to-dictionary program must be checked against its actual source before its behavior can be fully audited.
- Keep the README aligned with the code. If the code changes, review the claims and expected outputs again.
- Do not describe fixed values as user input, and do not claim validation or error handling unless those features exist in the code.
