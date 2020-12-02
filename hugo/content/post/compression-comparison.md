---
title: "Compression Comparison"
author: "Aleksa Ognjanović"
description: "Here I am going to show differences in various compression algorithms. This is a handy cheatsheet for (de)compressing commands."
categories: [
    "compression"
]
tags: [
    "compression",
    "linux",
    "cheatsheet"
]
date: 2020-12-02T18:40:48+01:00
---

## Compressing

### Gunzip
```sh
tar -cjvf test.tar.gz test
```
- c - create archive
- j - gz
- v - verbose
- f - file name of output

### Bzip2
```sh
tar -czvf test.tar.bz2 test
```
- z - bz2

### XZ
```sh
tar -cJvf test.tar.xz test
```
- J - xz

### Zip
```sh
zip -r test.zip test
```
- r - recursive

### 7zip
```sh
7z a test.7z test
```
- a - add

### Rar
```sh
rar a test.rar test
```

## Decompressing

### Tar
```sh
tar -xfv test.tar.*
```
- x - extract
- f - file to extract
- v - verbose

### Zip
```sh
unzip test.zip
```

### 7zip
```sh
7z x test.7z
```

### Rar
```sh
rar x test.rar
```

Source is available at: https://github.com/GrbavaCigla/CompressionComparison