#include<fstream.h>
#include<stdio.h>
#include<stdlib.h>
class stud
{  char section; int clas;
char name[20]; int rollno;
public:
void getdata()
{cout<<"Enter name, clas, rollno and section ";
gets(name);
cin>>clas>>rollno>>section;
}
void putdata()
{ cout<<"name="<<name<<"\n";
cout<<"class="<<clas<<section<<"\n";
cout<<"rollno"<<rollno<<"\n";
}
int getrno()
{return rollno; }
void modify()
{ cout<<"name="<<name<<"\n";
cout<<"class="<<clas<<section<<"\n";
cout<<"rollno"<<rollno<<"\n";
char nm[20]=" ",sec[4]=" ";
int cls;
cout<<" enter new name";
cin>>nm;
cout<<"enter new clas";
cin>>cls;
cout<<"enter new section";
cin>>sec;
}};
void main()
{ ofstream fout;
  char ans;   int d;
  stud s;
fout.open("stud.dat",ios::out)
while(ans=='y'||ans=='Y')
{  s.getdata();
fout.write((char*)&s,sizeof(s));
cout<<" Want to enter more records (y/n)";
cin>>ans;
}
fout.close();
cout<<"enter 1 for inserting more data serial wise";
cout<<"enter 2 for searching data";
cout<<"enter 3 for deleting a record";
cout<<"enter 4 for modifying data";
cout<<"enter 5 for entering more data";
switch(d)
{ case 1:
{
ifstream fin.open("stud.dat",ios::in)
ofstream fout.open("temp.dat",ios::out)
char last='y';
cout<<"enter details of student whose record is to be inserted";
stud s1,s2;
s1.getdata();
while(fin)
{fin.read((char*)&s2,sizeof(s2));
if(s1.getrno()<=s2.getrno())
{fout.write((char*)&s1,sizeof(s1));
last='n';
break; }
else
fout.write((char*)&s2,sizeof(s2));  }
if(last=='y')
fout.write((char*)&s1,sizeof(s1));
else if(fin)
{ while(fin)
{fout.read((char*)&s2,sizeof(s2));
fout.write((char*)&s2,sizeof(s2));
 }
fin.close() ;
fout.close();
remove("stud.dat");
rename("temp.dat","stud.dat");
fin.open("stud.dat",ios::in);
cout<<" file now contains \n";
while(fin)
{  fout.read((char*)&s2,sizeof(s2));
   if(fin) break;
   stud.putdata(); }
   fin.close();
 } }
 break;
 case 2:
{int rn; stud s1;
char found='n';
cout<<"enter the rollno you have to search";
cin>>rn;
while(fin)
{   fout.read((char*)&s1,sizeof(s1));
    if(s1.getrno()==rn)
    {s1.putdata();
    found='y';
    break;
    }}
    if (found='n')
    cout<<"rollno is not found in file"<<endl;
    fin.close(); }
case 3 :
{ifstream fin.open("stud.dat",ios::in)
ofstream fout.open("temp.dat",ios::out)
int rno; char found='f',confirm='n';
stud s1;
cout<<" enter rollno to be deleted"  ;
cin>>rno;
while(fin)
(  fout.read((char*)&s1,sizeof(s1));
 if(s1.getrno()==rno)
 { s1.putdata;
 found='t';
 cout<<"Are nyou sure you want to delete this record?(y/n);";
 cin>>confirm;
 if(confirm=='n')
 fin.write((char*)&s1,sizeof(s1);
 }
 else
  fin.write((char*)&s1,sizeof(s1);  }
  if(found=='f')
  cout<<" record not found \n";
  fout.close();
  fin.close();
  remove("stud.dat ")
  rename("temp.dat","stud.dat")
  fin.open("stud.dat",ios::in);
cout<<" file now contains \n";
while(fin)
{  fout.read((char*)&s2,sizeof(s2));
   if(fin) break;
   stud.putdata(); }
   fin.close();
 }  }
 break;
 case 4:
 { fstream fio("stud.dat",ios::in|ios::out|ios::binary)
 int rno;long pos; char found'f';
 stud s1;
 cout<<"enter rollno of studet to be modified \n";
 cin>>rno;
 while(fio)
 { pos=fio.tellg();
 fio.read((char*)&s1,sizeof(s1));
 if(s1.getrno()==rno)
 { s1.modify();
 fio.seekg(pos);
 fio.write((char*)&s1,sizeof(s1));
 found='t';
 break;}}
 if(found=='f')
 cout<<" record not found \n" ;
 fio.seekg(0);
 stud s2;
 cout<<" file now contains \n";
while(fin)
{  fout.read((char*)&s2,sizeof(s2));
   if(fin) break;
   stud.putdata(); }
   fin.close();
 } }
 break;
 case 5:
 {ofstream fout("stud.dat",ios::app);
 char ans='y'; stud s1;
 while(ans=='y'||ans=='Y')
 {s1.getdata();
 fout.write((char*)&s1,sizeof(s1));
 cout<<"Record added to file \n";
 cout<<"Want to enter more records?(y/n)";
 cin>>ans;
 }
 fout.close()   }
 break;
 }}
