# Circular Doubly Linked List & Round-Robin Scheduler

This project implements a **Circular Doubly Linked List** in Java and simulates a **Round-Robin Process Scheduler** using that structure. The main goal is to practice interpreting UML diagrams, working with interfaces, and managing dynamic data structures.

## 🧠 Key Concepts

- Circular Doubly Linked List (CDLL)
- Linked data structures
- Round-robin scheduling algorithm
- Object-oriented programming with Java
- UML class diagram interpretation
- JUnit testing and exception handling

## 🗂️ Project Structure

|-- src
| |-- ADTs
| |-- Apps
| |-- DataStructures
|
|-- test
| |-- ADTs
| |-- Apps
| |-- DataStructures
|
|-- lib
| |-- hamcrest-core-1.3.jar
| |-- junit-4.12.jar
| |-- DS_Library_List.jar
|
|-- test-.dat / test-.results

markdown
Copy
Edit


### 🔧 Core Files

- `CircularDoublyLinkedList.java`: Core class implementing the CDLL.
- `DoublyLinkedNode.java`: Node class used by the list.
- `Scheduler.java`: Application demonstrating round-robin scheduling.
- `Job.java`, `Events.java`: Helper classes used in scheduling.
- `CircularDoublyLinkedListTest.java`: Unit tests for CDLL implementation.
- `SchedulerTest.java`: Functional tests for scheduler logic.

## 📦 Setup Instructions

1. **Download and unzip the project folder.**
2. **Open the project in NetBeans 8.2.**
3. **Add the libraries from the `lib` folder:**
   - `hamcrest-core-1.3.jar`
   - `junit-4.12.jar`
   - `DS_Library_List.jar`
4. **Implement and test the following methods in `CircularDoublyLinkedList.java`:**
   - `addLast`
   - `addFirst`
   - `addAfter`
   - `remove`
   - `removeLast`
   - `contains`
5. **Run JUnit tests in `CircularDoublyLinkedListTest.java`.** All 31 tests should pass.

## 📈 Scheduler Use Case

The project models a **Round-Robin Scheduler**, where jobs take turns executing in a fixed time slice. If a job isn't finished, it's placed at the end of the list. Finished jobs are removed from the list.

This simulates real-world process scheduling in operating systems.

## ✅ Testing

- Unit tests use **JUnit 4.12**.
- Test cases cover:
  - Empty list scenarios
  - Element not found
  - Correct link adjustments
  - Edge cases and exception handling

## 💡 Example Methods

```java
public void addLast(T element);
public T remove(T element) throws EmptyCollectionException, ElementNotFoundException;
public boolean contains(T element);


## 🙏 Acknowledgments

This project was developed as part of a course assignment for [202310-Spring 2023-ITSC-2214-001-Data Structures and Algorithms] at [UNC Charlotte].

Project design, diagrams, and starter files were provided by [Dr. Qiong Cheng].

