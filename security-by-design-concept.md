# Security by Design Challenge Concept

## Initial Ideas

* Iterative / multi-level tasks
* Level 1: Focus purely on functionality
  * Set a pin high (i.e., "open the door") after receiving a static identifier from the RFID transponder
  * Use Mifare Ultralight or a similar protocol without encryption or additional security measures
* Level 2: Use an encrypted protocol
  * Implement 3DES or AES to communicate with the transponder using one of the Mifare DESFire modes
* Level 3: Implement secure key storage
* Level 4: Implement (basic) protections against side-channel analysis
  * noise generators, dummy computations, shuffling, masking, ...
* Level 5: Implement (basic) protections against fault injection attacks
  * duplication, code-based error detection / correction, ...

***

* Teaching material matches the corresponding level and introduced the required concepts.
* Inexperienced as well as experienced teams are offered a challenge that is doable but still offers room to experiment and learn new things.
* Regardless of the final level a team reaches, they should analyze the possible weaknesses of their implementation, describe how any flaws could potentially be abused, what additional measures could be taken to avoid this. Furthermore, they should ideally write a brief developer guidance outlining any security-relevant aspects of their chip that need to be considered by users in order to achieve the expected security level.