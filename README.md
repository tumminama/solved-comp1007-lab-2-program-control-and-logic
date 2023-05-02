Download Link: https://assignmentchef.com/product/solved-comp1007-lab-2-program-control-and-logic
<br>
Operators are used to perform operations on variables and values. Python has many operators for different purposes. The following are the commonly used operators.

Assignment Operator

We have already used the assignment operator =, which assigns the value of the right side operand to the left side variable. E.g.,

name = “Jack” grade = 95

Arithmetic Operators

Arithmetic operators are used for performing mathematical operations. The following table shows the operators with some examples:

<strong>Name                                                      Operator                                             Example</strong>

<table width="0">

 <tbody>

  <tr>

   <td width="197">Addition</td>

   <td width="188">+</td>

   <td width="181">&gt;&gt;&gt; 10 + 212</td>

  </tr>

  <tr>

   <td width="197">Subtraction</td>

   <td width="188">‐</td>

   <td width="181">&gt;&gt;&gt; 10 – 28</td>

  </tr>

  <tr>

   <td width="197">Multiplication</td>

   <td width="188">*</td>

   <td width="181">&gt;&gt;&gt; 10 * 220</td>

  </tr>

  <tr>

   <td width="197">Division</td>

   <td width="188">/</td>

   <td width="181">&gt;&gt;&gt; 10 / 25.0</td>

  </tr>

  <tr>

   <td width="197">Modulus</td>

   <td width="188">%</td>

   <td width="181">&gt;&gt;&gt; 5 % 32</td>

  </tr>

  <tr>

   <td width="197">Exponentiation</td>

   <td width="188">**</td>

   <td width="181">&gt;&gt;&gt; 10 ** 2100</td>

  </tr>

  <tr>

   <td width="197">Floor division</td>

   <td width="188">//</td>

   <td width="181">&gt;&gt;&gt; 5 // 31</td>

  </tr>

 </tbody>

</table>




<strong><em>Note: </em></strong><em>An arithmetic <strong><u>expression</u></strong> can be constructed by using multiple arithmetic operators and parentheses. </em>

It is very common to assign an expression to a variable. E.g.,

PI = 3.14159

Radius = 6378

Perimeter = 2 * PI * Radius

print(“The perimeter of earth is ” + str(Perimeter)) Volume = 4/3 * PI * Radius ** 3

print(“The volume of earth is {}”.format(Volume))

Remark: The expression <strong><u>4/3 * PI * Radius ** 3</u></strong> is equivalent to <strong><u>4/3 * PI * (Radius ** 3)</u></strong> because ** has a higher priority (or precedence) than * and /. Now you can use Python as a calculator!

<h2>Comparison Operators (also called Relational Operators)</h2>

Comparison operators are used for comparing two values, and the value of a comparison expression is either True or False. The following table shows the operators with the examples:

<strong>Name                                                     Operator                                             Example</strong>

<table width="0">

 <tbody>

  <tr>

   <td width="195">Equal</td>

   <td width="189">==</td>

   <td width="182">&gt;&gt;&gt; x = 1&gt;&gt;&gt; x == 1True&gt;&gt;&gt; x == 2False</td>

  </tr>

 </tbody>

</table>

&gt;&gt;&gt; x = 1

&gt;&gt;&gt; x != 1

<table width="0">

 <tbody>

  <tr>

   <td width="195">Not Equal</td>

   <td width="189">!=</td>

   <td width="182">False&gt;&gt;&gt; x != 2True</td>

  </tr>

  <tr>

   <td width="195">Greater than</td>

   <td width="189">&gt;</td>

   <td width="182">&gt;&gt;&gt; x = 1&gt;&gt;&gt; x &gt; 1False</td>

  </tr>

  <tr>

   <td width="195">Greater than or equal to</td>

   <td width="189">&gt;=</td>

   <td width="182">&gt;&gt;&gt; x = 1&gt;&gt;&gt; x &gt;= 1True</td>

  </tr>

  <tr>

   <td width="195">Less than</td>

   <td width="189">&lt;</td>

   <td width="182">&gt;&gt;&gt; x = 1&gt;&gt;&gt; x &lt; 1False</td>

  </tr>

 </tbody>

