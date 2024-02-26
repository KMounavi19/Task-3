By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad** 
![WhatsApp Image 2024-02-26 at 9 44 10 PM](https://github.com/KMounavi19/Task-3/assets/160726381/7989a7d5-4177-4d80-ad79-ab19c4c7be85)
*Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c&
![WhatsApp Image 2024-02-26 at 9 46 44 PM](https://github.com/KMounavi19/Task-3/assets/160726381/a9c231f8-04dc-48e1-a341-32b73f46783f)
Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c
![WhatsApp Image 2024-02-26 at 9 48 53 PM](https://github.com/KMounavi19/Task-3/assets/160726381/0e6068f1-4710-4148-bcf7-65ba5fd01a4f)
Step 5: Check the output by using the command

./a.out
![WhatsApp Image 2024-02-26 at 9 52 06 PM](https://github.com/KMounavi19/Task-3/assets/160726381/6c82fbe2-66d9-4df9-95bb-3f1539b25591)
The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c 
![WhatsApp Image 2024-02-26 at 9 57 21 PM](https://github.com/KMounavi19/Task-3/assets/160726381/1434443a-b2fd-477a-982d-f2f7b384b7a5)

Step 2: Compile the code in riscv using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![WhatsApp Image 2024-02-26 at 9 54 02 PM](https://github.com/KMounavi19/Task-3/assets/160726381/c6c6e088-8950-4f09-8f40-2d6469f5bb21)
Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command

ls -ltr sum1ton.c
![WhatsApp Image 2024-02-26 at 10 03 26 PM](https://github.com/KMounavi19/Task-3/assets/160726381/f1584a07-085d-4db9-a2d2-dd5da56a9204)
![WhatsApp Image 2024-02-26 at 10 07 55 PM](https://github.com/KMounavi19/Task-3/assets/160726381/4b5fb130-f33d-40e0-9b11-b6586767724e)
Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution
![WhatsApp Image 2024-02-26 at 10 09 38 PM](https://github.com/KMounavi19/Task-3/assets/160726381/5af2d0c5-88e3-4391-abf5-ca51e0b00631)
![WhatsApp Image 2024-02-26 at 10 10 45 PM](https://github.com/KMounavi19/Task-3/assets/160726381/12be47e5-c3d9-44b7-a10f-c1fd216c560b)
Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![WhatsApp Image 2024-02-26 at 10 12 58 PM](https://github.com/KMounavi19/Task-3/assets/160726381/c64beea0-9e83-42be-913f-a0181afd7e49)
![WhatsApp Image 2024-02-26 at 10 13 28 PM](https://github.com/KMounavi19/Task-3/assets/160726381/bf9c212f-aef1-46ae-8313-10f27b29fabb)

