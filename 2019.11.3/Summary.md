# Binary tree traversal summary

#### preorder traversal

```java
private void preorder(Node node){
  if(node == null)
  return;
    
    System.out.println(node.e);
    preorder(node.left);
    preorder(node.right);
}
```

***

inorder traversal 

```java
private void inorder(Node node){
  if(node == null)
  return;
  
    inorder(node.left);
    System.out.println(node.e);
    inorder(node.right);
}
```

postorder traversal

```
private void postorder(Node node){
  if(node == null)
  return;
  
    postorder(node.left);
    postorder(node.right);
    System.out.println(node.e);
  
}
```

总结：前中后 二分搜索树的中序遍历结果是顺序的 从小到大