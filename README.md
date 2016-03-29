Some notes on specific aspects of line-rate (highest speed at any given point
in time) routers, which are typically implemented using dedicated hardware.
Here's a tentative list of topics.  There's no particular order or reason to
these topics.

0. Performance requirements for a line-rate router.
   Router evolution over time.

1. Motivating the match-action or lookup model of routers.

2. The architecture of a line-rate router: Why are routers architected as a pipeline?

3. Memory performance models.

4. Why bypassing or operand forwarding doesn't work at line rate?

5. Building multi-ported memories from single-ported memories.

6. Dictionaries in hardware and their implementations (hash tables, cuckoo hashing, d-left, CAMs)

7. Dictionaries with inserts and deletes in the data-plane
   * MAC learning
   * d-left hash tables used for caching

7. TCAM implementations in hardware.

8. The partitioned Bloom Filter idea.

9. Using permutation networks in lieu of a multiplexer.

10. Some basics, required for building actual hardware.
    * Writing hardware in Verilog.
    * Using a silicon compiler like Synopsys DC.
    * (maybe) writing hardware in Chisel.
    * (maybe) formal verification of hardware.
