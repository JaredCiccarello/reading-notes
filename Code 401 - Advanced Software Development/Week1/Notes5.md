June 16, 2023

Linked lists

Head of a link list is where a link list starts.

Head does not know anything else, just that it is the head.

Node doesn't know it's the head. It only know's who comes after it.

Node1 has a value of 4.

Only has to be sequential in memory.
A list does not have to be sequential memory.


Why can you not use a traversal when using a for loop?
Because a for loop does not know how big the list is going to be.




Node requires values

node1 = Node(1)
node2 = Node (2, node1)

node1.value = 4
print(node1.value)

This will change node1 value to 4

def test_node_1()
  actual = Node(1)
  expected = 1
  assert actual == expected

This function expects a 1 but, will return a node instead. Meaning this function will fail.

it needs to be:
def test_node_1()
  actual = Node(1)
  expected = 1
  assert actual.value == expected

Must have .value to look for value inside of Node.



def test_node_next()
  node1=Node(1)
  node2=Node(2, node1)
  actual = node2.next
  expected = node1
  assert actual == expected

This test will pass because node2.next has (2, node1) The .next is referring to node1 inside of node2. Notice this is not callling the value of node1 which would be 1. Only the node itself. This means the expected of node1 would be correct.




TRAVERSE
def traverse(self):
  current = self.head
  while current is not None:
    print(current.value)  <-- This is what 
    current = current._next

    ll1 [4]->[1]->[10]->[8]->None

    4 1 10 8

    We go through our list looking for "None". Until we find None we continue iterating through our list.

    MEMORIZE THIS CODE ^^^^^^^^^^^^^^
This is how we traverse through a node.

We do not LOOP through a link list. We traverse.

Once you think you have code, run through some of these codes through chatGPT. Compare.





