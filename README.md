# ex_6.42
one of my exercises of C++,

//给make_plural函数（p201）的第二个形参赋予默认实参's'，利用新版本的函数输出单词success和failure的单数和复数形式
//.
//.

	#include<iostream>
	#include<string>

	using std::string;
	using std::cout;
	using std::endl;

	string make_plural(size_t ctr, const string &word,const string &ending = "s") 
	{
		return (ctr>1) ? word+ending : word;						  			
	}

	int main()
	{
		cout<<"单数："<<make_plural(1, "success")<<" "
					<<make_plural(1, "failure")<<endl;
		cout<<"复数："<<make_plural(2, "successe")<<" "
					<<make_plural(2, "failure")<<endl;
		return 0;
	}