</table>

&gt;&gt;&gt; x = 1

Less than or equal to                          &lt;=                                                          &gt;&gt;&gt; x &lt;= 1

True




<h2>Logical Operators</h2>

Logical operators are used for combining the conditional statements. The following table shows the operators and the examples:

<strong>Operator                   Description                                                                   Example</strong>

<table width="0">

 <tbody>

  <tr>

   <td width="113">and</td>

   <td width="267">If both operands are True, then the result is True. Otherwise, the result if False.</td>

   <td width="189">&gt;&gt;&gt; x = 5&gt;&gt;&gt; x &lt; 10 and x &gt; 3True</td>

  </tr>

  <tr>

   <td width="113">or</td>

   <td width="267">If both operands are False, then the result if False. Otherwise, the result if True.</td>

   <td width="189">&gt;&gt;&gt; x = 5&gt;&gt;&gt; x == 1 or x == 5True</td>

  </tr>

  <tr>

   <td width="113">not</td>

   <td width="267">The result is the reverse of the operand.</td>

   <td width="189">&gt;&gt;&gt; x = 5&gt;&gt;&gt; not x &gt; 10True</td>

  </tr>

 </tbody>

</table>










<h1>Control Statements</h1>

The most direct way to affect the flow of control is with a conditional statement. In Python, the main types of control statements are <em>if</em>, <em>while</em> and <em>for</em>. <em>if, if…else, if…elif…else</em> statements

The <em>if</em> statement performs an indicated action only when the condition is true; otherwise the action is skipped. The syntax is:

<em>if expression: </em>

<em>       statement </em>

Remark: the colon : at the end of if statement in very important. It indicates that the following block of statements with the same amount of indentation will be executed if the expression is true.

Let’s try the following example.

score = input(‘Please input the score: ‘) score = float(score)




if score &gt;= 50:

print(‘Congratulations!’)

print(‘You passed the course!’)




With the <em>else</em> clause (<em>if…else</em> statement), it allows you to specify that different actions are to be performed when the condition is false. The syntax is:

<em>if expression: </em>

<em>      statement(s) 1 </em>

<em>else: </em>

<em>      statement(s) 2 </em>




Try the following example.

<table width="0">

 <tbody>

  <tr>

   <td width="566">score = input(‘Please input the score: ‘) score = float(score)if score &gt;= 50:     print(‘PASS’)print(‘Congratulations!’) else:print(‘FAIL’)print(‘Please work harder!’)</td>

  </tr>

 </tbody>

</table>




The <em>if…elif…else</em> statement is used for multiple cases by placing the <em>elif</em> with conditions. The syntax is:

<em>if expression 1: </em>

<em>      statement(s) 1 elif expression 2:        statement(s) 2 elif … </em>

<em>       … </em>

<em>else </em>

<em>      statement(s) N</em>




For example, the following code will print different grades based on the score.

<table width="0">

 <tbody>

  <tr>

   <td width="566">score = input(‘Please input the score: ‘) score = float(score)if score &gt;= 85:     print(‘A’) elif score &gt;= 75:     print(‘B’) elif score &gt;= 65:     print(‘C’) elif score &gt;= 50:     print(‘D’) else:print(‘F’)</td>

  </tr>

 </tbody>

</table>




<h2><em>while</em> statement</h2>

The <em>while</em> statement is used to execute a block of statements repeatedly while some condition remains true. The syntax is:

<em>while expression: </em>

<em>      statement(s)</em>




Consider the following example code that prints the numbers from 1 to 10.

<table width="0">

 <tbody>

  <tr>

   <td width="566">i = 1  while i &lt;= 10:     print(i)i = i+1print(i)</td>

  </tr>

 </tbody>

</table>




The initial value of the variable <em>i</em> is 1. In the body of the while statement, <em>i</em> is printed and increased by

<ol>

 <li>The loop runs total 10 times while <em>i</em> iterates from 1 to 10. Notice that after the while loop, i becomes 11.</li>

</ol>

Try another example that uses while to implement a guess game:

answer = “Jack”

