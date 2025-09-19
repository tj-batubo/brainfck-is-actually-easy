# Brainfuck Is Actually Easy

This repository contains my notes and code experiments while learning **Brainfuck** — one of the smallest and most minimal programming languages ever created.  

Brainfuck was designed to be extremely simple:  
- The entire language has **only 8 commands**.  
- Programs work on a **memory block** made of slots (cells).  
- Each slot holds a single **byte** (a number between `0` and `255`).  
- A **pointer** moves across these slots to read and change values.  

Despite being minimal, Brainfuck is *Turing complete*, meaning you can technically write any program with it (though it won’t be pretty).  

---

## 🧠 The Basics

### Memory & Pointer
- Think of memory as a row of boxes (slots).  
- Each box holds a number from `0` to `255`.  
- A **pointer** tells you which box you’re currently at.  

### ASCII
When printing values, Brainfuck uses the **ASCII table**:  
- Example: `65` → `A`, `66` → `B`, etc.  
- To print text, you set a cell to the ASCII value of the character, then output it.  

---

## 🔑 The 8 Commands

| Command | Meaning |
|---------|----------|
| `>` | Move pointer right (to the next cell) |
| `<` | Move pointer left (to the previous cell) |
| `+` | Increment current cell value by 1 |
| `-` | Decrement current cell value by 1 |
| `.` | Output the value at the current cell as an ASCII character |
| `,` | Input a character and store its ASCII value in the current cell |
| `[` | Start loop (run code inside as long as current cell ≠ 0) |
| `]` | End loop |

---

## 📖 Example

To print `A` (ASCII 65):  
- Use `+` to increase a cell’s value until it reaches 65.  
- Then use `.` to print it.  

```brainfuck
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++.
````

---

## ℹ️ Why This Repo Exists

This repo is my personal journey into Brainfuck.

* **Not a tutorial** — just a reference so that when you look at my code, you’ll know how Brainfuck works at a high level.
* If you’ve never seen Brainfuck before, this README gives you enough context to figure out what’s going on.

---

## 🚀 Next Steps

If you want to dive deeper:

* Look up an [ASCII table](https://www.asciitable.com/) (super useful).
* Try writing a simple “Hello World” program.

---

