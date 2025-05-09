# EX 49 C function to search an element in the doubly linked list.
## DATE:09-05-25
## AIM:
To write a C function to search an element in the doubly linked list.

## Algorithm
1. Start. 
2. Define a variables. 
3. Write a function to search an element in the double linked list.. 
4. Read the value using scanf. 
5. Ask the user to make an input. 
6. Print out the answer. 
7. End

## Program:
```
struct Node 
{ 
struct Node *prev; 
struct Node *next; 
int data; 
}*head; 
 
void search(int data) 
{ 
struct Node *temp; 
int item=data,i=0,flag; 
temp=head; 
if(temp==NULL) 
{ 
printf("Empty list\n"); 
} 
else{ 
while(temp!=NULL) 
{ 
if(temp->data == item) 
{ 
printf("item %d found at location %d",item,i+1); 
flag=0; 
} 
i++; 
temp=temp->next; 
} 
if(flag!=0) 
{ 
printf("Item not found\n"); 
} 
} 
}
```

## Output:
![Screenshot 2025-05-07 224636](https://github.com/user-attachments/assets/e1a2f71b-4dd1-4e50-ad5e-ea4e1b69f084)


## Result:
Thus the program was executed and the output was verified successfully.
