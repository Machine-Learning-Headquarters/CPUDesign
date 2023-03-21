# CPUDesign
What CPUs are powering the cluster



Will probably be built around a RISC-V instruction set, probably extended with custom instructions  

Will need to support inter cpu comminucation and inter cluster communication (Board communication will probably be a "front end" design. Turing Pi 2
uses a microcontroller, but depending on the bandwidth we may need another specialized CPU for interfacing).  

Untether has a hybrid CPU structure that strikes a midpoint between [In-Memory Processing](<https://en.wikipedia.org/wiki/In-memory_processing> "Wiki link")
 and classic Von Neumann architecture. There are multiple ALUs with individual access to RAM blocks. This is meant to reduce energy useage of memory transfer,
  which they claim as the majority of energy loss in CPU instructions.
