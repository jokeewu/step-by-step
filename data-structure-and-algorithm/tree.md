# 树(Tree)

定义树的节点：
```javascript
function TreeNode(val) {
  this.val = val
  this.left = this.right = null
}
```

### 二叉树的遍历

先序、中序、后序其实指的是父节点被访问的次序。若在遍历过程中，父节点先于它的子节点被访问，就是先序遍历；父节点被访问的次序位于左右孩子节点之间，就是中序遍历；访问完左右孩子节点之后再访问父节点，就是后序遍历。不论是先序遍历、中序遍历还是后序遍历，左右孩子节点的相对访问次序是不变的，总是先访问左孩子节点，再访问右孩子节点。而层次遍历，就是按照从上到下、从左向右的顺序访问二叉树的每个节点。

#### 先序遍历

```javascript
// 递归版本
function traverse(root) {
  if (!root) {
    return
  }
  console.log(root.val)
  if (root.left) {
    traverse(root.left)
  }
  if (root.right) {
    traverse(root.right)
  }
}
// 迭代版本
function traverse_i(root) {
  if (!root) {
    return
  }
  const stack = []
  root.push(root)
  while(stack.length !== 0) {
    root = stack.pop()
    console.log(root)
    // 注意以下节点必须先右再左
    if (root.right) {
      stack.push(root.right)
    }
    if (root.left) {
      stack.push(root.left)
    }
  }
}
```

#### 中序遍历

```javascript
// 递归版本
function traverse(root) {
  if (!root) {
    return
  }
  if (root.left) {
    traverse(root.left)
  }
  console.log(root.val)
  if (root.right) {
    traverse(root.right)
  }
}
// 迭代版本
function traverse_i(root) {
  const stack = []
  while(true) {
    if (root) {
      stack.push(root)
      root = root.left
    } else if (stack.length !== 0) {
      root = stack.pop()
      console.log(root.val)
      root = root.right
    } else {
      break
    }
  }
}
```

#### 后序遍历

```javascript
function traverse(root) {
  if (!root) {
    return
  }
  if (root.left) {
    traverse(root.left)
  }
  if (root.right) {
    traverse(root.right)
  }
  console.log(root.val)
}
```

#### 层次遍历

```javascript
function traverse(root) {
  let queue = new Queue()
  queue.enqueue(root)
  while(!queue.empty()) {
    const node = queue.dequeue()
    console.log(node)
    if (node.left) {
      queue.enqueue(node.left)
    }
    if (node.right) {
      queue.enqueue(node.right)
    }
  }
}
```