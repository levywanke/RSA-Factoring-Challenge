
# RSA Factoring Challenge

## Overview
This project is an implementation of a program that factors RSA numbers into their prime factors. It's designed to be efficient and capable of running within a strict time limit of 5 seconds per input number. The challenge involves factorizing large numbers, which are crucial for decrypting potentially sensitive information.

## Project Structure
The project consists of two main executables and respective functionalities:

- **factors**: General number factorization where the factors may not necessarily be prime.
- **rsa**: Specialized version where the factors are always prime.

## Requirements
- **Language:** You can choose any programming language.
- **OS:** Standard Ubuntu 20.04 LTS.
- **Dependencies:** None; the program must run independently without any additional installs.
- **Execution Limit:** Programs will be terminated if they exceed 5 seconds per input number.

## Usage
### For `factors`
To factorize multiple numbers from a file into their product of two smaller numbers:

```bash
./factors <file>
```

- `<file>`: Contains natural numbers, one per line. Each line will be factorized into `n = p*q`.

### For `rsa`
To factorize a single RSA number into its prime factors:

```bash
./rsa <file>
```

- `<file>`: Contains one RSA number per file. Each number will be factorized into `n = p*q` where `p` and `q` are prime.

## Example
### `factors` Example
Given input file `tests/test00`:

```
4
12
34
128
1024
4958
1718944270642558716715
9
99
999
9999
9797973
49
239809320265259
```

Output:

```
4=2*2
12=6*2
34=17*2
128=64*2
1024=512*2
4958=2479*2
1718944270642558716715=343788854128511743343*5
9=3*3
99=33*3
999=333*3
9999=3333*3
9797973=3265991*3
49=7*7
239809320265259=15485783*15485773
```

### `rsa` Example
Given input file `tests/rsa-1`:

```
6
```

Output:

```
6=3*2
```