print(“======Can you guess my name?======”) guess = “”

while guess != answer:

guess = input(“Guess my name: “) print(“Bingo!”)




<em>                </em><em> </em>

<h2><em>for</em> statement</h2>

The <em>for</em> statement is used for iterating over a sequence. With the <em>for</em> statement, we can execute a block of statements, once for each item in the sequence (such as a list, tuple, range, and dictionary). The syntax is:




<em>for iterating_var in sequence:</em>

<em>      statement(s) </em>







Consider the following example code that prints the day names. The items in the list will be assigned to the iterating variable <em>d</em> one‐by‐one.

<table width="0">

 <tbody>

  <tr>

   <td width="566">days = [‘Monday’, ‘Tuesday’, ‘Wednesday’, ‘Thursday’, ‘Friday’, ‘Saturday’,‘Sunday’] for d in days:     print(d)</td>

  </tr>

 </tbody>

</table>




It is also very common to use the built‐in function <strong>range()</strong> to generate an immutable sequence and then iterate through a sequence. For example:

<table width="0">

 <tbody>

  <tr>

   <td width="566">days = [‘Monday’, ‘Tuesday’, ‘Wednesday’, ‘Thursday’, ‘Friday’, ‘Saturday’,‘Sunday’] for i in range(7):     print(days[i])</td>

  </tr>

 </tbody>

</table>




<h2><em>break </em>and <em>continue</em> statements</h2>

The <em>break</em> and <em>continue</em> statements are used to alter the flow of control when executed in a <em>while</em> or <em>for</em> statement.

The <em>break</em> statement causes an immediate exit from that statement. Therefore, the <em>break</em> statement is used to escape early from a loop.

Try the following code:

<table width="0">

 <tbody>

  <tr>

   <td width="303"> #%%1         for i in range(1, 10):2         if i &gt; 3: 3         break4         print(i)5         print(‘Broke out at x = {}’.format(i))</td>

  </tr>

 </tbody>

</table>

<table width="0">

 <tbody>

  <tr>

   <td width="154">123Broke out at x =  4</td>

  </tr>

 </tbody>

</table>

<em>Output:</em>




Remark: In the previous example, lines 2‐4 are the statements of the for loop and they are indented by four spaces. Line 3, the break statement, is under the if statement; so it has another level of indentation of four spaces.

The <em>continue</em> statement skips the remaining statements in the body of that control statement and evaluate the condition immediately (<em>while</em> loop) or performs the next iteration (<em>for</em> loop).  Try the following code:

<table width="0">

 <tbody>

  <tr>

   <td width="282">#%% i = 0  while i &lt; 6:     i = i+1if i == 3:continueprint(i)</td>

  </tr>

 </tbody>

</table>

<table width="0">

 <tbody>

  <tr>

   <td width="69">12456</td>

  </tr>

 </tbody>

</table>

<em>Output:</em>




<h1>Case Studies</h1>

<h2>Case Study 1 – Class Average Program 1</h2>

Imagine that a class of ten students took a quiz. The scores, integers in the range of [0, 100], for this quiz are available to us. We need to determine the grades and the class average on the quiz.

Assume that the scores are <em>50, 100, 75, 66, 88, 85, 46, 91, 0, </em>and <em>23</em>.

The grade assignment is based on the table below:

<table width="0">

 <tbody>

  <tr>

   <td width="102"><strong>Score range</strong></td>

   <td width="95"><strong>Grade</strong></td>

  </tr>

  <tr>

   <td width="102">85 or above</td>

   <td width="95">A</td>

  </tr>

  <tr>

   <td width="102">75 to 84</td>

   <td width="95">B</td>

  </tr>

  <tr>

   <td width="102">65 to 74</td>

   <td width="95">C</td>

  </tr>

  <tr>

   <td width="102">50 to 64</td>

   <td width="95">D</td>

  </tr>

  <tr>

   <td width="102">Below 50</td>

   <td width="95">F</td>

  </tr>

 </tbody>

</table>




Let’s try the following code:

