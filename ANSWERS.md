# Answers

## 1. Thread vs Process
A process is an independent program with its own memory, while a thread is a smaller unit inside a process that shares memory. Threads are faster to create and communicate compared to processes. In this assignment, we used threads because they are lightweight and efficient. Also, threads can easily share data which makes scheduling easier. Processes require more resources and are slower.

---

## 2. Ready Queue Behavior
In Round Robin scheduling, if a process does not finish within its time quantum, it is placed back into the ready queue. For example, in the output, we see a process running for a short time and then returning to the queue. This ensures fairness because all processes get equal CPU time. Re-queueing prevents any process from using the CPU for too long.

---

## 3. Thread Lifecycle
A thread starts in the New state when it is created. After calling Thread.start(), it moves to Runnable state. When the CPU executes it, it enters Running state. If it waits (like Thread.sleep()), it goes to Waiting state. Finally, after finishing execution, it enters Terminated state. In this program, each process thread follows this lifecycle.

---

## 4. Real-World Applications
One example is a web server handling multiple users at the same time. Each request is handled by a thread using scheduling. Another example is a game engine where multiple tasks like rendering and input handling run concurrently. Round Robin scheduling ensures fairness and smooth performance. These systems rely on multithreading to improve responsiveness.
