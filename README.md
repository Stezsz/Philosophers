# 🍝 Philosophers – 42 School Project

The **Philosophers** project is a synchronization challenge that simulates the dining philosophers problem using multiple threads. Each philosopher alternates between thinking and eating. They need two forks to eat, and can only hold one fork at a time. The goal is to avoid deadlock and ensure that no philosopher is starving.

---

## 🎯 Main Objectives

- Implement synchronization and mutual exclusion with threads.
- Ensure all philosophers can eat without starving or deadlocking.
- Use mutexes and semaphores for thread synchronization.
- Avoid race conditions and unnecessary complexity.
- Develop the solution in C using **POSIX threads (pthreads)**.

---

## 🧠 Problem Breakdown

- **Philosophers:** Each philosopher alternates between thinking and eating. They need two forks to eat, but can only hold one fork at a time.
- **Forks:** There are five forks in total, one for each philosopher, placed between them.
- **Deadlock:** The goal is to avoid a scenario where no philosopher can eat because they are all waiting for forks.
- **Starvation:** The system must ensure that all philosophers get a chance to eat.

---

## 🧪 Example Usage

```bash
$ make
$ ./philosophers 5 800 200 200 0
```

Arguments:
- `5` – Number of philosophers.
- `800` – Time in milliseconds each philosopher will spend thinking.
- `200` – Time in milliseconds each philosopher will spend eating.
- `200` – Time in milliseconds before checking if the philosopher is dead.
- `0` – Maximum number of times a philosopher can eat before terminating.

The program will simulate the philosophers' behavior and print the events.

---

## 📘 Conclusion

The **Philosophers** project introduces complex concepts of **thread synchronization**. It teaches how to avoid common pitfalls like deadlocks and starvation in a multithreaded environment. Solving this problem helps develop a deeper understanding of concurrency and resource management in C programming.

---

> ✅ **Final Grade: 100/100**
> Project made at [42 Lisboa](https://www.42lisboa.com/pt/)
> 👤 Author: Stephan Rodrigues Lassaponari ([@Stezsz](https://github.com/Stezsz))