<table width="0">

 <tbody>

  <tr>

   <td width="367">scores = [50, 100, 75, 66, 88, 85, 46, 91, 0, 23] total = 0;for s in scores:total += s if s &gt;= 85:grade = ‘A’elif s &gt;= 75:grade = ‘B’elif s &gt;= 65:grade = ‘C’elif s &gt;= 50:grade = ‘D’else:grade = ‘F’ print(i, grade, sep=’t’) print(‘Class average is ‘, total / len(scores))</td>

  </tr>

 </tbody>

</table>

<table width="0">

 <tbody>

  <tr>

   <td width="165">50      D100     A75      B66      C88      A85      A46      F91      A0       F23      FClass average is 62.4</td>

  </tr>

 </tbody>

</table>

<em>Output:</em>




In this example, we use a <em>for </em>statement to get each score from the list and assign it to the variable <em>s</em>.

In the <em>for</em> loop, we use the operator <strong>+=</strong> to increase the value of <em>total</em> by <em>s</em>. It is exactly the same as  <strong>total = total + s</strong>. So <strong>+=</strong> is also an assignment operator.

An <em>if…elif…else</em> statement is used for comparing the value of <em>s</em> and assign the grade.

The <strong>print(i, grade, sep=’t’)</strong> statement outputs two values, <em>i</em> and <em>grade</em>, separated by a tab (i.e., <strong>‘t’</strong>).




<h2>Case Study 2 – Class Average Program 2</h2>

We need to implement a program for determining the grades and the class average on the quiz. Our program will prompt the user to input the scores until the input equals ‐1. The grade assignment is based on the same criteria mentioned in Case Study 1.

Let’s try the following code:

<table width="0">

 <tbody>

  <tr>

   <td width="373">#%%total = 0 # total markscount = 0 # to count the number of students while True:s = input(‘Enter score, ‐1 to end: ‘)s = int(s) if s &lt; 0:         break total += scount += 1 </td>

  </tr>

 </tbody>

</table>

<em>Output:</em>

<table width="0">

 <tbody>

  <tr>

   <td width="373">


    <table width="0">

     <tbody>

      <tr>

       <td width="373">    if s &gt;= 85:grade = ‘A’elif s &gt;= 75:grade = ‘B’elif s &gt;= 65:grade = ‘C’elif s &gt;= 50:grade = ‘D’else:grade = ‘F’ print(‘Grade ‘, grade) if count &gt; 0:average = total / count else:average = 0print(‘There are {} students’.format(count)) print(‘Class average is {0:.2f}’.format(average))</td>

      </tr>

     </tbody>

    </table></td>

   <td width="726">


    <table width="0">

     <tbody>

      <tr>

       <td width="215">Enter score, ‐1 to end: <strong>75</strong>Grade  B Enter score, ‐1 to end: <strong>45</strong>Grade  F Enter score, ‐1 to end: <strong>63</strong>Grade  D Enter score, ‐1 to end: <strong>15</strong>Grade  F Enter score, ‐1 to end: <strong>82</strong>Grade  B Enter score, ‐1 to end: <strong>‐1 </strong>There are 5 studentsClass average is 56.00</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>




As we do not know how many scores will be inputted, we use a while statement with <strong>True</strong>. It is an infinite loop that will not stop because the condition always is true.

In addition, we check whether the user input equals ‐1 or not. If yes, we use a <strong>break</strong> statement to exit the loop.

We use the variable <strong>count</strong> to count the number of scores inputted.

One more thing we need to pay attention to is that the user may input <strong>‐1</strong> immediately after starting the program. The value of <strong>count</strong> will be zero. There is a zero division program when we calculate the average using the statement <strong>average = total / count</strong>. Therefore, we need to check whether <strong>count</strong> is greater than zero or not.

Finally, to only print 2 factional digits of variable <strong><em>average</em></strong>, we use a placeholder {0:.2f} in the last <strong>print</strong> statement. The {0} indicates that the placeholder {} will be replaced by the 1<sup>st</sup> argument in the format(). The “.2f” indicates that the argument is a floating number with 2 digits after the period.




<h2>Case Study 3 – Shapes Printing Program</h2>




We are going to use Python program to print shapes with star symbols. The expected outputs are as follows.

*

**

***

****

*****

******

*******

