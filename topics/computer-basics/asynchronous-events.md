
## Asynchronous Events: Polling Loops and Interrupts

### Hard Disk Drive (HDD) and Solid State Drive (SSD)

- HDD has moving parts - a spinning magnetic disk. This reduces longevity and speed.
- SDD is fully electronic making it faster and more efficient.
- Both are forms of permanent storage, meaning data is not lost when powered down.

### Keyboard and Mouse

- Devices for user input.
- Allows for interaction with programs and files.

### Monitor and Printer

- Displays computer output.

### Audio Output Device (Speakers)

- Outputs sounds produced by a computer.

### Network Interface

- Allows for communication between computers.

### Scanner

- Converts images into binary numbers for use on a computer such as display, manipulation, etc.

### Device Driver

- Software translated to machine language and executed by the CPU to allow the computer to communicate and interact with the various devices connected (such as the aforementioned).

### Busses

- A set of wires carrying information between devices.
- Carries data, addresses, and control signals.

### Control Signals

- Used by one device to alert another that data is available for it on the bus.

### Diagram of Interaction Between Computer, Devices, and Busses

![Simple Computer System Diagram](/images/simple-computer-system.jpg)

### Polling

- An inefficient solution to solve how a CPU is able to tell how incoming data is ready for processing.
- The computer constantly scans all input devices and processes information as it is made available.
- Wastes time that could be used more productively.

### Interrupts

- A more efficien solution to the aforementioned problem.
- A signal is sent by the input device once data is available for processing. When received, the CPU is immediately stops it current task to respond before continuing.

#### How do Interrupt Signals Work?

- Mechanically.
- The signal activates a wire that the CPU is set up to respond to by immediately storing its current task to respond to.

### Interrupt Handler

- Part of the Device Driver Software.
- Stores instructions for the CPU to execute in response to the signal.
- Instructs CPU to resume its previous task once the signal is dealt with.

### Asynchronous Events

- Events that happen unpredictably; outside of the synchronous fetch and execute cycle.
- Dealt with via interrupts.

#### Example: Starting a Program

1. CPU sends signal to HDD/SSD requesting data be sent to RAM in order to execute a program.
2. HDD/SSD is very slow compared to CPU, so while this data is being uploaded to RAM the CPU continues with whatever other tasks is has to accomplish.
3. Once data is fully loaded to RAM, HDD/SSD sends an interrupt signal to CPU causing it to pause its current task to execute the uploaded data.
4. CPU then fetches and executes uploaded data via Interrupt Handler.

### Multitasking

- Performing multiple tasks at once.

### Timesharing

- A timesharing computer is one that allows multiple users to be using the same computer at the same time.
- The computer quickly swaps its attention between each user's inputs and tasks to complete them all simultaneously.

### Threads

- An individual task a CPU is working on.
- Each core in a CPU can run a thread, therefore CPUs with multiple cores are able to multitask efficiently.
- The amount of threads that can be worked on are limited, and so efficient multitasking is a problem currently dealt with via different means.

### Yielding

- When a thread voluntarily allows another to run.

### Blocked Thread

- A thread is considered blocked when it needs to wait for an asynchronous event (such as user input) to proceed.

### Preemptive Multitasking

- When a computer suspends a thread to allow others to run via a special timer device.
- Timer device generates an interrupt signal at regular time intervals (example: 100 times per second) to allow quick swapping between tasks, similar to a timesharing computer swapping between users.
- All modern computers utilise this as a solution to the limited amount of threads that can be worked on at once.

###### Sources:

Eck, D. J. (2022). *Introduction to Programming Using Java Version 9, JavaFX Edition.* Hobart and William Smith Colleges.

Available [here](https://math.hws.edu/javanotes/?fbclid=IwAR3V0pxqmqNeSpasvbbVrx-RAylNmYW7yYnD2q8-1nJMHErQxynK27MNOhw)