**Famus Language**

**Project Name:** Famus

Members :<br>
**[Mehmet Fatih Kızıldağ - 20190808041](https://github.com/FatihKizildag)**
**[Mustafa Can Kartal    - 20180808046](https://github.com/cankartal01)**

 ##  Explanations about the language:
 <br>
The "Famus" programming language is a beginner-level language that includes basic loop, boolean, and function operations. Using loops, you can repeat certain actions, while using logical expressions enables you to control your programs based on conditions. Functions are reusable code blocks that perform a specific task. Code in "Famus" must follow specific syntax and semantic rules. This helps to reduce programming errors and increase code readability. Additionally, "Famus" includes various data types, such as numbers, strings, and boolean values. Since "Famus" is still in its early stages, many new features are planned. These may include more advanced data types, complex loops, and additional functions. The goal of the "Famus" language is to help beginners learn fundamental programming concepts and practice coding. It can also be used as a transition language for those wishing to move onto more advanced programming languages.
<br>
 
 
 ## Blocks and Commands
* **program :**  <br>
 	GO program STOP <br>
        **|** statements program <br>
	**|** program statements <br>
	**|** statements <br>
	**|** error <br>
* **statement :**  
 	statements <br>
        **|** printnumberStatement <br>
        **|** ınputStatement <br> 
        **|** IfElseStatement <br>
        **|** loopStatement <br>
        **|** commentStatement <br>
        **|** assignmentStatement <br>
    	**|** printStringStatement <br>
    	**|** booleanStatement <br>
	**|** methodStatement <br>
	**|** methodSingleParameterStatement <br>
	**|** methodDoubleParameterStatement <br>

* **printStringStatement:**<br>
    	PRINT STRING

* **printnumberStatement:**<br>
        PRINT term

* assignmentStatement:<br>
        ASSIGN '='exp

* **funcStatement :** <br>
	METHOD FUNCNAME statements RETURN statements SEMICOLON <br>
	**|** METHOD FUNCNAME OPP term CLP RETURN <br>
	**|** METHOD FUNCNAME OPP term COMMA term CLP RETURN IfElseStatement <br>

* **commentStatement :** <br>
	COMMENT

* **inputStatement:** <br>
	 INPUT

* **booleanStatements :**<br>
 	INT EQUALS INT <br>
	**|** INT BIGGER INT <br>
	**|** INT SMALLER INT <br>
	**|** INT BIGGER_EQUALS INT <br>
	**|** INT SMALLER_EQUALS INT <br>
	**|** INT AND INT <br>
	**|** INT OR INT  <br>
* **IfElseStatements:**  <br>
	IF booleanExpression exp ELSE exp <br>
	**|** IF booleanExpression PRINT term ELSE PRINT term <br>
	**|** IF term EQUALS term exp ELSE  <br>
	**|** IF OPP term MOD term CLP EQUALS term  <br>
	**|** IF term EQUALS term PRINT STRING ELSE PRINT STRING<br>

*  **loopStatement:** <br> LOOP term SMALLER term RETURN exp SEMICOLON       
        **|** LOOP term BIGGER term RETURN exp SEMICOLON      <br>
    	**|** LOOP term SMALLER term RETURN PRINT exp SEMICOLON<br>
    	**|** LOOP term BIGGER term RETURN PRINT exp SEMICOLON <br>
	**|** LOOP term SMALLER term RETURN PRINT STRING SEMICOLON <br>
	**|** LOOP term BIGGER term RETURN PRINT STRING SEMICOLON <br>
	**|** LOOP term NOT_EQUALS term RETURN term '=' term term '=' term assignmentStatement term <br>
	**|** LOOP term SMALLER term RETURN<br>

<a name="expressions"></a>
### Expressions ###

* **expression:** <br>
	comparisonExpression  <br>
	**|** orExpression <br>
	**|** andExpression  <br>
	**|** booleanExpression <br>

*  **exp**  : 
  term  <br>
  **|**  exp '+' term  <br> 
  **|**  exp '-' term <br>
  **|**  exp MOD term <br>
  **|**  FUNCNAME OPP term COMMA term CLP  <br>

*  **booleanExpression**  :  
  	term EQUALS term   <br>
  	**|** term BIGGER term   <br>
	**|** term SMALLER term    <br>
	**|** term BIGGER_EQUALS term <br> 
	**|** term SMALLER_EQUALS term <br>	 
	**|** term AND term <br>
	**|** term OR term <br>



* **comparisonExpression :**  <br>
 INT assignmentOperator INT <br>
 **|** ASSIGN assignmentOperator INT <br>


*  **orExpression :**<br>
        BOOLEAN OR BOOLEAN

*  **andExpression :** <br>
	BOOLEAN AND BOOLEAN

* **assignmentOperator :** <br>
 EQUALS <br>
 **|** BIGGER_EQUALS  <br>
 **|** SMALLER_EQUALS<br>
 **|** BIGGER<br>
 **|** SMALLER<br>


<a name="ExplanationSysntax"></a>
## Explanation Of the Syntax

<br>
* **PRINT DESCRIPTION-->**
In Famus language, "print" is used to display values on the screen. We print with the keyword "PRINT" and the character ":". 

```
GO
PRINT:"SELAM"
STOP

```
> SELAM


<br>
* **BOOLEAN OPERATION DESCRIPTION-->**

In Famus, the Boolean operators are EQUALS, GREATER, LESS, GREATER_EQUALS, LESS_EQUALS, AND, OR, or NOT. There may be operators that compare values and return TRUE or FALSE (like EQUALS, GREATER, LESS, GREATER_EQUALS, or LESS_EQUALS).

```
GO
1==2
1<4
STOP
```
> FALSE

> TRUE
<br>
* **IF ELSE-->**

In the Famus language, the conditional statement consists of two sections, the "if" part and the "else" part. The "if" section is utilized to determine the code block that will be executed if the specified condition is true. Conversely, the "else" section is employed to define the code block that will be executed if the same condition is false, in other words, it executes the statements following the "else" keyword.

```
GO
a=1
IF a<10 
  PRINT:1 
ELSE 
  PRINT:2
STOP
```
> 1
<br>
* **LOOP DESCRIPTION-->**

The while loop takes a single parameter and loops as long as that parameter is true. In our programming language, we can use a previously assigned variable as a parameter in a while loop.
```
GO
s = 0
LOOP s < 3 RETURN
  s+5;
STOP
```
> 15
<br>
* **METHOD DESCRIPTION-->**

To declare a function in the Famus language, the declaration begins with the keyword "METHOD". After that, the function name is specified using the " : " symbol, followed by parentheses where the parameters are defined based on the function's requirements. Finally, the function body is written using the "RETURN" keyword.
```
GO 
a = 1
b = 2
METHOD yaz: (a , b) RETURN 
     IF a<b 
         OUTPUT:5
     ELSE 
         OUTPUT:6
STOP
```
> 5
<br>
* **ERROR HANDLING DESCRIPTON-->**

Error handling has been incorporated into our programming language to anticipate, identify, and resolve programming, application, and communication errors. When an error occurs, the user is provided with an error message indicating that error handling has been triggered and the line number where the error has occurred.
```
GO 
a = 1  /*line1
b = 2  /*line2
c = 7  /*line3
unrecognized_text  /*line4
STOP /*line5
```
> syntax error on line 4
<br>
* **Example Program--> 1**

```
GO 
a = 5
b = 3
METHOD hangisibuyuk: (a , b) RETURN 
     IF a>b 
         PRINT: 1
     ELSE 
         PRINT: 2

STOP
```
> 1
<br>
* **Example Program--> 2**

```
GO
x = 0
y = 5
LOOP x < y RETURN PRINT: x ;
STOP
```
> 1

<br>
* **Example Program--> 3**

```
GO
a = 5
b = 25
c = b % a
PRINT: c
STOP
```
>0 <br>
>0 <br>
>0 <br>
>0 <br>



 




