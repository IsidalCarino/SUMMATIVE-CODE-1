# SUMMATIVE-CODE-1
```
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string name;
    string age;
    cout << "\nEnter your fullname: \n";
    cin >> name;
    getline(cin, name);
    cout << "\nEnter your age: \n";
    cin >> age;
    getline(cin, age);
    cout << "\nEnter your grades (1-100): \n";
    double grd1;
    double grd2;
    cin >> grd1
        >> grd2;
    double sum = grd1 + grd2;
    double avg = sum / 2;
    cout << "Sum: " << sum << endl;
    cout << "Avg: " << avg << endl;
    cout << "\nEnter your average (copy from above BE HONEST!): \n";
    int marks;
    cin >> marks;
    if (cin.fail())
    {
        cin.clear();
        cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
        cout << "\nCOMMAND IS INCORRECT! PLEASE ENTER YOUR AVERAGE\n: ";
    }
    else if (marks > 100) {
        cout << "\nENTER YOUR PROPER AVERAGE MARK (HONESTY IS THE BEST POLICY)\n";
    }
    else {
        switch (marks / 10)
        {
        case 10:
        case 9:
        case 8:
        case 7:
        {   cout << "Name: Mr./Ms. " << name << endl << "Your grade is A.\n";
        break;
        }
        case 6:
        {   cout << "Name: Mr./Ms. " << name << endl << "Your grade is B.\n";
        break;
        }
        case 5:
        {   cout << "Name: Mr./Ms. " << name << endl << "Your grade is C.\n";
        break;
        }
        case 4:
        {   cout << "Name: Mr./Ms. " << name << endl << "Your grade is D.\n";
        break;
        }
        case 3:
        case 2:
        case 1:
        case 0:
        {   cout << "Name: Mr./Ms. " << name << endl << "Your grade is F.\n";
        break;
        }
        default:
        {cout << "INVALID INPUT!\n";
        }
        }
    }
}
```
