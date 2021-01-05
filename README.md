#include <iostream>
using namespace std;
int main(void){
    
    char x[1000];
    int K,count=0;
    int i;
    
    cout << "現在の西暦を入力してください:";
    cin >> x;
    cout << x << "年" << endl;
    
    cout << "Kの値を入力してください:";
    cin >> K;
    cout << K << endl;
    
    for(i=0;x[i];i++){
        if(x[i] == '0'){
            count++;
        }
    }
    cout << "桁数：" << i << endl;
    cout << "0の数：" <<count+1 << endl;
    
    if(count+1 > K){
        cout << "Yes" << endl;
    }
    else{
        cout << "No" << endl;
    }
    
    
    return 0;
    
}