********

*********




Let’s try the following code:

for i in range(10):

for j in range(i):

print(‘*’, end=”)     print()

In the above example, we nest <em>for</em> statements inside another <em>for</em> statements. The outer for statement is used for printing ten rows. The inner for statement is used for printing a single row. Note that the <strong>print()</strong> function with <strong>end=”</strong> (empty string instead of the default ‘
’ newline character) will print the value without a newline. And, the <strong>print()</strong> function without parameter will print a newline.

<strong>A more interesting example</strong>: In the following example, the program will output the same shape as an animation by sleeping for 0.5 second after displaying a *. Python has a <strong>time</strong> module that offers many useful functions related to time and date. To access this <strong>time</strong> module, we need to use <strong>import time</strong> first. The function <strong>time.sleep(sec)</strong> will suspend the execution of the program for the given number of seconds. We will learn more Python modules in this course.

<table width="0">

 <tbody>

  <tr>

   <td width="42">1234567</td>

   <td width="300">import time # import the time module of Python for i in range(10):for j in range(i):print(‘*’, end=”)time.sleep(0.5)         <em># pause for 0.5 second </em>print()</td>

  </tr>

 </tbody>

</table>




<h1>Exercises</h1>

<h2>Exercise 1 – Greeting</h2>

Write a program to accept a user input and then print the greeting based on the following rules:

<table width="0">

 <tbody>

  <tr>

   <td width="62">Rule</td>

   <td width="164">Input</td>

   <td width="203">Reply</td>

  </tr>

  <tr>

   <td width="62">1</td>

   <td width="164">“How are you?”</td>

   <td width="203">“Fine, and you?”</td>

  </tr>

  <tr>

   <td width="62">2</td>

   <td width="164">“How do you do.”</td>

   <td width="203">“How do you do.”</td>

  </tr>

  <tr>

   <td width="62">3</td>

   <td width="164">“Good to see you.”</td>

   <td width="203">“Me too.”</td>

  </tr>

  <tr>

   <td width="62">4</td>

   <td width="164">others</td>

   <td width="203">“…”</td>

  </tr>

 </tbody>

</table>




<strong>Hint:  </strong>

<ul>

 <li>Use the function <strong>input() </strong>to get the user input.</li>

 <li>Use <strong>.then..else</strong> statement to check the inputted text.</li>

 <li>Use the function <strong>print()</strong> to print the reply.</li>

 <li>The following is the sample output of the program:</li>

</ul>

<em>Computer: </em>Hi!

<em>You: </em>Good to see you.

<em>Computer:</em> Me too.




<h2>Exercise 2 – Summation</h2>

Write a program to accept integer inputs until the user inputs a non‐integer. Then, the program prints the summation of the inputted numbers.

<strong>Hint: </strong>

<ul>

 <li>Use the function <strong>input()</strong> to get the user input.</li>

 <li>Use a variable <strong>total</strong> for calculating the summation.</li>

 <li>Need to use <em>while</em> loop for the repeated inputs.</li>

 <li>Use if statement with <strong>isdigit()</strong> function to check whether the user input is an integer or not.</li>

</ul>

if (n.isdigit() == False):

break




<ul>

 <li>If the user input is an integer, use the function <strong>int()</strong> to convert the user input to an integer and add it to the variable <strong>total</strong>.</li>

</ul>

a = int(n)




<ul>

 <li>If the user input is not an integer, use the <strong>break</strong> statement to exit the loop immediately.</li>

 <li>The following is the sample output of the program:</li>

</ul>

Input an integer: 5




Input an integer: 10




Input an integer: 2




Input an integer: x total =  17




<h2>Exercise 3 – Maximum Value</h2>

Write a program to get 5 integer inputs and then print the maximum one. Assume that the user will input integers only.

<strong>Hint: </strong>

<ul>

 <li>Use <em>for</em> statement to get user inputs 5 times.</li>

 <li>Use <em>if</em> statement to compare the integers.</li>

 <li>The following is the sample output of the program:</li>

</ul>

Input a number: 15




Input a number: 3




Input a number: 21




Input a number: 9




Input a number: 18

Maximum is  21