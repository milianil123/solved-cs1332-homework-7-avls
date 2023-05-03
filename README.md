Download Link: https://assignmentchef.com/product/solved-cs1332-homework-7-avls
<br>
You are required to implement an AVL tree. An AVL is a special type of binary search tree that follows all the same rules: each node has 0-2 children, all data in the left subtree is less than the node’s data, and all data in the right subtree is greater than the node’s data. The AVL differs from the BST with its own self-balancing rotations, which you must implement.

All methods in the AVL tree that are not O(1) <strong>must be implemented recursively</strong>. Good recursion with simple, focused states is strongly encouraged for this assignment in particular.

It will have two constructors: a no-argument constructor (which should initialize an empty tree), and a constructor that takes in data to be added to the tree, and initializes the tree with this data.

<h2>Balancing</h2>

Each node has two additional instance variables, height and balanceFactor. The height variable should represent the height of the node. If you recall, a node’s height is max(child nodes’ heights) + 1 where the height of a null is -1. The balance factor of a node should be equal to its left child’s height minus its right child’s height. Since we’ve stored this information in each node, we no longer need to recursively compute them.

The tree should rotate appropriately to make sure it’s always balanced. For an AVL tree, a tree is balanced if every node’s balance factor is either -1, 0, or 1. Keep in mind that you will have to update the balancing information stored in the nodes on the way back up the tree after modifying the tree; the variables are not updated automatically.

<h2>Important Notes</h2>

Here are a few notes to keep in mind when switching from BST to AVL trees:

<ol>

 <li>Use the <strong>successor</strong>, not predecessor.</li>

 <li>After every change to the tree, make sure to update height and balance factor fields of all nodes whose subtrees have been modified.</li>

 <li>Make sure the height method is O(1).</li>

 <li>The traversals and the isBST() method have been removed, and two other recursive practice problems have been added.</li>

</ol>