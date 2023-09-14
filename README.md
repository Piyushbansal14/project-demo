# project-demo
#include <iostream>

using namespace std;
class A 
{
    int x,y;
    public:
    virtual void data()
    {
        cout<<"You are in class A";
    }
};

class B:public A
{
    int x,y;
    public:
    void data()
    {
        cout<<"You are in class B";
    }
    
};
int main()
{
    B*o;
    A a;
    B b;
    o=&b;
    o->data();
    o=(B*)&a;
    o->data();
    
}
