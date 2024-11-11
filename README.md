# raspi_c_optimization
A group project focused on different optimization techniques and levels in programming. Tested on raspberry pi's

## Assignments

- [ ] Constant Folding - Graham
- [ ] Loop Unrolling - Jaden
- [ ] Dead Code Elimination - Bryce
- [ ] Loop Invariant Code Motion - Nicky
- [ ] Subexpression Elimination - Isaac
- [ ] General Code Motion - All?

## Steps
1. Add code examples to a folder titled your assignment:

```
constant_folding/
    - optimized.c
    - unoptimized.c
    - ...
loop_unrolling/
    - optimized.c
    - unoptimized.c
    - ...
```

3. Compile with each optimization level on the pi's
4. Profile with Massif - Memory and cache performance changes from original to optimized
5. Document all info in a table below

## Results

### Subexpression Elimination ***SEE***

The table below shows runtime per System/Example combo

| System/Example   |   -O0    |   -O1    |   -O2    |   -O3    | 
| ---------------- | -------- | -------- | -------- | -------- |
| PC/Optimized     | 0.129317 | 0.051817 | 0.056084 | 0.055378 |
| PC/Unoptimized   | 0.166281 | 0.051825 | 0.055457 | 0.054935 |
| Rasp/Optimized   | -------- | -------- | -------- | -------- |
| Rasp/Unoptimized | -------- | -------- | -------- | -------- |

The table below shows Memory Usage per System/Example combo in MB

| System/Example   |   -O0    |   -O1    |   -O2    |   -O3    | 
| ---------------- | -------- | -------- | -------- | -------- |
| PC/Optimized     |   15.27  |   15.27  |   15.27  |   15.27  |
| PC/Unoptimized   |   15.27  |   15.27  |   15.27  |   15.27  |
| Rasp/Optimized   | -------- | -------- | -------- | -------- |
| Rasp/Unoptimized | -------- | -------- | -------- | -------- |

The table below shows total instruction count per System/Example combo in millions

| System/Example   |   -O0    |   -O1    |   -O2    |   -O3    | 
| ---------------- | -------- | -------- | -------- | -------- |
| PC/Optimized     |   75.50  |   25.91  |   17.57  |   17.57  |
| PC/Unoptimized   |   109.8  |   25.91  |   17.57  |   17.57  |
| Rasp/Optimized   | 0.129317 | 0.051817 | 0.056084 | 0.055378 |
| Rasp/Unoptimized | 0.129317 | 0.051817 | 0.056084 | 0.055378 |



## Challenges faced

TODO: challenges we faced 

