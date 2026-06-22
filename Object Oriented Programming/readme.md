# 📓 Personal Reflection — Object Oriented Programming (SECJ2154)
---

## Lab Exercise — Patient & Hospital Classes

This lab exercise introduced me to the fundamentals of class design in Java through a simple hospital payment system, where a `Patient` class with private fields and public methods was created alongside a `Hospital` driver class. Implementing `updatePaymentAmount()` and `copyPayment()` as separate methods — rather than directly manipulating fields — made the concept of encapsulation feel concrete and purposeful for the first time: the data is protected, and all changes go through controlled channels. Overriding `toString()` to produce a clean, readable output also reinforced how even small design decisions in a class affect how easy it is to work with later.

---

## Project Proposal — Staff Attendance Application

Putting together the project proposal required us to think through the system's structure before writing a single line of code, which was a more useful exercise than it initially seemed. Designing the class diagram in draw.io — with an abstract `Staff` class, `FullTimeStaff` and `PartTimeStaff` subclasses, a `ClockIn` interface, and an `AttendanceRecord` utility class — forced us to decide early on which responsibilities belonged where, and why inheritance made more sense than duplicating clock-in logic across two separate unrelated classes. Listing the OOP concepts we planned to use (inheritance, abstraction, polymorphism, interfaces, exception handling, file handling) in the proposal also held us accountable to actually applying them in the final build.

---

## Project — Staff Attendance Application

Building the Staff Attendance Application brought together nearly every OOP concept covered in the course into one working system. The abstract `Staff` class with its `markAttendance()` and `calculateWorkingHours()` abstract methods meant that `FullTimeStaff` (8 hours base) and `PartTimeStaff` (4 hours base) each provided their own implementation without duplicating shared logic like timestamp generation or the `toString()` format. What I found most instructive was the exception handling in `MainApp` — validating that staff IDs are alphanumeric, names contain only letters and spaces, staff type inputs are strictly `yes` or `no`, and OT hours are non-negative — because it made me think about all the ways a user could break the system and how to handle each case gracefully rather than letting the program crash. The `AttendanceRecord` class writing to `attendance.txt` in append mode also gave me a first real experience with persistent file I/O, including the importance of closing the `FileWriter` properly to avoid data loss.

---

## Overall Reflection

This course shifted how I think about writing code — from writing instructions that work, to designing structures that are maintainable and extensible. The progression from the lab exercise (a two-class encapsulation example) to the full project (six classes, an interface, file I/O, and exception handling working together) made each concept feel earned rather than abstract. The part I want to keep building on is the design phase: the proposal's class diagram saved us significant rework during implementation because the responsibilities of each class were already settled. Going forward, I want to make that kind of upfront structural thinking a habit rather than something that only happens when it is required as a deliverable.

---

*Submitted for SECJ2154 — Object Oriented Programming*
