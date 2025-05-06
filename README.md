# 🎢 Day-33: Java Data Structures – Queue & Stack

Welcome to **Day-33** of our Backend Engineering journey! Today, we're diving into **two of the most powerful and foundational data structures** in software development: `Queue` (FIFO) and `Stack` (LIFO).

This lesson is packed with **real-world applications**, an engaging **project assignment**, and plenty of practice to help you internalize these concepts like a pro.

---

## 📚 What You'll Learn

- ✅ The difference between `Queue`, `Stack`, `Deque`, and `Collection`
- ✅ FIFO vs LIFO — what they mean, and why they matter
- ✅ How to use `Queue` and `Stack` with Java Collections Framework
- ✅ How to simulate real-world processes using these data structures
- ✅ Writing clean, testable code using OOP and Maven
- ✅ Unit testing with JUnit 5

---

## 💬 Summary of Key Concepts

### 🔁 Stack (LIFO)
- Last-In, First-Out
- Think: Undo history, browser back buttons, function calls
- Java: `Stack<T>`, or use `Deque<T>` as a better alternative

### 🚶 Queue (FIFO)
- First-In, First-Out
- Think: Customer lines, job schedulers, request handlers
- Java: `Queue<T>` with implementations like `LinkedList` or `ArrayDeque`

### 🔁 Deque (Double-Ended Queue)
- You can add/remove from both ends
- Behaves like both a Stack *and* a Queue

---

## 🚀 Assignment: RideManagerPro 🎡

You will implement a **CLI-based amusement park ride manager** that uses:

- A **Queue** to handle guest lineups
- A **Stack** to keep track of the last riders (for safety/photo review)

🧩 Full details are in the assignment file:  
📄 [`RideManagerPro Assignment`](https://github.com/FW-Zalando-Java-Backend-Engineer/RideManagerPro)

✅ The project uses:
- Java 17+
- Maven
- Clean OOP architecture
- Custom exceptions
- Unit tests with JUnit 5

---

## 🛠️ Project Setup Instructions

### 📦 Maven Project

If you're creating from scratch:

1. Open IntelliJ → New Project → Maven
2. Use:
```

GroupId: org.ridepark
ArtifactId: RideManagerPro

````

3. Fix JUnit dependency in `pom.xml`:
```xml
<dependency>
  <groupId>org.junit.jupiter</groupId>
  <artifactId>junit-jupiter-engine</artifactId>
  <version>5.9.1</version>
  <scope>test</scope>
</dependency>
````

---

## 🔍 File Structure (Suggestion)

```
RideManagerPro/
├── main/
│   └── RideManagerApp.java         # CLI interface
├── ride/
│   ├── Guest.java                  # Represents a visitor
│   ├── RideQueueManager.java       # Handles FIFO queue
│   └── RideHistoryStack.java       # Handles LIFO stack
├── exception/
│   ├── EmptyQueueException.java
│   └── NoRideHistoryException.java
└── test/
    └── ride/
        ├── RideQueueManagerTest.java
        └── RideHistoryStackTest.java
```

---

## 🧪 Testing Guide

Write **JUnit 5 tests** for:

| Class              | Test Class Name        |
| ------------------ | ---------------------- |
| `RideQueueManager` | `RideQueueManagerTest` |
| `RideHistoryStack` | `RideHistoryStackTest` |
| `Guest`            | `GuestTest`            |

✅ Use `@BeforeEach`, `@DisplayName`, `assertThrows`, and other best practices.

---

## 🧠 Your Tasks

| Task                       | Status |
| -------------------------- | ------ |
| Understand Stack and Queue | ✅      |
| Fork this repo             | ⏳      |
| Clone & open in IntelliJ   | ⏳      |
| Implement the codebase     | ⏳      |
| Write full test coverage   | ⏳      |
| Push to your GitHub        | ⏳      |
| Submit your repo link      | ⏳      |

---

## 📼 Zoom Recording

🎥 **Lecture Recording for Day-33**:
🔗 [Click to Watch](https://us06web.zoom.us/rec/share/5ZCUX4_zcxOKX0rM6udNhJYRrcliVKITtfIQtmwSkSGyDP22nOg8IxWHyeRznyQ8.UNdXCncmaDIdyZG2?startTime=1746428918000)

🧪 **Demo Exercise**:
[Customer Service Ticketing System](https://github.com/FW-Zalando-Java-Backend-Engineer/CustomerServiceSystem) 
---

## ✍️ Exercise Submission

Please complete the following and submit via Google Form (or platform):

* Fork this repo and implement `RideManagerPro`
* Add your name to the `README` if working as a group
* Push code to GitHub
* Submit your GitHub repo link [here](#)

---

## 🏁 Completion Checklist

* [ ] RideManagerApp.java runs with full CLI
* [ ] Queue and Stack behavior fully demonstrated
* [ ] JUnit 5 tests written for every class
* [ ] Custom exceptions handled
* [ ] Clean OOP design & JavaDocs
* [ ] README filled with your name

---

## 🧠 Final Thoughts

> "Mastering Stack and Queue is like learning how traffic works:
> You’ll build faster, cleaner, and smarter systems.
> And remember — a good ride manager never lets guests jump the line (unless you're coding in PHP)." 😄

---

## 📚 References

### 🔹 Official Documentation

* [Java Collections Framework (Oracle Docs)](https://docs.oracle.com/javase/8/docs/technotes/guides/collections/index.html)
* [Java `Queue` Interface (Oracle)](https://docs.oracle.com/javase/8/docs/api/java/util/Queue.html)
* [Java `Stack` Class (Oracle)](https://docs.oracle.com/javase/8/docs/api/java/util/Stack.html)
* [Java `Deque` Interface](https://docs.oracle.com/javase/8/docs/api/java/util/Deque.html)

---

### 🔹 Articles & Tutorials

* [Beginner’s Guide to Java Data Structures: Stack and Queue – by Alexander Obregon](https://medium.com/@AlexanderObregon/beginners-guide-to-java-data-structures-stack-and-queue-54b6f7259a08)
* [GeeksforGeeks – Stack in Java](https://www.geeksforgeeks.org/stack-class-in-java/)
* [GeeksforGeeks – Queue in Java](https://www.geeksforgeeks.org/queue-interface-java/)
* [Baeldung – Introduction to Java Collections](https://www.baeldung.com/java-collections)

---

### 🔹 Videos & Visuals

* [Queue vs Stack Visualization (YouTube)](https://www.youtube.com/watch?v=wjI1WNcIntg)
* [Java Stack vs Queue - Simple Animation](https://www.youtube.com/watch?v=wjI1WNcIntg)
* [Core Java Tutorial (Telusko - YouTube)](https://www.youtube.com/watch?v=TBWX97e1E9g&list=PLsyeobzWxl7poL9JTVyndKe62ieoN-MZ3)

---

### 🔹 Practice Platforms

* [LeetCode – Stack Tag](https://leetcode.com/tag/stack/)
* [LeetCode – Queue Tag](https://leetcode.com/tag/queue/)
* [HackerRank – Data Structures Practice](https://www.hackerrank.com/domains/tutorials/10-days-of-javascript)




