#include <bits/stdc++.h>
#include <iostream>
#include <string>
#include <windows.h>
using namespace std;
void loading()
{
    char a = 177, b = 219;
    cout <<"\t\t\t\t\t\t\t\tLoading...\n\n";
    cout<<"\t\t\t\t\t\t\t";
    for(int i=0; i<26;i++)
    {
       cout<<a;
    }
    cout <<"\r";
    cout<<"\t\t\t\t\t\t\t";
    for(int i=0;i<26;i++)
    {
        cout << b;
        Sleep(100);
    }
    cout << endl;
    cout << endl;
    cout<<"\n                                                CHAO MUNG DEN VOI BO TOC MIXI GAMING !!!";
    Sleep(1000);
    system("cls");
    system("color F");
}
int main()
{

    fstream filein;
    filein.open("dotoc.txt",ios_base::in);
    cout <<"                                             ****  Xin chao ! My name is Huu Hieu  ****"<< endl;
    cout <<"                                                  ***   FROM MIXI WITH LOVE   ***  "<<endl;
    cout<<endl;
    cout<<"                                              ============================================"<<endl;
    string a;
    string pass ="HuuHieu";
    cout<<"                                              Nhap Ten de xac minh ban la Tac gia : "; cin >> a;
    if( a == pass)
    {
    cout <<"                                                       XAC NHAN BAN LA TAC GIA !"<<endl;
    loading();
    fstream newfile;
    newfile.open("dotoc.txt",ios::in);
    if(newfile.is_open())
    {
        string s;
        while(getline(newfile,s))
        {
            cout <<"\t\t\t "<< s << endl;
            Sleep(100);
        }
        newfile.close();
    }
    system("pause");
    return 0;
}
if( a != pass) cout <<"                                                    Ban KHONG phai la Tac gia !\n\n\n\n";
}
