# Move-all-zero-at-the-end-of-array
move all zero at end
void moveZeroes(vector<int>& a) {

    int j=0;
    for (int i = 0; i < a.size(); i++)
     {
        if (a[i] != 0) {  \\ check the condition ..if it is non zero value then swap it with j position value...
                            \\for zero value skip ...i will increase because of for loop but j remain in the same position.
                         swap(a[i],a[j]);
                          j++;
                       }
      }  
}
int main() {
    vector<int> a = {1,0,2,0,0, 3,0};
     moveallzero(a);
       for(int num: a)
        {cout<<num<< " ";}

    return 0;
}
