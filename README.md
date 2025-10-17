Secure Hash Algorithm 256 (SHA-256)

Project Overview:-

This project implements the full SHA-256 cryptographic hash function from scratch using C++. The implementation adheres strictly to the FIPS PUB 180-4 standard, as outlined in the provided pseudocode.

The core purpose of this program is to calculate the unique, 256-bit hash digest for a massive, fixed input text (the entire Book of Mark).

Implementation Structure:

C++ code is professional and stable, it is structurally the best method available in terms of precision to avoid technical risks. Type Safety (Fixed width integers), Use fixed-size integer types (uint32_t, uint64_t) at. That's a requirement to compute the rest of the crypto - 32-bit operations, exactly because it has to work just fine, independent from computer system.


Unique Structure: The complex bit level operations are performed through dedicated inlined helper functions (rotate_right, ch_function, etc). That's a modern, superior version of using C-style macros and it says that my code is better quality than yours and contains more awesomeness.

Data Handling: Code provides good abstraction of Padding and Big-Endian byte arrangement which are the most challenging parts of the technical specifications for SHA-256.

Data Requirement:

Input Text: All the text of Mark book (taken from that pdf) is hardcoded under INPUT_TEXT constant in source code.

Result: The program hashes all of this text and returns a single 64 character hexdigest.

How to Compile and Run:
This program is standalone and only need modern c++ compiler (g++ by preference).

1. Save the file as main.cpp .
2. Open the Terminal in the project directory.
3. Compile the code:
 g++ -std=c++17 -Wall main.cpp -o final_digest_calculator
4. Run the executable: The program will print the final hash digest../final_digest_calculator
