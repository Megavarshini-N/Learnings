1 class and object
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
void update(int *a,int *b)
{
    int sum=*a+*b;
    int diff=abs(*a-*b);   
    *a=sum;
    *b=diff;
}

int main()
{
    int a, b;
    int *pa = &a, *pb = &b;
    
    scanf("%d %d", &a, &b);
    update(pa, pb);
    printf("%d\n%d", a, b);

    return 0;
}

3
using namespace std;
int main() {
    int i;
    long l;
    char c;
    float f;
    double d;
    scanf("%d %ld %c %f %lf", &i, &l, &c, &f, &d);
    printf("%d\n", i);
    printf("%ld\n", l);
    printf("%c\n", c);
    printf("%.3f\n", f);
    printf("%.9lf\n", d);

    return 0;
}

3
#include<iostream>
using namespace std;
int arra(int arr[],int n)
{
    int s=0,t;
    int e=n-1;
    while(s<e)
    {
        t=arr[s];
        arr[s]=arr[e];
        arr[e]=t;
        s++;
        e--;
    }
    return 0;
}
void pri(int arr[],int n)
{
    int i;
    for(i=0;i<n;i++)
    {
        cout<< arr[i]<<" ";
    }
}
int main() {
     int arr[1000],i,n;
     cin>>n;
     for(i=0;i<n;i++)
     {
        cin>>arr[i];
     }
     arra(arr, n);
     pri (arr, n);
    return 0;
}
