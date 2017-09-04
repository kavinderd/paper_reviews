# Review: 'Extensibility, Safety and Performance in the SPIN Operating System'

Authors: Bershad, Savage et al.
Institution: University of Washington

##Summary

###Motivation
The researchers felt there was a need for an OS that better met
the variable needs of different applications. They cite criticism from both
Database and Network application developers that experience poor performance in
traditional operating systems

- general purpose OS's can run everthing but don't run anything particularly well
- specialized OS's can run only a few program's well. 

Can SPIN be the best of both worlds?

###Contribution

The researchers contribute SPIN OS as an alternate OS architecture. SPIN OS is designed to provide the following:

- extensibilty: How flexible is the use of OS services
- safety: how well applications are protected from each other
- performance: comparable performance of applications compared to traditional OS designs

###Methodology
The researchers achieved their goal in SPIN OS by doing the following

1. Colocation of OS & extension services = low cost of communication
2. Modularity enforced by lang Modula-3: inherently provides boundaries between
modules at compile time
3. Logical Protection Domains: Namespaced units in the kernel that have a
limited exposed intrface. These domains are linked at runtime so inter-LPD
communication occurs at the cost of a procedure call
4. Dynamic Call Binding: An event handler that can dynamically bind events in
the OS to extensions. These are executed at the cost of a procedure call

Why modula-3?
3 aspects of the language were important in developing SPIN:
- interfaces: public & private methods that are enforced at compile-time
- strongly typed: no casting pointers of one kind to another at run time
- automatic storage management: Garbage collection, reference checks, etc

Open Questions: 
- How does the protection model in SPIN OS work?
- What are capabilities?
- What are protection domains in SPIN OS?
- How are OS extensions supported in SPIN OS?
- What are the core services provided by SPIN OS?
- How does SPIN handle memory management?
- How does SPIN handle thread management?

###Conclusion

Open Questions
- What are the conclusions the researchers make about SPIN OS?
- How does SPIN OS compare to other OS's

