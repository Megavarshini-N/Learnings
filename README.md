1
#include <iostream>
class Student
{
private:
    int scores[5];

public:
    void input() 
    {
        for (int i = 0; i < 5; i++) 
        {
            std::cin >> scores[i];
        }
    }

    int calculateTotalScore() 
    {
        int total = 0;
        for (int i = 0; i < 5; i++)
        {
            total += scores[i];
        }
        return total;
    }
};


2
#include<cstdlib>
void update(int *a,int *b) {
    int sum=*a+*b;
    int diff=abs(*a-*b);   
    *a=sum;
    *b=diff;
}

int main() {
    int a, b;
    int *pa = &a, *pb = &b;
    
    scanf("%d %d", &a, &b);
    update(pa, pb);
    printf("%d\n%d", a, b);

    return 0;
}
