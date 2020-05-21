# Link List :>
 * is a linear structure consisting of node. Each node has a data part that holds the clint-supplied information, and a link that refers to the next node in the linked list 

* To access the entries of the linked list, a reference to its first entry is all we need.

 - One can access any entry by simply following the chain of links.
 - When an entry is removed from some place in a linked list, all that needs to be done is to have its predecessor's link refer to its successor.
 - Similarly, an entry may be inserted anywhere in the list without having to move other entries over to create space.

* the structure for link list 

`class Node{` 

`constructor(data, next = null){` 
` this.data = data,` 
` this.next = next` 

` }` 
`}` 

> next field of the node class is a reference to another Node<T> object.

* Inserting a node at the beginning of the singly linked list.

`LinkedList.prototype.insertAtBeginning = function(data){` 

`let newNode = new Node(data);` 
`newNode.next = this.head;    ` 
`this.head = newNode;` 
`return this.head;` 

`}` 

* delete from linked list 

`LinkedList.prototype.deleteFirstNode = function(){` 

` if(!this.head){` 

`   return;` 
`}` 
`this.head = this.head.next;` 

` return this.head;` 

`}` 

## what even is Big O?

 * how much time it requires at runtime given how much time and memory it needs.
 - An O(1) function takes constant time, which is to say that it doesn’t matter how many elements we have, or how huge our input is: it’ll always take the same amount of time and memory to run our algorithm.
 - O(n) function is linear, which means that as our input grows (from ten numbers, to ten thousand, to ten million), the space and time that we need to run that algorithm grows linearly.
 - O(n²) function, which clearly takes exponentially more time and memory the more elements that you have.

## difference between array and linked list

![array-Vs-linkedList](https://lh3.googleusercontent.com/proxy/KjS7e8a__Pt-FczThkS1izouJS481WuldLr8LwngNi7gVDDa-bq_7coBstO9I8vlw6nLwUEYhWGSkkSyPVxdB-7x6CiwdzUPZ9Dpf1kwRum7WyPQDYquUfh-zhauLEhglX3tXQwuE5Ag_3-pAnNL4IpUXNk)
