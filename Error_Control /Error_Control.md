## 10.1.1 Types of Errors
  - i) Single-bit error:
      - only 1 bit of a given data unit (such as a byte, character, or packet) is changed from 1 to 0 or from 0 to 1.
  - ii) Burst error:
      - 2 or more bits in the data unit have changed from 1 to 0 or from 0 to 1.

### Note: The number of bits affected depends on the data rate and duration of noise.
- Example: if we are sending data at 1 kbps, a noise of 1/100 second can affect 10 bits.

## 10.1.2 Redundancy 
- The central concept in detecting or correcting errors is redundancy.
- We(sender) send extra bits with the data to detect and correct corrupted bits.

## 10.1.3 Detction vs Correction
- i) Error Detection:
   -  Only cares about whether the error has occured or no. (i.e. Yes or No).
   - Not interested in the number of corrupted bits and their locations.
   - A single-bit error is the same here as a burst error.
     
- ii) Error Correction:
    - Bothers about the exact number of bits that are corrupted and,  their location in the message.
    - The number of errors and the size of the message are important factors.
