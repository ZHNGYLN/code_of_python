from random import randint
import os
class Star:
    def __init__(self):  #这个模块开始的时候就创建
        self.position = randint(0,23)
    def left(self):
        if(self.position >=1):
            self.position-=1

    def right(self):
        if(self.position <23):
            self.position+=1  #设成相应的self的变量

    def draw(self):
        print("."*self.position+"*"+"."*(23-self.position))

if (__name__ == "__main__"):  #当这个文件在其他文件中被import，下面的代码不会执行
    isRunning = True
    star = Star()
    while(isRunning == True):
        os.system("cls")  #命令行清屏cls在win，clear是linux
        star.draw()
        command = input("请输入移动星星的指令（L/l or R/r）：") # input从终端键盘输入
        if(command.upper() == 'L'):  #upper变成大写字母
            star.left()
        if(command.upper() == 'R'):  
            star.right()
        if(command.upper()=="EXIT"):
            isRunning = False