# G_cand

Source code repo for the gcand.so  metioned by our paper.

Our purpose is generating candidatesets for GNN model . Thus , We modified the huge code in LKH algorithm , only retain the CandidateSet part . We uses **Ctype** to transfer C function to Python to refrain from the expensive IO cost 

## Download

Just clone the repo from github

```shell
git clone https://github.com/rainingapple/G_cand.git
```

## Build

Using gcc -shared to build a .so file

```shell
gcc -I SRC/INCLUDE SRC/*.c -fPIC -shared -o gcand.so
```

### Usage

Move gcand.so file to corresponding folder

```shell
mv gcand.so "your folder path"
```

