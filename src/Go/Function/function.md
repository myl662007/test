## 函数、包和错误处理

- 函数
    
        函数：为完成某一功能的程序指令(语句)的集合
        函数分为: 自定义函数、系统函数
        
        func 函数名（形参列表)(返回值列表){}

- 包
    
        包的基本概念：go 的每一个文件都是属于一个包的，也就是说 go 是以包的形式来管理文件和项目目录结构的
        
        包的三大作用：
            区分相同名字的函数、变量等标识符 
            当程序文件很多时,可以很好的管理项目 
            控制函数、变量等访问范围，即作用域

注意：go语言中没有private和public等，通过首字母大小写控制是否能被其他包调用


- init函数

        每一个源文件都可以包含一个 init 函数，该函数会在 main 函数执行前，被 Go 运行框架调用，也 就是说 init 会在 main 函数前被调用。

- 匿名函数
        
        匿名函数就是没有名字的函数，如果我们某个函数只是希望使用一次，可以考 虑使用匿名函数，匿名函数也可以实现多次调用。
        
        案例：
        
        func main(){
        	res1 := func (n1 int, n2 int) int{
        		return n1+n2
        	}(10,20)
        
        	fmt.Println("res=",res1)
        }