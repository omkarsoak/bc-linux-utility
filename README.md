# *bc* Linux Utility
#### An Arbitrary Length Binary Calculator (*bc*) for Linux terminal

A command line calculator that supports very large integers. It can perform addition, subtraction, multiplication, and division on numbers far beyond standard data type limits. The program processes entire expressions directly in infix form using stacks, and it stores each number as a linked list in which every digit is a node.

### Features
- Handles numbers of any size  
- Supports addition, subtraction, multiplication, and division  
- Evaluates full expressions in infix form using stack based processing  
- Stores numbers as linked lists for flexible size management  
- Example expression: `12038138198*120398019281-1232198319283+834729387242/32242`

---

## Run Locally

```bash
gcc -Wall main.c linked_list.c stack.c operations.c -o main
```

- **Input:** A single string containing integers and operators `+` `-` `*` `/`  
- **Output:** The computed result  

### Example  
```bash
Input: 198237918479+83634875862-123312*242 
Output: 281842952837
```

## Data Structures used

- Linked list to store each number with one digit per node  
- Stack of nodes to hold numbers during infix evaluation  
- Stack of characters to hold operators during expression parsing