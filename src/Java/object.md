##面向对象

- 什么是面向对象：

- 类和对象的概念

  	    类：是一组相关的属性和行为的集合
  		对象：是该类事物的具体体现

- 定义类其实就是定义类的成员
  	    
  	    成员变量	和以前定义变量是一样的，只不过位置发生了改变。在类中，方法外。
  		成员方法	和以前定义方法是一样的，只不过把static去掉，后面在详细讲解static的作用。

- 类（抽象的）
    
        类是模子，确定对象将会拥有的特征（属性）和行为（方法）
    
        定义一个类：
            public class 类名{
                //属性部分（成员变量）
                //属性方法
            }
        
        定义一个类的时候首字母要大写
        
        成员变量和局部变量：
        成员变量：类的属性
        局部变量：类的成员方法中定义的变量
        注意：Java中局部变量没有初始值，成员变量有初始值

- 对象（客观存在的）
    
        对象的属性：
    
        对象的方法：

- 构造方法：
        
        作用：创建一个新的对象
        
        定义：
            public 构造方法名(){
                //1.没有返回值类型
                //2.与类名相同
                //3.可以指定参数
            }
        
        构造方法也可以进行方法的重载

- 方法重载：
        
        方法名相同，参数个数，类型不同的方法
        
- 静态成员：(static使用之静态变量)
        
        静态成员可以使用类名直接访问，也可以使用对象名进行访问
        
- 静态方法：
        
        1.静态方法中可以直接调用同类中的静态成员，但不能直接调用非静态成员
        
        2.静态方法中调用非静态变量，可以创建类的对象，然后通过对象来访问非静态变量
        
        3.在普通成员方法中，则可以直接访问同类的非静态变量和静态变量
        
        4.静态方法中不能直接调用非静态方法，需要通过对象来访问非静态方法

- 静态初始化块
        
        静态初始化块只在类加载时执行，且只会执行一次，同时静态初始化块只能给静态变量赋值，不能初始化普通的成员变量
        
        初始化块定义：
        static{
        }
        
- 面向对象特征
		
        封装(encapsulation)
        继承(inheritance)
        多态(polymorphism)
        
- 封装：

        1.修改属性的可见性 private
        
        2.创建getter/setter方法（用于属性的读写）
        
        3.在getter/setter方法中加入属性控制语句
        
- this关键字
        
        当前对象

- super关键字

        1.获取父类对象的值
        2.如果放在子类的构造方法中，需要放到第一行，调用父类的构造方法
        
- object对象
        
        tostring
        
        equals()方法        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        

