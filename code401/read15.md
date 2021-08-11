# Trees

## Common Terminology

- Node - A tree node is a component which may contain it's own values, and references to other nodes
- Root - root is the node at the beginning of the tree.
- K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, `k = 2`
- Left - A reference to one child node, in a binary tree.
- Right - A reference to the other child node in a binary tree.
- Edge - The edge in a tree is the link between a parent and child node.
- Leaf - A leaf is a node that does not have any children.
- Height - The height of a tree is the number of edges from teh root to the furthest leaf.

## Traversals

- Traversing a tree allows us to seach for a node, print out the contents of a tree, and much more. There are two categories of traversals when it comes to trees: Depth First, Breadth First.

### Depth First

- Prioritize going through the depth (heigth) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the `root`.
- Pre-order: `root >> left >> right`
- In-order: `left >> root >> right`
- Post-order: `left >> right >> root`
- The most common way to traverse through a tree is to use recursion, which relies on teh call stack to navigate back up the tree when we have reaches the end of a sub-path.

### Pre-order

- means the `root` has to be looked at first.
- When we look at `root.value` first, it means that we output its value. When we call `preOrder` for the first time, the `root` will be added to the call stack.
- Next we check if the `root` has a `left` node set, if so, then send the `left` node to our preOrder method recursively and that `node` becomes the new `root`. 
- The process continues until we reach a leave `node` (bottom of the tree). If the leave node doesn't have a `root.left` or `root.right`, both will return `null` and will end the execution of that method call.
- When it compeletes a function call, we pop it off the stack and are able to continue execution through thte previous function call.
- Code block picks up at the previous root node and check `root.right`, and so-on.

### Breadth First

- iterates through the tree by going through each level of teh tree node-by-node.
- Uses a queue(instead of the call stack via recursion) to traverse the width/breadth of the tree.
- Put `root` nodd into the front of the queue.
- Now that we have one node in our queue, we can `dequeue` it and use that node in our code.
- From our `dequeued` node `A`, we can `enqueue` the `left` and `right` child( in that order).
- node `B` becomes front and node `C` becomes `node.next`.
- `dequeue` node `B` and `enqueue` node `D` and `E`.
- Node that `C` is first node, repeat the `dequeue + enqueue` children process. 
- Once we reach a node that doesn't have any children, we just `dequeue` it without any further `enqueue`.

### Binary Tree Vs K-ary Tress

- Trees have a number of children per node, but Binary trees restrict the number of children to two (`left` and `right` children).
- There is no specific sorting order for a binary tree. Nodes can be added whever space allows them.