# Array-codes

1.Write a program that asks the user for the number of elements (assume at most
100), reads that many integers into an array, and then calculates and displays
the sum of the array elements.

#include <.iostream>
<br>
using namespace std;

int main() {

    int n, arr[100], sum = 0;

    cout << "Enter the number of elements and it should be between 100: ";
    cin >> n;


    if(n < 1 || n > 100)
        {
        cout << "Invalid number of elements declared!" << endl;
        }
    else
        {

        cout << "Enter " << n << " integers:" << endl;
        for(int i = 0; i < n; ++i)
        {
            cin >> arr[i];
            sum =sum+arr[i];
        }

        cout << "The sum of the array elements: " << sum << endl;
    }

    return 0;
}

2.Write a program that reads a list of integers into an array and then determines
and prints the maximum and minimum values among them.

#include <.iostream>
<br>
using namespace std;

int main() {
<br>
    int n, arr[100];

    cout << "Enter the number of elements (max 100): ";
    cin >> n;

    if(n < 1 || n > 100)
        {
        cout << "Invalid number of elements!" << endl;
        }
    else
        {

        cout << "Enter " << n << " integers:" << endl;
        for(int i = 0; i < n; ++i)
        {
            cin >> arr[i];
        }


        int maxedValue = arr[0];
        int miniValue= arr[0];

        // Find max and min
        for(int i = 1; i < n; ++i) {
            if(arr[i] > maxedValue)
                maxedValue= arr[i];
            if(arr[i] < miniValue)
                miniValue = arr[i];
        }

        // Display results
        cout << "Maximum value: " << maxedValue << endl;
        cout << "Minimum value: " << miniValue << endl;
    }

    return 0;
}

3.Write a program that reads a sequence of integers into an array and then
reverses the array in place. Finally, display the reversed array.

#include <.iostream>

using namespace std;

int main()
<br>
{
    int m,arr[10],i;

    cout<<"Enter the size of the array : ";
    cin>>m;
    cout<<"Enter the elements of the array : ";

    for(i=0;i<m;i++)
    {
        cin>>arr[i];
    }
    cout<<"Actual array is:";

    for(i=0; i<m; i++)
    {
        cout<<arr[i]<<" ";
    }
    cout<<endl;

    cout<<"Reversed array is:";

    for(i=(m-1); i>=0; i--)
    {
        cout<<arr[i]<<" ";
    }
    return 0;

}



