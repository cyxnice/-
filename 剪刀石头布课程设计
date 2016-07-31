#include <stdio.h>
#include <conio.h>
#include <stdlib.h>
#include <time.h>
void main()
{
	char Human,Computer;
	int i,j,win=0,lose=0,deuce=0,result;
	void menu1();              //菜单函数1.2.3的声明
	void menu2();
	void menu3();
	srand(time(NULL));
do
{	
win=0,lose=0,deuce=0;
menu1();
printf("请做出你的选择：");
scanf("%d",&i);
if(i==1)               //练习模式的开始
{ 	
	menu2();
	for(j=0;;j++)           //无限循环体的引入
	{
		printf("第%d场比赛开始",j+1);
		printf("你的选择(1、2、3): ");
	
	while(1)                      //设计人与电脑的对战的while循环
	{ 
		Human = getch();
		if(Human=='1'||Human=='2'||Human=='3'||Human=='4')
		{
			printf("%C\t",Human);break;
		}
	}                                                         //无限循环的结束
	if(Human=='4') break;
			switch(Human)     //判断开始游戏的真正对弈，人的主动选择
			{
			case '1': printf("石头VS ");break;
			case '2': printf("剪刀VS ");break;
			case '3': printf("布VS ");break;
			}
            Computer = rand()%3+1+48;
            switch(Computer)       //电脑的随机选择
			{ 
            case '1': printf("石头\n");break;
            case '2': printf("剪刀\n");break;
            case '3': printf("布\n");break;
			}
			result=Human-Computer;    //游戏结果的运算
			switch(result)       
			{
			case 0:deuce++;break;
			case -1:case 2:win++;break;
			case 1:case -2:lose++;break;
			}
	}
    printf("游戏结束\n");                         
	printf("----------------------------------\n");
	printf("***你和电脑一共决战了%d回合***\n",j);
	printf("***你赢了%d场，输了%d场****\n",win,lose);
	printf("----------------------------------\n");
	    if(win==lose)               //分出胜负
		{
    printf("***比赛结果：我们打成平手哦***\n");
		}
		else if(win>lose)
		{
    printf("***比赛结果：电脑，我赢了哦***\n");
		}
		else if(win<lose)
		{
	printf("***比赛结果：电脑，你赢了，但我不服，要再战一回合***\n");
		
		} 
}                                //对战模式的结束
else if(i==2)                    //游戏模式的开始 
{
	menu3();
	for(j=0;j<2;j++)               //for循环的开始，有限循环，满足两局一胜制
	{
		printf("第%d场比赛开始",j+1);
		printf("你的选择(1、2、3): ");
	  
	while(1)                            //设计人与电脑的对战的while循环
	{ 
		Human = getch();          
		if(Human=='1'||Human=='2'||Human=='3'||Human=='4')
		{
			printf("%C\t",Human);break;
		}
	}                            //for循环的结束
	if(Human=='4') break;
			switch(Human)                //判断开始游戏的真正对弈，人的主动选择
		
			{
			case '1': printf("石头VS ");break;
			case '2': printf("剪刀VS ");break;
			case '3': printf("布VS ");break;
			}
            Computer = rand()%3+1+48;
            switch(Computer)                 //电脑的随机选择
			{ 
            case '1': printf("石头\n");break;
            case '2': printf("剪刀\n");break;
            case '3': printf("布\n");break;
			}
			result=Human-Computer;      //游戏结果的运算
			switch(result)
			{
			case 0:deuce++;break;
			case -1:case 2:win++;break;
			case 1:case -2:lose++;break;
			}
		}
		printf("比赛结束\n");
		if(win==lose)                    //分出胜负
		{
            printf("我们打成平手哦\n");
		}
		else if(win>lose)
		{
			printf("电脑，我赢了哦\n");
		}
		else if(win<lose)
		{
			printf("电脑，你赢了，但我不服，要再战一回合\n");
		
		} 
}                                                   //游戏模式的结束
else if(i==3)
	printf("你退出游戏了哦\n");

}while(i==1||i==2);
}
void menu1()         //定义菜单函数1.2.3
{  
	printf("\t\t--------------------------------------------- \n");
	printf("\t\t|           欢迎来到石头剪刀布游戏           |\n");
	printf("\t\t|    ----------------------------------      |\n");
	printf("\t\t|                                            |\n");
	printf("\t\t|        说明:练习模式，请按1                |\n");
	printf("\t\t|             游戏模式，请按2                |\n");
	printf("\t\t|             退出游戏，请按3                |\n");
    printf("\t\t--------------------------------------------- \n");	
	return;
}
void menu2()
{
	printf("\t\t---------------------------------------------\n");
	printf("\t\t|              欢迎来到练习模式              |\n");
	printf("\t\t|    ----------------------------------      |\n");
	printf("\t\t|                                            |\n");
	printf("\t\t|      此游戏是用C语言实现的结构化程序       |\n");
	printf("\t\t|      设计，能够实现用户和电脑互对玩的      |\n");
	printf("\t\t|      过程，其中用户的出拳在下面有说明      |\n");
	printf("\t\t|                                            |\n"); 
	printf("\t\t|  用户操作:                                 |\n"); 
	printf("\t\t|                                            |\n");
	printf("\t\t|         1-石头 2-剪刀 3-布  4-退出         |\n"); 
	printf("\t\t|--------------------------------------------|\n");
	return;
}
void menu3()
{
	printf("\t\t---------------------------------------------\n");
	printf("\t\t|              欢迎来到对战模式              |\n");
	printf("\t\t|    ----------------------------------      |\n");
	printf("\t\t|                                            |\n");
	printf("\t\t| 说明:         三局两胜制                   |\n");
	printf("\t\t|      此游戏是用C语言实现的结构化程序       |\n");
	printf("\t\t|      设计，能够实现用户和电脑互对玩的      |\n");
	printf("\t\t|      过程，其中用户的出拳在下面有说明      |\n");
	printf("\t\t|                                            |\n"); 
	printf("\t\t|  用户操作:                                 |\n"); 
	printf("\t\t|                                            |\n");
	printf("\t\t|         1-石头 2-剪刀 3-布  4-退出         |\n"); 
	printf("\t\t|--------------------------------------------|\n");
	return;
}
