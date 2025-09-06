EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Name:FRANKLIN RAJ

Reg No: 212223230058

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:
```
#include <stdio.h>
#define SIZE 5

int stack[SIZE];  
int top = -1;     

void push(int value) {
    if (top == SIZE - 1) {
        printf("Stack is full (Overflow)\n");
    } else {
        top++;
        stack[top] = value;
        printf("%d pushed to stack\n", value);
    }
}

void pop() {
    if (top == -1) {
        printf("Stack is empty (Underflow)\n");
    } else {
        printf("%d popped from stack\n", stack[top]);
        top--;
    }
}

void display() {
    if (top == -1) {
        printf("Stack is empty\n");
    } else {
        printf("Stack elements:\n");
        for (int i = top; i >= 0; i--) {
            printf("%d\n", stack[i]);
        }
    }
}

int main() {
    push(10);
    push(20);
    push(30);
    display();
    pop();
    display();
    return 0;
}
```

Output:
![Screenshot 2025-05-07 112223](https://github.com/user-attachments/assets/0127af1b-302e-420f-aa0d-b6a336281cd1)
![Screenshot 2025-05-07 112237](https://github.com/user-attachments/assets/721810b9-ee58-438b-b834-b8f191de657e)
![Screenshot 2025-05-07 112250](https://github.com/user-attachments/assets/e1c0983c-2881-48f9-a202-b02546d63065)




Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:
```
char stack[100];
int size=3,top=-1; 
void push (float data) { 
    if(top==size-1) 
    {
    printf("stack is full\n");
    } 
    else
    {
        stack[top]=data; 
    } 
    }
```
Output:

<img width="485" height="544" alt="EX-9_02" src="https://github.com/user-attachments/assets/a5f4faef-e64c-4deb-8f39-8a1298d25e8b" />

Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:
```
int queue[50], rear=-1, front=-1; 
void display() { 
    if(front==-1||front>rear) 
    {
        printf("No elements to display");
    }     
    else
    { 
    for(int i=front;i<=rear;i++)
    { 
        printf("%d\n",queue[i]); 
    }
    }
}
```   
Output:

<img width="674" height="521" alt="EX-9_03" src="https://github.com/user-attachments/assets/42e1b9b4-79bd-4e8e-8388-576e2a83373d" />



Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:
```
int front,rear,size=3; 
char queue[50];
void enqueue(char data) { 
    if(rear<size) 
    { if(front==-1) 
    {
        front=0;
    } 
    rear++;
    queue[rear]=data;
    }
    }
```
Output:

<img width="724" height="453" alt="EX-9_04" src="https://github.com/user-attachments/assets/e09aeb6c-24c9-4107-a868-2261a7cccb41" />


Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:
```
int front, rear; 
void dequeue() { 
    if(front==-1||front>rear) 
    { 
        printf("Queue Underflow.\n");
    } 
    else 
    { 
        front++; 
    } 
    }
```
Output:

<img width="824" height="620" alt="EX-9_05" src="https://github.com/user-attachments/assets/a3a5b835-b181-4e15-8ce8-d5528232806d" />



Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
