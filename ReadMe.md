# Templates

## Python Template

```python

import sys
input = sys.stdin.readline

############ ---- Input Functions ---- ############
def inp():
    return(int(input()))

def inlt():
    return(list(map(int,input().split())))

def insr():
    s = input()
    return(list(s[:len(s) - 1]))

def invr():
    return(map(int,input().split()))

if __name__ == '__main__':
    # Start coding

```

## Javascript Template

```javascript
"use strict";

process.stdin.resume();
process.stdin.setEncoding("utf-8");

let inputString = "";
let currentLine = 0;

process.stdin.on("data", (inputStdin) => {
  inputString += inputStdin;
});

process.stdin.on("end", (_) => {
  inputString = inputString
    .trim()
    .split("\n")
    .map((string) => {
      return string.trim();
    });

  main();
});

function readline() {
  return inputString[currentLine++];
}

function main() {
  const input = readline();

  // Start coding
}
```
