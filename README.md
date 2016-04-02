Some notes on specific aspects of line-rate (highest speed at any given point
in time) routers, which are typically implemented using dedicated hardware.
Here's a tentative list of topics.  There's no particular order or reason to
these topics.

0. Performance requirements for a line-rate router.
   Router evolution over time.

1. Motivating the match-action or lookup model of routers.

2. The architecture of a line-rate router: Why are routers architected as a pipeline?
   (this is the area and power argument)

3. The cost of a line-rate router: Why is the pipeline model in silicon more
   effective than throwing an array of processors at the problem.

4. Memory performance models.

5. Why bypassing or operand forwarding doesn't work at line rate?

6. Building multi-ported memories from single-ported memories.

7. Dictionaries in hardware and their implementations (hash tables, cuckoo hashing, d-left, CAMs)

8. Dictionaries with inserts and deletes in the data-plane
   * MAC learning
   * d-left hash tables used for caching

9. TCAM implementations in hardware.

10. The partitioned Bloom Filter idea.

11. Using permutation networks in lieu of a multiplexer.

12. Some basics, required for building actual hardware.
    * Writing hardware in Verilog.
    * Using a silicon compiler like Synopsys DC.
    * (maybe) writing hardware in Chisel.
    * (maybe) formal verification of hardware.
