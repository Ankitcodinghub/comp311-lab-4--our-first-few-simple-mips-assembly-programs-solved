# comp311-lab-4--our-first-few-simple-mips-assembly-programs-solved
**TO GET THIS SOLUTION VISIT:** [Comp311 Lab 4- Our First Few Simple MIPS Assembly Programs! Solved](https://www.ankitcodinghub.com/product/comp311-our-first-few-simple-mips-assembly-programs-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;131813&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Comp311 Lab 4- Our First Few Simple MIPS Assembly Programs! Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
Next: Configure MARS

Enable pseudo-instructions: go to Settings then select Permit extended (pseudo) instructions and formats

Enable compact memory address layout: go to Settings-&gt;Memory Configuration and select Compact, Data at Address 0. then press the Apply and Close button.

Finally: Run the example assembly programs

In this repo you will see the following two example assembly files: Sum.asm and SumArray.asm

The bottom pane has two tabs:

MARS Messages shows errors or warnings during assembly Run I/O is the input/output.

Run each of the two programs. Make sure you understand every single line of code. Here is what to expect for each:

Sum.asm: Single-step through the program, and observe that the result (i.e., sum of numbers 0..4) will be in register $8 at the end of execution.

SumArray.asm: Single-step through it, and observe that the result (sum of 7, 8, 9, 10, and 8) will be in the sum variable (at data address 0x0 in the memory).

More Info

There are several library routines provided by MARS that an assembly program can use. These are called system calls, or syscall. These services include support for printing integers and strings (similar to the printf() function in C), reading integers and strings from the keyboard (similar to scanf() in C), memory allocation (similar to malloc() in C), exiting from a program (similar to return from main() in C), etc.

An assembly program accesses those services using the syscall command. There is only one syscall command for all these services, but which service is requested is determined by the values provided in certain registers. The value in register $v0 determines which service is requested, and often parameters are passed to the service using registers $a0, $a1, $a2 and $a3. If a value needs to be returned to the program (e.g., reading an integer from the keyboard), it is typically returned in register $v0.

For a full listing of system calls available in MARS, please refer to http://courses.missouristate.edu/kenvollmar/mars/help/syscallhelp.html. We will mostly be using system calls numbered 1 to 17.

For example, to exit a program, you would use syscall with 10 in $v0:

addi $v0, $0, 10 # system call 10 for exit syscall # exit the program

Part 1: Basic I/O and Arithmetic

You are given a program in MIPS assembly language that computes the area of a rectangle given the width and the height (ex1.asm). The width and height are read from the standard input after prompting the user, and then the program computes the area and prints it on the standard output. Here’s an example scenario:

Enter width (integer):

2

Enter height (integer):

4

Rectangle’s area is 8

Modify the program so that it also calculates and prints the perimeter (i.e., sum of all sides) of the rectangle. Thus, after modification, the example scenario would become:

Enter width (integer):

2

Enter height (integer):

4

Rectangle’s area is 8

Its perimeter is 12

Part 2: Loops

Create a new assembly file called “ex2.asm”.

Copy your final ex1.asm file to ex2.asm. Modify the program in ex2.asm to make it work on multiple inputs. In particular, it should repeatedly ask for width and height values, and print the corresponding area and perimeter, until the user enters the value 0 for width. At that point, the program should terminate. Here’s an execution scenario:

Enter width (integer):

2

Enter height (integer):

4

Rectangle’s area is 8

Its perimeter is 12

Enter width (integer):

5

Enter height (integer):

6

Rectangle’s area is 30 Its perimeter is 22

Enter width (integer):

0

Test your program in MARS, and once you are satisfied that it is working properly, commit your changes and submit to Gradescope to run the autograder.

Submit your assignment

Assignment submissions will be made through GradeScope.

1. Submit modifications using the commit Github Desktop instructions.

2. Update remote (origin) repository using the push Github Desktop instructions.

3. Go to the COMP 311 course in GradeScope and click on the assignment called Lab 04.

5. You should see a list of your public repositories. Select the one named lab-04-yourname and submit it.

6. Your assignment should be autograded within a few seconds and you will receive feedback.
