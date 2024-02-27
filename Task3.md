By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command


sudo snap install leafpad**

![WhatsApp Image 2024-02-27 at 10 23 53_3f8db2f0](https://github.com/saad5738/Mohammed-Saad/assets/160725153/48f53b0f-c2f5-4fb4-85b9-71e0d5e73ec5)

**Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c&
![WhatsApp Image 2024-02-27 at 10 23 53_7ad0d7ab](https://github.com/saad5738/Mohammed-Saad/assets/160725153/7a7c1eb1-7fb8-4689-9177-18d10bd09006)
Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c
Step 5: Check the output by using the command

./a.out
The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c
![WhatsApp Image 2024-02-27 at 10 23 54_b0e8276f](https://github.com/saad5738/Mohammed-Saad/assets/160725153/869a3957-182a-4712-8820-779c636dd185)
Step 2: Compile the code in riscv using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![WhatsApp Image 2024-02-27 at 10 23 54_26ea6f5c](https://github.com/saad5738/Mohammed-Saad/assets/160725153/9fe51a5d-838a-4424-a869-1e6b086c0f7d)
Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command

ls -ltr sum1ton.c
![WhatsApp Image 2024-02-27 at 10 23 54_26ea6f5c](https://github.com/saad5738/Mohammed-Saad/assets/160725153/8c38d056-961f-41f5-818e-85ed789450c0)

![WhatsApp Image 2024-02-27 at 10 23 55_04a52b37](https://github.com/saad5738/Mohammed-Saad/assets/160725153/5e701b56-18e4-4947-8152-5946e237892b)
Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C exe
![WhatsApp Image 2024-02-27 at 11 10 48_f0abbdf6](https://github.com/saad5738/Mohammed-Saad/assets/160725153/48a3e5a2-8638-4e6d-bf9f-e57054c08fb3)


cution

![WhatsApp Image 2024-02-27 at 10 04 18_cfdc73d1](https://github.com/saad5738/Mohammed-Saad/assets/160725153/d29edabf-9c7a-40fe-b991-e5f67057b376)

Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![WhatsApp Image 2024-02-27 at 10 04 17_c2ea7991](https://github.com/saad5738/Mohammed-Saad/assets/160725153/d8b1282a-fb67-4fb1-9859-c57817d5de50)
![WhatsApp Image 2024-02-27 at 10 04 17_516bf5da](https://github.com/saad5738/Mohammed-Saad/assets/160725153/d9c18a0e-8e5c-4aef-b53f-7981b32c547c)

