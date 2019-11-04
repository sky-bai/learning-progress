# Generics

```java

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		MyCollection<String> mc = new MyCollection<String>();
		mc.set("bai", 0);
		mc.set(8888,1);
		//里面只能传string
		String b = (String)mc.get(0);
		

		
		
	}

}
// mycollection 里面放入里牛肉羊肉 这里的E相当于形参
class MyCollection<E>{
	//这个容器能放5个对象 
	Object[]  objs = new Object[5];
	
	//set方法 设置容器里面每一个对象的值 传入对象 传入对象位置
	public void set(Object obj, int index) {
		objs[index] = obj;
		}
	//获得对应索引位置的内容 传个索引位置 我把对应索引位置的内容传出去 所以方法的类型为 Object
	public E get(int index) {
	    return (E)objs[index];	
	}
	
	
}

```

对于generics 我把语法搞清 在创建类对象的时候只需要注意我要用什么参数 

能让我写出类型安全性的集合

能让编译器防止我把cat放入pat中

什么东西有什么用 找清框架 马上细分

