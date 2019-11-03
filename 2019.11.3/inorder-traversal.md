# Inorder-traversal

中序遍历:先遍历左子树 再根节点 后右子树 

遍历元素不需要返回什么

还是写一个对于用户公有的方法

```
public void inorder(){
    inorder(root);
}
```

***

在私有方法中 我们要遍历以node为根节点的二分搜索树

#### 1所以传入参数根节点

```
private void inorder(Node node){
}
```

***

#### 2递归终止条件

```java
if(node == null)
  return;
```

***

#### 3遍历左节点 因为是中序遍历 先找到左节点 再打印左节点

```java
inorder(node.left);
System.out.println(node.e);
```

***

#### 4遍历右子树

```java
inorder(node.right);
```

***

#### 5二分搜索树的中序遍历结果是顺序的 从小到大

