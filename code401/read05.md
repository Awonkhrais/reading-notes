# Linked Lists

![](https://res.cloudinary.com/practicaldev/image/fetch/s--XEtVnws7--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/trsu6uhv8j0x1fhzx53a.png)

* A linked list is a sequence of data elements, which are connected together via links. Each data element contains a connection to another data element in form of a pointer

## types of Linked List:

Singly : Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

Doubly : Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

* Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

* Next:

Each node contains a property called Next. This property contains the reference to the next node.

* Head:

The Head is a reference type of type Node to the first node in a linked list.

* Current

The Current reference is a reference type of type Node that is currently being looked at. This node is traditionally used when traversing through a full linked list. When traversing, you typically reset the current to the head to guarantee you are starting from the beginning of the linked list.

* Big O Notation

![](https://res.cloudinary.com/practicaldev/image/fetch/s--ark_FZG1--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/1omv0tmikzeaj24z8ps2.jpeg)

* is a way of evaluating the performance of an algorithm. takes into account the speed and efficiency with which something functions when its input grows to be any (crazy big!) size.

* O:

referred to as just “O” or sometimes as “order”, and a variable n, where n is the size of the input

* O(1):

function takes constant time, which is to say that it doesn’t matter how many elements we have, or how huge our input is: it’ll always take the same amount of time and memory to run our algorithm.

* O(n):

function is linear, which means that as our input grows (from ten numbers, to ten thousand, to ten million), the space and time that we need to run that algorithm grows linearly.

* O(n²):

function : which clearly takes exponentially more time and memory the more elements that you have. It’s pretty safe to say that we want to avoid O(n²) algorithms, just from looking at that crazy red line!