# SECR2043 Operating Systems — Reflection
---

## Lab Assessment 1 — Basic Linux Commands & C Programming

Lab Assessment 1 gave me a solid foundation in navigating the Linux environment from the command line. Working through basic file operations like `pwd`, `ls`, `mkdir`, `cp`, `mv`, and `rm` felt straightforward at first, but combining them with Activity 2's text manipulation using `echo`, `cat`, and `nano` made me realise how powerful even simple commands can be when chained together. Activity 3 pushed me further by introducing the full write-compile-run cycle in C using `gcc`, and writing programs like `sum.c` and `echo.c` helped me connect low-level programming to the OS environment. Overall, this assessment built my confidence in working directly with the Linux terminal, which became essential groundwork for everything that followed.

---

## Lab Assessment 2 — Process Monitoring and Management

This assessment gave me hands-on experience with how an operating system manages running processes, which I had previously only understood theoretically. Using `ps` with various flags, `pstree`, `grep`, and `renice` to inspect and manipulate the dummy `mainprocess`, `subprocess1`, and `subprocess2` processes made the concepts of PIDs, PPIDs, process hierarchy, and priority scheduling feel very concrete. The most interesting part was Question 10, where I wrote a C program using `fork()` and `wait()` to demonstrate parent-child process creation — seeing the child PID print before the parent confirmed message really clicked the concept into place for me. This lab showed me that process management is not just a background OS function but something a developer can directly observe and control.

---

## Lab Assessment 3 — File Management & Bash Scripting

Lab 3 shifted focus from individual commands to writing reusable bash scripts, which felt like a meaningful step up in complexity. Creating the directory and file tree from a shell script (`yasmin.sh`) taught me how to string together multiple commands programmatically, and building the interactive file extension counter (`file_extension.sh`) introduced me to reading user input and using `find` with `wc` inside a script. The second half of the lab, dealing with `chmod` permissions, was particularly valuable — translating the permission table into octal values and verifying the results with `ls -ld` made the read/write/execute model much clearer than any lecture slide could. Writing `myname2a.sh` and `myname2c.sh` together showed me how scripting and permission management work hand in hand in real system administration tasks.

---

## Group Project — Paging Concept Visualization (Group Quadratech)

The group project was a rewarding exercise in bridging an abstract OS concept with a real-world analogy. By mapping paging to a hospital scenario — where patients are processes, general wards are virtual memory pages, and ICU rooms are physical memory frames — our team made the mechanics of the page table, frame allocation, and internal fragmentation genuinely intuitive. Implementing the simulation in Python reinforced the theoretical understanding by forcing us to think concretely about data structures and allocation logic. Seeing the output show 3 beds of total internal fragmentation across ICU rooms made the cost of fixed-size frames tangible in a way that a textbook example rarely does. This project also strengthened my appreciation for collaborative work, as dividing the design, implementation, and documentation phases across the team required clear communication and coordination.

---

## Overall Reflection

Looking back across all three lab assessments and the group project, the SECR2043 Operating Systems course gave me a much deeper appreciation for the layer of software that sits between hardware and applications. I started the semester seeing the OS as a black box, but through hands-on practice I came to understand it as a set of carefully designed mechanisms — file systems, process schedulers, memory managers — each with real trade-offs. The progression from basic Linux commands to bash scripting to process management and finally to memory concepts felt well-scaffolded, and the project gave me the opportunity to consolidate everything into something creative and communicable. The skills I picked up here, particularly comfort with the Linux command line and systems-level thinking, are ones I expect to carry forward into future data engineering and software work.
