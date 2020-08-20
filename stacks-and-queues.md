## Stacks & Queues

* Stack is a data structure that consists of nodes
* Each node references the next node in the stack

### Terminology

* **push** - Nodes or items that are puth into the stack are pushed
* **pop** - Nodes or items that are removed from the stack are popped
* **Top** - Top of the stack
* **Peek** - View the value of the top Node in the stack
* **isEmpty** - returns true when stack is empty. Otherwise returns false

### Stack Concepts

* **FILO** - First In Last out - If you think of this visually, it makes good sense. The first thing on the stack has to wait for anything stacked on top to be removed (pop) before it can be removed.
* **LIFO** - Last In First Out - This is the opposite of the previous
* Stack Visualization
  * Top most item is called the top
  * Each new item becomes the new top
  * Whe something is removed, the thing below it becomes the top again
* Push O(1) - Pushing a Node onto a stack is O(1) as it takes the same amount of time no matter no many Nodes(n) are in the stack 
* Steps
  1. Identify Node that should be added to stack
  2. Assign the **next** property of new Node to reference the same Node that **top** is referencing
  3. Re-assign top to the new Node
* Pseudo code to push a node onto a stack
  * `algorithm push(value)`
     `//Input <-- value to add, wrapped in Node interally`
     `// Output <-- none`
     `node = New Node(value)`
     `node.next <-- Top`
     `top <-- Node`
* Pop O(1) - Popping a Node off a stack is the action of removing a Node
  1. Create reference named **temp** that points to same Node that top points to
  2. Re-assign top to the value that the next property is referencing
  3. Remove top node safely without affecting the rest of the stack
    * Remember to clear out the next property in current **temp** reference
* Peek O(1) - Only inspecting the top Node in the stack
  * Check **isEmpty** before peeking.

### What is a Queue?

  * Enqueue - Nodes or items added to the queue
  * Dequeue - Nodes or items removed from queue
  * Front - First node of the queue
  * Rear - Last Node of the queue
  * Peek - View the value of the **front** Node in queue
  * IsEmpty - Returns true when queue is empty
* Queues are FIFO and LILO
* Enqueue O(1) - Does not matter how many other items live in the queue
* Dequeue O(1) - Does not matter how many other items are in the queue
* Peek O(1) - Only inspecting the front Node of the queue
* IsEmpt O(1) - checking it queue is empty
