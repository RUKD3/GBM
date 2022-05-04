---
title: "CODING"
date: 
draft: false
menu: Project
# category : "post"
# series : "post"
# tag : "Unity"
---
## coding by  C++
\
\
一个简单的HP模拟，询问当前的操作，并输出当前玩家的状态
\
\
\
```
#include <iostream>
#include <string>

using namespace std;

int main()
{
    int hp = 50;
    char ch = 'n';
    int change = 0;


    cout << "初始HP为" << to_string(hp) << endl;

    cout << "请选择 伤害 或 治疗，用字母a或b表示" << endl;
    cin >> ch;

    cout << "请输入伤害或治疗的数值" << endl;
    cin >> change;


    if (ch == 'a' || ch == 'b')
    {
        if (ch == 'a')
        {
            cout << "您选择了伤害" << to_string(change) << endl;
            hp -= change;
        }
        else
        {
            cout << "您选择了治疗" << to_string(change) << endl;
            hp += change;
        }


        if (hp > 100)
        {
            hp = 100;
        }
        if (hp < 0)
        {
            hp = 0;
        }


        cout << "玩家当前HP为" << to_string(hp) << endl << "当前玩家状态为";

        if (hp <= 0)
        {
            cout << "死亡";
        }
        else if (hp < 20)
        {
            cout << "濒死";
        }
        else if (hp < 80)
        {
            cout << "正常";
        }
        else
        {
            cout << "完美";
        }


    }
    else
    {
        cout << "请重新输入";
    }

    return 0;

}

```
\
\
\
## OUTPUT

![001](../../images/output.png)