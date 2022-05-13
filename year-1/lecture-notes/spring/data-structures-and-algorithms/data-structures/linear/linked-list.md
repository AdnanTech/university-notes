# Linked List

## Singly Linked List

A singly linked list is a linear, 'node based' data structure that uses dynamic memory allocation. Very similar to arrays, a linked list uses a collection of nodes that colectively form a linear sequence. Each node stores a reference to an object that is an element of the sequence.

* Memory 'blocks' of elements can be placed randomly in memory, as they are connected via a pointer, tail and head that keeps track of all the nodes with their data inside the block of memory.
* Singly Linked lists to not allow for reverse traversal.
* Removal of the last node is relatively ineffecient.
* Has nodes that keep track of the "head" and "tail" of a data set.

![](<../../../../../../.gitbook/assets/image (205) (1).png>)

### Insertion in a Singly Linked-List

You can easily add elements at the head of a singly linked list. To do this, you would create a new node, set its element to the new element, set its next link to refer to the current head, and set the list's head to point to the new node.

Not that the next pointer of the new node is set **before** we reassign variable head to it. If the list were initially empty (i.e., head is null), then a natural consequence is that the new node has its next reference set to null.

![](<../../../../../../.gitbook/assets/image (202).png>)

Using similar logic, we can add elements to the end of a singly linked list. You create a new node, assign its next reference to null, set the next reference of the tail to point to this new node, and then update the tail reference itself to this new node

![](<../../../../../../.gitbook/assets/image (199) (1).png>)

### Removal in a Singly Linked-List

To remove an element from a the head of a singly linked list, we use the reverse operation of insertion.

![](<../../../../../../.gitbook/assets/image (197).png>)

Note that we cannot easily delete the last node of a isngly linked list as we need to acess the node before the last node in order to remove the last node. Meaning we can't go back up from the tail. So instead, the way to remove the last node would be by following the links from the head until you get to the tail. **This is time ineffecient.** Which brings us onto Doubly linked lists.

### Implementing a Singly Linked List Class

```python
class Node:
   def __init__(self, data=None):
      self.data = data
      self.next = None
class SLinkedList:
   def __init__(self):
      self.head = None

# Function to add newnode
   def Atbegining(self, data_in):
      NewNode = Node(data_in)
      NewNode.next = self.head
      self.head = NewNode

# Function to add newnode
   def AtEnd(self, newdata):
      NewNode = Node(newdata)
      if self.headval is None:
         self.headval = NewNode
         return
      laste = self.headval
      while(laste.nextval):
         laste = laste.nextval
      laste.nextval=NewNode
      
# Function to add node
   def Inbetween(self,middle_node,newdata):
      if middle_node is None:
         print("The mentioned node is absent")
         return

      NewNode = Node(newdata)
      NewNode.nextval = middle_node.nextval
      middle_node.nextval = NewNode
         
# Function to remove node
   def RemoveNode(self, Removekey):
      HeadVal = self.head
         
      if (HeadVal is not None):
         if (HeadVal.data == Removekey):
            self.head = HeadVal.next
            HeadVal = None
            return
      while (HeadVal is not None):
         if HeadVal.data == Removekey:
            break
         prev = HeadVal
         HeadVal = HeadVal.next

      if (HeadVal == None):
         return

      prev.next = HeadVal.next
         HeadVal = None

   def LListprint(self):
      printval = self.head
      while (printval):
         print(printval.data),
         printval = printval.next

llist = SLinkedList()
llist.Atbegining("Mon")
llist.Atbegining("Tue")
llist.Atbegining("Wed")
llist.Atbegining("Thu")
llist.RemoveNode("Tue")
llist.LListprint()
```

## Doubly Linked-Lists

A doubly linked list is where each node keeps an explicit reference to the **node before it and a reference to the node after it**. These lists allow a greater variety of O(1)-time update operations, including insertions and deletions at arbitrary positions within the list. The most significant change from single to double is that the head and tail turn into head and trailer nodes, called **sentinels**.

![](<../../../../../../.gitbook/assets/image (201).png>)

**Advantages** include being able to traverse backwards and forwards. Also, the header and trailer are never changed, making operations on the list more simple. Random insertion and removal can be done easier.

### Implementation of a Doubly Linked-List

```python
# Initialise the Node
class Node:
    def __init__(self, data):
        self.item = data
        self.next = None
        self.prev = None
# Class for doubly Linked List
class doublyLinkedList:
    def __init__(self):
        self.start_node = None
    # Insert Element to Empty list
    def InsertToEmptyList(self, data):
        if self.start_node is None:
            new_node = Node(data)
            self.start_node = new_node
        else:
            print("The list is empty")
    # Insert element at the end
    def InsertToEnd(self, data):
        # Check if the list is empty
        if self.start_node is None:
            new_node = Node(data)
            self.start_node = new_node
            return
        n = self.start_node
        # Iterate till the next reaches NULL
        while n.next is not None:
            n = n.next
        new_node = Node(data)
        n.next = new_node
        new_node.prev = n
    # Delete the elements from the start
    def DeleteAtStart(self):
        if self.start_node is None:
            print("The Linked list is empty, no element to delete")
            return 
        if self.start_node.next is None:
            self.start_node = None
            return
        self.start_node = self.start_node.next
        self.start_prev = None;
    # Delete the elements from the end
    def delete_at_end(self):
        # Check if the List is empty
        if self.start_node is None:
            print("The Linked list is empty, no element to delete")
            return 
        if self.start_node.next is None:
            self.start_node = None
            return
        n = self.start_node
        while n.next is not None:
            n = n.next
        n.prev.next = None
    # Traversing and Displaying each element of the list
    def Display(self):
        if self.start_node is None:
            print("The list is empty")
            return
        else:
            n = self.start_node
            while n is not None:
                print("Element is: ", n.item)
                n = n.next
        print("\n")

# Create a new Doubly Linked List
NewDoublyLinkedList = doublyLinkedList()
# Insert the element to empty list
NewDoublyLinkedList.InsertToEmptyList(10)
# Insert the element at the end
NewDoublyLinkedList.InsertToEnd(20)
NewDoublyLinkedList.InsertToEnd(30)
NewDoublyLinkedList.InsertToEnd(40)
NewDoublyLinkedList.InsertToEnd(50)
NewDoublyLinkedList.InsertToEnd(60)
# Display Data
NewDoublyLinkedList.Display()
# Delete elements from start
NewDoublyLinkedList.DeleteAtStart()
# Delete elements from end
NewDoublyLinkedList.DeleteAtStart()
# Display Data
NewDoublyLinkedList.Display()
```

## Circularly Linked Lists

In real life, there might not be a first to last linear sequence. Instead, it may loop around once last has been executed. For example, in a video game, Player A takes a turn, Player B and then Player C. Until the game is complete, it must loop back around to Player A's turn once Player C has finished his turn. This is called having a **cyclic order**, running on a continours loop.

The most significant case of circularly linked lists is in round-robin cpu scheduling, where each execution of given a time slice, interrupted if the time-slice has been complete, regardless of if the program has fully executed.

![](<../../../../../../.gitbook/assets/image (206) (1).png>)

Implementation would look something like this:

![](<../../../../../../.gitbook/assets/image (198).png>)
