EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

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

int stack[100];
int top = -1;
int n;

void push(int x) {
    if (top == n - 1) {
        printf("Stack Overflow\n");
        return;
    }
    top++;
    stack[top] = x;
}

void pop() {
    if (top == -1) {
        printf("Stack Underflow\n");
        return;
    }
    printf("Popped: %d\n", stack[top]);
    top--;
}

void display() {
    if (top == -1) {
        printf("Stack is empty\n");
        return;
    }
    for (int i = top; i >= 0; i--) {
        printf("%d ", stack[i]);
    }
    printf("\n");
}

int main() {
    int choice, value;

    printf("Enter stack size: ");
    scanf("%d", &n);

    while (1) {
        printf("\n1.Push\n2.Pop\n3.Display\n4.Exit\n");
        printf("Enter choice: ");
        scanf("%d", &choice);

        if (choice == 1) {
            printf("Enter value: ");
            scanf("%d", &value);
            push(value);
        } 
        else if (choice == 2) {
            pop();
        } 
        else if (choice == 3) {
            display();
        } 
        else if (choice == 4) {
            break;
        } 
        else {
            printf("Invalid choice\n");
        }
    }

    return 0;
}

```

Output:

<img width="1627" height="739" alt="image" src="https://github.com/user-attachments/assets/745ea68b-4a87-44e2-ba2d-c24ab7fea9c5" />



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
#include <stdio.h>

float stack[100];
int top = -1;
int n;

void push(float x) {
    if (top == n - 1) {
        printf("Stack Overflow\n");
        return;
    }
    top++;
    stack[top] = x;
    printf("Pushed: %.2f\n", x);
}

int main() {
    float value;

    printf("Enter stack size: ");
    scanf("%d", &n);

    printf("Enter value to push: ");
    scanf("%f", &value);

    push(value);

    return 0;
}

```

Output:

<img width="1629" height="733" alt="image" src="https://github.com/user-attachments/assets/1488dd14-313b-4c63-8e42-13df589f8fd6" />




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
#include <stdio.h>

int queue[100];
int front = -1, rear = -1, n;

void enqueue(int x) {
    if (rear == n - 1) {
        printf("Queue Overflow\n");
        return;
    }
    if (front == -1) front = 0;
    rear++;
    queue[rear] = x;
    printf("Enqueued: %d\n", x);
}

void dequeue() {
    if (front == -1 || front > rear) {
        printf("Queue Underflow\n");
        return;
    }
    printf("Dequeued: %d\n", queue[front]);
    front++;
}

void display() {
    if (front == -1 || front > rear) {
        printf("Queue is empty\n");
        return;
    }
    printf("Queue elements: ");
    for (int i = front; i <= rear; i++) {
        printf("%d ", queue[i]);
    }
    printf("\n");
}

int main() {
    int choice, value;

    printf("Enter queue size: ");
    scanf("%d", &n);

    while (1) {
        printf("\n1.Enqueue\n2.Dequeue\n3.Display\n4.Exit\n");
        printf("Enter choice: ");
        scanf("%d", &choice);

        if (choice == 1) {
            printf("Enter value to enqueue: ");
            scanf("%d", &value);
            enqueue(value);
        } 
        else if (choice == 2) {
            dequeue();
        } 
        else if (choice == 3) {
            display();
        } 
        else if (choice == 4) {
            break;
        } 
        else {
            printf("Invalid choice\n");
        }
    }

    return 0;
}

```

Output:

<img width="1637" height="727" alt="image" src="https://github.com/user-attachments/assets/042f9fd2-d369-463b-8831-1a9e0ad92132" />



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
#include <stdio.h>

float queue[100];
int front = -1, rear = -1, n;

void enqueue(float x) {
    if (rear == n - 1) {
        printf("Queue Overflow\n");
        return;
    }
    if (front == -1) front = 0;
    rear++;
    queue[rear] = x;
    printf("Enqueued: %.2f\n", x);
}

int main() {
    float value;

    printf("Enter queue size: ");
    scanf("%d", &n);

    printf("Enter value to enqueue: ");
    scanf("%f", &value);
    enqueue(value);

    return 0;
}


```

Output:

<img width="1641" height="740" alt="image" src="https://github.com/user-attachments/assets/e9c4bde0-381b-4972-85dd-fdff135d5367" />


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
#include <stdio.h>

int queue[100];
int front = -1, rear = -1, n;

void enqueue(int x) {
    if (rear == n - 1) {
        printf("Queue Overflow\n");
        return;
    }
    if (front == -1) front = 0;
    rear++;
    queue[rear] = x;
    printf("Enqueued: %d\n", x);
}

void dequeue() {
    if (front == -1) {
        printf("Queue is empty\n");
        return;
    }
    printf("Deleted element: %d\n", queue[front]);
    front++;
    if (front > rear) {
        front = rear = -1;
    }
}

void display() {
    if (front == -1) {
        printf("Queue is empty\n");
        return;
    }
    printf("Queue elements: ");
    for (int i = front; i <= rear; i++) {
        printf("%d ", queue[i]);
    }
    printf("\n");
}

int main() {
    int choice, value;

    printf("Enter queue size: ");
    scanf("%d", &n);

    while (1) {
        printf("\n1.Enqueue\n2.Dequeue\n3.Display\n4.Exit\n");
        printf("Enter choice: ");
        scanf("%d", &choice);

        if (choice == 1) {
            printf("Enter value to enqueue: ");
            scanf("%d", &value);
            enqueue(value);
        } 
        else if (choice == 2) {
            dequeue();
        } 
        else if (choice == 3) {
            display();
        } 
        else if (choice == 4) {
            break;
        } 
        else {
            printf("Invalid choice\n");
        }
    }

    return 0;
}

```

Output:

<img width="1650" height="735" alt="image" src="https://github.com/user-attachments/assets/7f99b5a6-5b44-4f63-9ffe-0ffe38328899" />


Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
