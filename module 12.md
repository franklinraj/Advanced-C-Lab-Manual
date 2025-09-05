

# EXP NO 26: C PROGRAM TO DISPLAY STACK ELEMENTS USING LINKED LIST.
# Aim:
To write a C program to display stack elements using linked list.

# Algorithm:
1.	Define a structure Node with two members: data to store the integer value and next to point to the next node in the linked list.
2.	Declare a global variable head representing the starting node of the linked list.
3.	Define a function display to print the elements of the linked list.
4.	Declare a pointer p and initialize it with the head of the linked list.
5.	Use a while loop to traverse the linked list:
6.	Print the data of the current node.
7.	Move to the next node using the next pointer.
 
# Program:
```
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void display()  
{  
    while(head!=NULL)
    {
        printf("%.2f\n",head->data);
        head=head->next;
    }
}
```

# Output:

<img width="771" height="776" alt="12 1" src="https://github.com/user-attachments/assets/cf001206-f5e0-425d-a2a0-950b99fc8df0" />


# Result:
Thus, the program to display stack elements using linked list is verified successfully. 



# EXP.NO 27: C PROGRAM TO POP AN ELEMENT FROM THE GIVEN STACK USING 
LINKED LIST.
# Aim:
To write a C program to pop an element from the given stack using liked list.

# Algorithm:
1.	Check for Empty Stack
2.	If head is equal to NULL, Print "Stack is empty."
3.	Else Proceed to the next step.
4.	Set head to point to the next node in the stack.
 
# Program:
```
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void pop()  
{ 
    struct Node*temp;
    if(head==NULL)
    {
        printf("stack is empty");
    }
    else
    {
        temp=head;
        head=head->next;
        free(temp);
    }
}
```
# Output:

<img width="910" height="469" alt="12 2" src="https://github.com/user-attachments/assets/5810b2e6-07bd-49e8-9f47-e10088cd5e70" />



# Result:
Thus, the program to pop an element from the given stack using liked list is verified successfully.

 
# EXP NO:28 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING LINKED LIST.
# Aim:
To write a C program to display queue elements using linked list.
# Algorithm:
1.	Check if Queue is Empty
2.	Display Queue Elements
3.	Print the data of the current node pointed to by front
4.	Update front to point to the next node.
5.	End the display function.
 
# Program:

```
struct Node
{
   int data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void display()
{
    struct Node *temp;
    temp=front;
    if(rear==NULL)
    {
        printf("queue is empty");
    }
    else
    {
        while(temp!=NULL)
        {
            printf("%d\n",temp->data);
            temp=temp->next;
        }
    }
}
```
# Output:

<img width="758" height="680" alt="12 3" src="https://github.com/user-attachments/assets/cb37e439-70fb-45bc-af36-e6712f713df3" />


# Result:
Thus, the program to display queue elements using linked list is verified successfully.


 
# EXP NO:29 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING LINKED LIST

# Aim:
To write a C program to insert elements in queue using linked list

# Algorithm:
1.	Allocate Memory for New Node
2.	Set Data and Next Pointer
3.	Check if Queue is Empty
4.	Set both front and rear to point to the new node p.
5.	Set the next pointer of the current rear to point to the new node p.
6.	End of Enqueue Operation
 
# Program:
```
struct Node
{
   char data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void enqueue(char data)
{
    struct Node *newnode;
    newnode=(struct Node*)malloc(sizeof(struct Node));
    newnode->data=data;
    newnode->next=NULL;
    if(front==NULL && rear==NULL)
    {
        front=rear=newnode;
    }
    else
    {
        rear->next=newnode;
        rear=newnode;
    }
}
```
# Output:

<img width="769" height="686" alt="12 4" src="https://github.com/user-attachments/assets/92e1ab90-ddcd-4dc0-b59f-cc8e748b028b" />


# Result:
Thus, the program to insert elements in queue using linked list is verified successfully.



# EXP NO:30 C FUNCTION TO FIND THE PEEK OF QUEUE USING LINKED LIST.


# Aim:

The aim of this function is to retrieve the "peek" (the front element) of a queue implemented using a linked list

# Algorithm:

1.	Check if the queue is empty:
o	If the queue is empty (i.e., the front pointer is NULL), return an error or a message indicating that the queue is empty.
2.	Access the front element:
o	If the queue is not empty, return the data stored in the front node of the linked list (i.e., the element at the head of the queue).

# Program:

```
struct Node
{
   char data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void peek()
{
    printf("%c\n",front->data);
}
```

# Output:


<img width="569" height="713" alt="12 5" src="https://github.com/user-attachments/assets/74a55da0-390c-479e-ab9b-dba71aecfcad" />


# Result:

Thus, the program to retrieve the "peek" (the front element) of a queue implemented using a linked list is verified successfully.


