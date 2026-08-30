## Professor Answer Key — do not hand out this section

Accept any reasonable, well-explained answer. Multiple OS jobs are
often defensible; the goal is reasoning, not a single "correct" pick.

### Part A

1. **CPU time.** The scheduler gives each app short time slices, so
   both feel active at once.
2. **Memory.** Each process has its own private memory space, so one
   crash does not spread to others.
3. **CPU time** (priority for the call's audio requests) or **Device**
   (the disk driver serving the download). Both are defensible.
4. **Device.** A new printer needs a device driver before the OS can
   talk to it.
5. **CPU time** (more processes competing for turns) or **Memory**
   (each tab uses its own memory space). Both are defensible.
6. **Memory.** Private memory spaces stop one app from reading
   another app's data, which protects saved passwords too.

### Part B

1. **CPU time** (most likely, a whole-machine problem, not one
   process's private memory) — accept **Device** if a shared driver
   is blamed instead.
2. **CPU time.** Idle or lightly-used apps get very short, infrequent
   time slices, so they barely affect anything.
3. **Device.** The mouse needs its driver working correctly to
   communicate with the OS.
4. **Memory.** Each window (process) keeps its own separate memory
   space; one closing does not touch the other's data.
5. **Device** (both compete for the same disk/network driver) or
   **CPU time** (the download's requests crowd out the call's).
   Both are defensible.
6. **CPU time.** The scheduler gives idle processes very little time,
   since they are not asking to do anything.
