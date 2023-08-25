---
title: Class Info
layout: home
---

## Basic Information

- Lectures: TR 3:30-4:45pm, Derring Hall 3092
- Instructor: [Huaicheng Li](https://people.cs.vt.edu/~huaicheng),
  huaicheng@vt.edu
  - Office hours: Fridays 1-2pm, GP 4109
- TA: Jacqueline Bruen, jacquelineb@vt.edu
  - Office hours: Tuesdays 10-11am, GP 1st floor lobby by the stairs
- Online forum: Ed Discussion
  - Please turn on the notifications to avoid missing important course updates!

**Lecture attendance is mandatory**. Each student is allowed to miss three
lectures over the course of the semester; students missing more than three
lectures will not receive participation credit (15%) unless there is a
compelling reason for the absences.

Please ask questions.

### Three types of lectures

1. Lectures by the instructor, covering topics:
  - OS designs and principles
  - Storage: SSDs/HDDs, block layer, file systems
  - Memory: virtual memory, TLB, address translation, paging, protection,
    sharing
  - CPU: scheduling, process/threads, concurrency
  - Cloud infrastructure: virtualization, offloading, acceleration,
    disaggregation, new hardware/OS architecture.

2. Research paper discussion, presented by YOU
  - reading group: 4 members / group

3. Guest lectures: academic and industry talks
  - Recent research
  - Recent technology trends in industry


## Gradings (tentative)

- Participation: 15%
  - Class attendance is mandatory!
- Paper reviews + presentations: 15%, 5-10 papers
- Course project (open-ended): 50%
  - Proposal: 5%
  - Midterm report: 10%
  - Final presentation: 10% (demo video)
  - Final report: 25%
- Labs: 20% (semi open-ended, tentative, details TBA)
  - CloudLab setup + kernel compilation + measuring latency numbers
  - Reading, understanding and hacking Linux kernel source code (nvme, fs, net, etc.)
  - FEMU FTL: Mapping, Garbage Collection (GC), Wear Leveling (WL)
  - Linux page table walker (kernel module)
  - Bonus: FEMU enhancement, other new features! (Up to 10%)


## Reading Materials

No required textbooks for the class. The lectures are defined by the instructor
to focus on topics which are not fully covered by one specific textbook.
However, there are many great resources (books, online resources, etc.) I
recommend if you would like to go deeper in understanding and hacking OS.

### Textbooks

1. **OSTEP**, [Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/), by Remzi Arpaci-Dusseau and Andrea Arpaci-Dusseau, free OS textbook!

2. **OS:PP**, [Operating Systems: Principles and Practice (2nd edtion)](http://ospp.cs.washington.edu/), by Tom Anderson and Michael Dahlin 

3. [Linux Kernel Development (3rd edition)](https://www.amazon.com/Linux-Kernel-Development-Robert-Love/dp/0672329468), By Robert Love


### Linux Kernel Programming

There are tons of online materials talking about Linux kernel programming, see
below for some examples:

- The Linux Kernel [Source Code](https://github.com/torvalds/linux)
  - Why not?
- The Linux Kernel [Documentation](https://docs.kernel.org/)
- The Linux Kernel Module Programming [Guide](https://sysprog21.github.io/lkmpg/)
  - Free guide/book
- [Linux Kernel Programming, by Kaiwan N Billimoria](https://www.oreilly.com/library/view/linux-kernel-programming/9781789953435/)
  - VT students can access this book online for free, check instructions [here](https://ask.lib.vt.edu/faq/330720)

### Research Papers

- **TBA**

### Systems Programming

Systems programming skills are necessary for this course. If you would like to
sharpen your C/C++ systems programming skills in the UNIX/Linux environment,
the following books are worth reading:

- [Advanced Programming in the UNIX Environment (3rd edition)](https://learning.oreilly.com/library/view/advanced-programming-in/9780321638014/)

- [The Linux Programming Interface: A Linux and UNIX System Programming Handbook](https://man7.org/tlpi/)

### Writing OSes 

Interested in building an OS? See the exciting projects below:

- [Writing an OS in Rust](https://os.phil-opp.com/)

- [PintOS](https://pintos-os.org/), the [paper](https://benpfaff.org/papers/pintos.pdf), [code](https://pintos-os.org/cgi-bin/gitweb.cgi?p=pintos-anon;a=summary), by Stanford

- [Xv6, a simple Unix-like teaching operating system](https://pdos.csail.mit.edu/6.828/2023/xv6.html), by MIT
