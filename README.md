# SUMMATIVE-CODE-1
```
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string name;
    cout << "\nEnter your fullname and age (FORMAT: Name, Age): \n";
    cin >> name;
    getline(cin, name);
    cout << "\nEnter your grades (1-100): \n";
    double grd1;
    double grd2;
    cin >> grd1
        >> grd2;
    double sum = grd1 + grd2;
    double avg = sum / 5;
    cout << "Sum: " << sum << endl;
    cout << "Avg: " << avg << endl;
    cout << "Enter your average (copy from above): \n";
    int marks;
    cin >> marks;
    if (cin.fail())
    {
        cin.clear();
        cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
        cout << "COMMAND IS INCORRECT! PLEASE ENTER YOUR AVERAGE\n: ";
    }
    else if (marks > 100) {
        cout << "ENTER YOUR PROPER AVERAGE MARK (HONESTY IS THE BEST POLICY)\n";
    }
    else {
        switch (marks / 10)
        {
        case 10:
        case 9:
        case 8:
        case 7:
        {   cout << name << ", Your grade is A.\n";
        break;
        }
        case 6:
        {   cout << name << ", Your grade is B\n";
        break;
        }
        case 5:
        {   cout << name << ", Your grade is C\n";
        break;
        }
        case 4:
        {   cout << name << ", Your grade is D\n";
        break;
        }
        case 3:
        case 2:
        case 1:
        case 0:
        {   cout << name << ", Your grade is F\n";
        break;
        }
        default:
        {cout << "INVALID INPUT!\n";
        }
        cout << name << marks;
        }
    }
}
```
