# A tour of computer systems

## 1.1 Information is bits + context

- All information in a system is represented as a bunch of bits.

## 1.2 Programs are translated by other programs into different forms

- source program(hello.c) -[Preprocessor]-> Modified source program(hello.i) -[Compiler]-> Assembly program(hello.s) -[Assembler]-> Relocatable object programs(hello.o) -[Linker]-> Executable object program(hello)

## 1.3 It pays to understand how compilation system work

- Optimizing program performance.
- understanding link-time errors.
- Avoiding security holes.

## 1.4 Processor read and interpret instructions stored in memory

- Hardware: Buses, I/O devices, Main memory, Processor.

## 1.5 Caches matters

- Cache memories are smaller, faster, and serve as temporary staging areas for information that the processor is likely to need in the near future.
- CPU read speed: Register > L1 cache > L2 cache > main memory > disk
- main memory: dynamic random access memory (DRAM)
- L1/L2 cache: static random access memory (SRAM)

## 1.6 Storage device form a hierarchy

- Inserting a smaller, faster storage device between the processor and a larger, slower device is a general idea.

## 1.7 The operating system manages the Hardware

- Purposes of operating system
  1. Protecting the hardware from misuse by runaway applications.
  2. Providing applications with simple and uniform mechanisms for manipulating complicated and often wildly different low-level hardware devices.
- The operating system achieves both goals via the fundamental abstractions: processes, virtual memory, and files.
- The operating system perform this interleaving with a mechanism known as **context switching**.

## 1.8 Systems communicate with other systems using networks

- Network can be viewed as just another I/O device.

## 1.9 Import themes

- Amdahl's law
$$\text{Speedup} = \frac{1}{(1 - \alpha) + \frac{\alpha}{k}}$$
