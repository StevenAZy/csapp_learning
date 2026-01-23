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
  - When we speed up one part of a system, the effect on the overall system performance depends on both how significant this part was and how much it sped up.
$$\text{Speedup} = \frac{1}{(1 - \alpha) + \frac{\alpha}{k}}$$

- Concurrency and parallelism (do more, run faster)
  - Thread-level Concurrency
  - Instruction-level parallelism
  - Single-instruction, Multiple-data(SIMD) parallelism

- The importance of abstractions in computer system
  - Files(I/O devices), Virtual memory(Files + Main Memory), Instruction set architecture(Processor), Processes(Virtual memory + Instruction set architecture), Virtual machine(Processes + Operating system)

## 1.10 Summary

 -Refer to the book for more details.
