#include<iostream>

using namespace std;

class student{



 private:

     string name;
     int age;

    public:
        void data(string s,int a)
        {
            name=s;
            age=a;
        }





    void show(){
        cout<<"name"<<name;
        cout<<"age"<<age;
    }

}s1,s2;

int main()
{
    pair<int ,string>p1;
    pair<int, student>p2;

    p1=make_pair(23,"nitin");
     s1.data("balli",45);
    p2=make_pair(34,s1);

    cout<<p1.first<<" "<<p1.second;
    cout<<p2.first<<" ";
    s2=p2.second;
    s2.show();
}

