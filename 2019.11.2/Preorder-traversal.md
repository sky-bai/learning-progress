# Preorder traversal

先写个共有方法 对于用户来说 只需要根节点 就是传入的参数root

对树的遍历 也不需要返回什么

```java
public void preOrder(){
      preOrder(root);
}
```

再写私有方法

前序遍历对以node为根的二分搜索树，递归算法

#### 1递归终止条件

如果节点遍历完了就返回

```
if(node == null)
return;
```

------

#### 2遍历节点开始打印

```java
System.out.println(node.e);
```

------

#### 3递归调用preorder

```java
preOrder(node.left);	
```

对于二分搜索树来说 根下面一定有节点 一直打印左字树 左子树打印完了再打印右子树

------

4递归调用preorder 打印右子树

```java
preOrder(node.right);	
```

------



```java
private void preOrder(){
    //先写递归终止条件
  if(node == null)
  return;
    //对于二分搜索树来说 先打印根节点再打印左子树 再打印右子树
    System.out.println(node.left);
    
    //再递归调用
    preOrder(node.left);
    preOrder(node.right);
    
}
```

