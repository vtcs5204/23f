---
title: Labs
layout: home
---

----

Please work on the labs by yourself!


### Lab 0 

#### 0. Fill out the Google Form to submit your Github account info

We will use Github classroom for lab submissions. We need your github IDs to
add you to the classroom. Please fill out the
[form](https://forms.gle/yvF9dwU4Ci63D4Gv8), the form will close on **8/28/2023
at 11:55pm**. Please work on it ASAP.

We will add you to the Github Classroom account by the end of Tuesday
(8/29/2023). Afterwards, please accept the assignment (i.e., Lab 0) on Github
Classroom using this [link](https://classroom.github.com/a/QKlNWKiA). You will
have a separate repo for you to submit codes/results.


#### 1. Apply for a Cloudlab account

Apply for an account using the [signup link](https://cloudlab.us/signup.php).
On the "Person Information" panel, click "Join Existing Project" and fill in
our project name ``vtcs5204``. Please use your @vt.edu email address. Your
application will be approved by us shortly. Setting up the experiment
environment in Cloudlab.

We are going to use ``c220g5`` machines equipped with 2 x 10-core Intel Skylake
CPUs, 192GB ECC Memory and One Intel DC S3500 480 GB 6G SATA SSD. You can find
the detailed hardware description and how the machines are interconnected
[here](https://docs.cloudlab.us/hardware.html) and current availability
[here](https://www.cloudlab.us/resinfo.php). 

Note that you can only reserve CloudLab servers for a limited amount of time
(lease can be extended if servers are available). But please start the lab
early to avoid missing the deadline due to the availability issue.


#### A2. Compile and install Linux kernel on CloudLab

- Get Linux kernel source from github [here](https://github.com/torvalds/linux)
- Switch to tag "v6.4"
- Change kernel config file to ensure the kernel name includes **your 9-digit
  VT PID and last name** in the kernel name, i.e., kernel name should end with
  "${YourPID}-${YourLastName}". ${YourPID} refers to your PID, e.g., 123456789
  and ${YourLastName} is your last name, e.g., "ABCD". Then the kernel name
  should end with "123456789-ABCD". If your kernel is installed successfully,
  after you login, the output of ``uname -a`` should contain have
  "123456789-ABCD" in it.
- Compile and install the Linux kernel using default options
- Change grub to reboot the machine using your compiled kernel
- Double check ``uname -a`` shows that you're using your compiled Linux kernel
  v6.4. 
- Use tools like ``asciinema`` to record a video which showcases you type in
  ``uname -a`` and ``cat /proc/cmdline`` in the shell and it outputs a string
  with your PID and LastName. Please put the link to your asciinema demo in a
  markdown file named "linux-kernel-demo.md".


#### A3. Write a **C** program to measure L1, L2, L3, DRAM, and SSD performance

Your C program should report the following
results:

- L1 cache size and latencies for 64B load/store access (in nanoseconds)
- L2 cache size and latencies for 64B load/store access (in nanoseconds)
- L3 cache size and latencies for 64B load/store access (in nanoseconds)
- DRAM latencies for 64B load/store accesses (in nanoseconds)
- A brief report (name it as "cache-results.md") explaining the approach you
  used to measure the above metrics.  Reason about the correctness of your
  measured results.

Requirements:

- Your C program must be named as "memlat.c"
- Write a "Makefile" for it (by typing "make", it should resolve all the
  dependencies and compile the binary to "memlat")

Hints: Check Figure 1 of this
[paper](https://lmbench.sourceforge.net/lmbench-usenix.pdf). Your program needs
to report results in a similar style.

#### A4. Measure the SSD write bandwidth

Please use [FIO](https://github.com/axboe/fio) and steady-state configuration
[here](https://github.com/axboe/fio/blob/master/examples/ssd-steadystate.fio)
to measure SSD's write bandwith. Note you need to change ``filename=/dev/fioa``
to point to the SSD block device (Intel DC S3500 480 GB). Using the collected
bandwidth results, plot a graph where:

- X-axis is time (in seconds)
- Y-axis is write bandwidth in MB/s
- The title of the graph should be "S3500-Bandwidth ${PID} ${LastName}", replace
  ${LastName} with your last name and ${PID} with your VT PID
- Caption: describe and explain the trend of bandwidth changes you observed
- Save the graph with all the above information as "ssd-bw.pdf" 


#### 5. Submission

Please submit the following files for tasks A2-A4 to your personalized Lab0 repo, with

- A2: "linux-kernel-demo.md"
- A3: "memlat.c", "Makefile", "cache-results.md"
- A4: "ssd-bw.pdf"

**The submission deadline is Aug 31, 2023, 15:30 EDT.** You won't be able to
push to the repo after the deadline.

----

### Lab 1

TBA

### Lab 2

TBA

### Lab 3

TBA
