# **Java Tokens → 
smallest individual components/units in a java program that the compiler understands.
Java tokens are broadly divided into 5 types →

i) Keywords
ii) Identifiers
iii) Operators
iv) Separators / punctuators
v) Literals
vi) Comments

---

# **i) Keywords :**

✔ **Datatype keywords** → byte, short, int, long, float, double, char, boolean

✔ **Access Modifiers** → public, private, protected

✔ **Non-Access Modifiers** → static, final, abstract, synchronized, volatile, transient, native, strictfp

✔ **Class and object related keywords** → class, extends, interface, implements, new, this, super

✔ **Control flow keywords** → if, else, switch, case, default, for, while, do, break, continue, return

✔ **Exception Handling keywords** → try, catch, finally, throw, throws

✔ **Package related keyword** → package, import

✔ **Loop and decision support** → assert

✔ **Miscellaneous keyword** → void, instanceof, enum

✔ **Reserved but not used** → goto, const

---

### **Properties :**

• Keywords are reserved words in java that have a predefined meaning and special purpose.
• Java has 50 keywords.
• Once declared, can’t change the meaning.
• Lower case always.
• Not defined as identifiers.

---

# **ii) Identifiers :**

Names given to the program elements such as package, class, interface, object, method, variable.
→ They help identify elements uniquely in a program.

---

### **Rules for naming identifiers →**

• Alphabets (A-Z, a-z)
• Digits (0-9)
• Contains _ and $ . No other special characters and space are allowed.

• Must not start with a digit
❌ int 2num;
✔ int num1;

• Must not be a java keyword
❌ int class;
✔ int a;

• Case sensitive
int total;
int Total;
both are different

---

# **Naming conventions – standard / best practice for developers :**

Element → Convention → Example

• package → lower_case → javapack
• class and interface → PascalCase → StudentDetails, Printable
• method → camelCase → testMain(), calculateSum()
• variable → camelCase → totalMarks
• constant → UPPER_CASE → MAX_SIZE

*PascalCase is also known as UpperCamelCase*

---

# **iii) Separators :**

Special symbols used to separate program elements and define the structure of a java program.

---

### **List of java separators →**

Separator → Purpose

( ) → parenthesis used in methods, conditions, loops

{ } → curly braces define class, method, loop blocks

[ ] → square brackets used for arrays

; → semicolon ends a statement

, → comma separates variable / arguments

. → dot used to access class members

: → colon used in labels, enhanced for loop

... → Ellipsis used in var-args

---

# **iv) Operators :**

Operators are symbols that perform operations on variables and values.

They are used to manipulate data and produce results.

---

### **Types of operators →**

• Arithmetic → (+, -, *, /, %)

• Comparison / Relational → (>, <, >=, <=, ==, !=)

• Logical → (&&, ||, !)

• Assignment → (=, +=, -=, *=, /=, %=)
or compound assignment operators

---

• Increment – Decrement → (++ , --)
→ pre(++a, --a) and post(a++, a--)

---

• Ternary / conditional → (?)
→ condition ? value1 : value2
               True     False

---

• Bitwise → (&, ^, ~, <<, >>)
(AND, XOR, complement, left shift, right shift)

---

• Instance operator → (used to check object type)

```
if (obj instanceof String)
{
   sopln ("String object");
}
```

---

### **Unary operators → works on only one operand → ++, --, !**

---

### **Arithmetic addition →**

i) Basic addition
a + b → 30

ii) Concatenation
"java" + 10 → java10

---

### **Combination case →**

i) 10 + 20 → 30
ii) "10" + 20 → 1020
iii) 10 + "20" → 1020
iv) "A" + 10 + 20 → A1020
v) 10 + 20 + "A" → 30A

---

# **v) Literals :**

Fixed constant values directly written in a java program.
→ Their value doesn’t change during program execution.

int x = 10; // 10 is a literal
String name = "java"; // "java" is a literal
---

### **Java literals are mainly 6 types →**

• Integer (byte, short, int, long(L))
number system (decimal, octal, hexadecimal, binary)

• Floating point (float(f), double)

• Character (char) → enclosed with single quotes 'a'

• String (String) → enclosed with double quotes"java"

• Boolean → (true, false)

• Null (null) → represents no reference

---

### **Notes :**

• null, true, false → literals not keywords
• float literals need the suffix f
• literals are fixed value

---

# **vi) Comments :**

Non-executable statements used to explain code.
They are ignored by the java compiler.

---

### **Types →**

• Single line → //
• Multiline → /* */

---
