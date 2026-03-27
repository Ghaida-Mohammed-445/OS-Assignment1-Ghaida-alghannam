# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

A process is a program that runs with its own memory.
A thread is a small part of a process.
Threads share the memory of their process, but processes do not share memory.
Creating a thread is faster and needs less time and resources than a new process.
Threads are good for this assignment because they use less context switch and share data easily.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**
If a process does not finish in its time quantum, it is added back to the ready queue.
Adding the process to the queue is important so it can continue its work   



Example from my output:
 ظû╢ P1 executing quantum [4000ms] 
  ظأة Quantum progress: [ظûêظûêظûêظûêظûêظûêظûêظûêظûêظûêظûêظûêظûêظûêظûê] 100%
  ظ╕ P1 completed quantum 4000ms ظ¤é Overall progress: [ظûêظûêظûêظûêظûêظûêظûêظûêظûêظûّظûّ ظûّظûّظûّظûّظûّظûّظûّظûّظûّ] 46%
     Remaining time: 4553ms
  ظ╗ P1 yields CPU for context switch

  ظئـ P1java.awt.Color[r=255,g=255,b=0] (Priority: 5) added to ready queue ظ¤é Burst time: 8553ms

**Explanation of example:**
This is an example of a process that did not finish its work, so it was added to the ready queue



---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**


1. **New**: P1 is New when we make it but do not start it yet
2. **Runnable**:After we use Thread.start() P1 is Runnable and waits for the CPU
3. **Running**: P1 is Running when the CPU runs its code in run()
4. **Waiting**: P1 goes Waiting if we use Thread.sleep() or Thread.join()
5. **Terminated**: P1 is Terminated when it finishes all its work
---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1:YouTube

**Description**: 
YouTube runs many tasks like playing a video loading comments and downloading next videos in the background

**Why Round-Robin works well here**: 
Each task gets a fair turn to use the CPU so the app stays smooth fast and responsive

### Example 2: WhatsApp

**Description**: 
A chat app handles receiving messages showing notifications and letting the user type at the same time


**Why Round-Robin works well here**: 
Round-Robin gives each task a small time slice so everything works together quickly and nothing freezes

---

## Summary

**Key concepts I understood through these questions:**
1. 
2. 
3. 

**Concepts I need to study more:**
1. 
2. 
