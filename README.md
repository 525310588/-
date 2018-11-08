# -新式类和旧式类
新式类是广度优先,旧式类是深度优先
class A():
    def foo1(self):
        print "A"
class B(A):
    def foo2(self):
        pass
class C(A):
    def foo1(self):
        print "C"
class D(B, C):
    pass
    
d = D()
d.foo1()
新式类结果为：C
旧式类为：A
