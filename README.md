Table of Contents
About the Project
Features
Tech Stack
Data Structures Used
Installation & Usage
Project Workflow
Learning Outcomes
About the Project

The Banking Transaction System is a console-based application that manages customer transactions efficiently using a Queue data structure. It demonstrates the practical implementation of queues, one of the fundamental concepts in data structures.

The system processes transactions in FIFO (First In First Out) order, ensuring fair and sequential handling of customer requests such as deposits and withdrawals.

Features
Feature	Description
Add Transaction	Insert a new customer transaction into the queue
Process Transaction	Process the front transaction (deposit/withdraw)
Display Transactions	View all pending transactions
FIFO Processing	Ensures transactions are handled in order
Queue Overflow Handling	Prevents insertion when queue is full
Queue Underflow Handling	Prevents processing when queue is empty
Tech Stack
+------------------+------------------+------------------+
|   Programming    |   Data Structure |     Approach     |
+------------------+------------------+------------------+
|        C         |      Queue       |  Modular Design  |
|     Language     |   (Array Based)  |  Step-by-Step    |
+------------------+------------------+------------------+
Language: C
IDE/Compiler: GCC / Turbo C++
Data Structure: Queue (Array Implementation)
Concept: FIFO (First In First Out)
Data Structures Used
Queue (Array Implementation)

Each element in the queue stores:

┌────────────┬──────────────┬──────────────┬────────────┐
│ acc_no     │ name         │ type         │ amount     │
├────────────┼──────────────┼──────────────┼────────────┤
│ int        │ char[50]     │ char[10]     │ float      │
└────────────┴──────────────┴──────────────┴────────────┘
Key Concepts Applied

✅ Queue Operations — Enqueue, Dequeue, Display
✅ FIFO Principle — First In First Out processing
✅ Structures — struct customer and struct queue
✅ Condition Handling — Queue Full and Queue Empty
✅ String Handling — strcmp() for transaction type

Installation & Usage
Step 1: Save the Code

Save the file as:

banking_queue.c
Step 2: Compile the Code
gcc banking_queue.c -o banking
Step 3: Run the Program
./banking
Sample Output
Menu
1-Enqueue Transaction
2-Dequeue (Process)
3-Display
4-Exit
Enter choice:
Project Workflow
┌───────────────────────────────────────────────┐
│                   MENU                        │
│ 1. Enqueue   2. Dequeue   3. Display   4. Exit│
└───────────────────────────────────────────────┘
                      │
        ┌─────────────┼─────────────┐
        ▼             ▼             ▼
   ┌───────────┐ ┌────────────┐ ┌───────────┐
   │ ENQUEUE   │ │  DEQUEUE   │ │ DISPLAY   │
   │Transaction│ │ Processing │ │ Pending   │
   └─────┬─────┘ └─────┬──────┘ └─────┬─────┘
         │              │              │
         ▼              ▼              ▼
  ┌────────────┐ ┌────────────┐ ┌────────────┐
  │ Add to Rear│ │ Remove from│ │ Show All   │
  │ of Queue   │ │ Front      │ │ Transactions│
  └────────────┘ └────────────┘ └────────────┘
Learning Outcomes

Through this project, we have gained hands-on experience in:

Understanding and implementing Queue data structure
Applying FIFO concept in real-world scenarios
Working with structures and arrays in C
Handling edge cases like overflow and underflow
Writing modular and menu-driven programs
