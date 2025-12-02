README – Implement Stack Using Two Queues
📝 Problem Description

Implement a Stack (LIFO) data structure using two Queues (FIFO).

Your stack must support:

push(x)

pop()

top()

isEmpty()

🎯 Goal

Simulate stack behavior using only queue operations:

push()

pop()

front()

empty()

💡 Approach (Efficient Pop Method)

We use two queues:

q1 → main queue

q2 → temporary queue

Push(x) logic

Push x into q2.

Move all elements from q1 into q2.

Swap the names of the queues.

After this:

q1 will always have the newest element at the front,
making pop() and top() fast.

Pop() logic

Pop the front of q1.

📊 Time Complexity
Operation	Time
push()	O(n)
pop()	O(1)
top()	O(1)
empty()	O(1)
