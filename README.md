Some notes on specific aspects of line-rate (highest speed at any given point
in time) routers, which are typically implemented using dedicated hardware.
Here's a tentative list of topics.  There's no particular order or reason to
these topics.

0. Performance requirements for a line-rate router.
   Router evolution over time.

1. The architecture of a line-rate router: Why are routers architected as a pipeline?

2. Memory performance models.

3. Building multi-ported memories from single-ported memories.

4. Dictionaries in hardware and their implementations (hash tables, cuckoo hashing, d-left, CAMs)

5. TCAM implementations in hardware.

6. The partitioned Bloom Filter idea.

7. Using permutation networks in lieu of a multiplexer.

8. Some basics, required for building actual hardware.
    --> Writing hardware in Verilog.
    --> Using a silicon compiler like Synopsys DC.
    --> (maybe) writing hardware in Chisel.
    --> (maybe) formal verification of hardware.
