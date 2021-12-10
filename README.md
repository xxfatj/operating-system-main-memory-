# operating-system-main-memory-

􏰀􏰔􏰕􏰖􏰃􏰄􏰗 􏰘 􏰏􏰕􏰇􏰂 􏰏􏰄􏰙􏰁􏰗􏰚

Stall: the need of the processer to stall. When completing a memory access may take many cycles of the CPU clock

Cache:  The remedy of adding fast memory between the CPU and main memory, typically on the CPU chip for fast access. 

 Base register: holds the smallest legal physical memory address; the limit register specifies the size of the range.

Binds: A compiler typically binds these symbolic addresses to relocatable addresses (such as “14 bytes from the beginning of this module”).

Relocatable code: .If it is not known at compile-time where the process will reside in memory, then the compiler must generate

Logical adresse: An address generated by the CPU is commonly referred to

Memory address register: referred to physical addressee

Virtual address.  What the physical address is referred to

Logical address space the set of all logical address is generated by a program

Physical address space the set of all physical addresses corresponding to these logical addresses

Memory management unit the runtime mapping from virtual to physical addresses is done by hardware called MMU

Relocation Register: the base register that is added to every ad dress generated by a user process

Dynamic loading we use it to obtain better memory space utilisation

Dynamically linked libraries our system library is linked to use your programs when the programs are running

Static linking system libraries are treated like any other object model and combined by ladder into the binary program image

Shared libraries is another way that dynamically linked libraries is known

Contagious memory allocation every process is contained in a single section of memory that is contagious to the section containing the next process

Variable partition scheme the operating system keep the table indicating which part of memory are available and which are occupied

Whole the available memory for the user processes that is considered as one large block of available memory

Dynamic storage Allocation problem: concern how to satisfy a require a request of size n from a list of free holes

First fit fit best fit and worst fit strategies are the one most commonly used to select free holes from set of available holes

External fragmentation both the first fit and the best fits strategies for memory allocation suffer from it

50% rule statistical analysis of first fit reveals that even with some optimisation given in allocated blocks another 0.5 in blocks will be lost to fragmentation that is one third of memory mightbe unusable

 Internal fragmentation is an  unused memory that is internal to a partition 

Compocition is one solution to the fragmentation problem

Paging A memory management scheme that permits and crosses physical address space to be non-contagious

Frames is a fixed sized lock that is break down into the physical memory as the basic method for implementing paging

Pages frames are breaking logical memory into blocks of the same size called pages

Page number: Is used as an index into fair process page table

 page offset

Huge pages is a page size and an architecture dependent large page size

Page table base rigester: is a single system of data structure that stores information

Translation lookaside buffer is a special small and fadt look up hardware cache that’s used as a standard solution for the problem that slows the memory access 

Translation lookaside buffer miss happens when a page number is not in there hence the address of the translation process can quickly find the next reference

Wire down: TLB entires for key kernel code are wired down. some translation lockable buffers that is allowing setting and to be wire down so they cannot be removed from the translation look up buffer

Add face identifier is an address stored in the translation look up for entry and address space identifier is a uniquely identifies every process and it is used to provide address space protection for the process 

Flushe: Is in a race entry from the translation look up buffer

Hit ratio is the percentage of time the page number of interest is found in the translation look up buffer

Valid invalid is an additional bits attached to each entry in the page table when it is set to be valid the associated page in the process of logical‘s space hence it is a valid   page. when the bit is set invalid the page is not in the process logical address

Page table and register is in the hardware provided by SunSystems to indicate the size of the page table

Rent friend code is the code that can be shared and compiled

Forward mapped scheme The actress translation method for the architecture of which the logical addresses are divided into a page number considering of 20 bits in the page office consisting of 12 bit the forward mad scheme addresses translation works from the outer page table inward. 

Page Table Is One Approach For Handling Addresses Spaces Larger than 32 Bits

Invented page table is a solution to solve the drawbacks problem

Sollair 64-bit with you pretty system are tightly integrated low overheads virtual memory that is running on
SPARC cpu

Translation look up walk is a functionality found in many modern cpus, that copies the entry of TSB into the translation look up buffer

Swapped the movement of the process or pro Prussian of process out of memory to a backing store and then brought back into the memory continued execution swapping makes it possible for the total physical address space of all processes excuse the real physical memory of the system

Page out is in operation moves pages from memory to packing store reverse the process is known as page in

Application stage before terminating a process and write it to flash memory so that it can be quickly restarted

Local descriptor table information about the first partition is kept on it

global descriptor table: Second partition of information is kept on it

Page directory is the high 10 order bits reference an entry in the outer  most page table

Page address extension is a software developers program that allows 32 bit to process to access physical address space larger than 4 GB

Page directory pointer table is the top two bits

X 86/64AMD 64 and Intel 64 processes

Itanium: is an Endo 74 bit architecture wasn’t widely adopted

Translation granules: Each of which reports different page size as well as larger section memory known as regions
