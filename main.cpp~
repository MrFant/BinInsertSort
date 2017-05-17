#include<iostream>
#include"dataList.h"
using namespace std;
void BinaryInsertSort(staLinkList &s){
	node temp;
	int i,j,low,high,mid;
	for(i=2;i<=s.n;i++){
		if(s.elem[i-1].data>s.elem[i].data){
			temp=s.elem[i];
			low=1;
			high=i-1;
			while(low<=high){
				mid=(low+high)/2;
				if(temp.data<s.elem[mid].data){
					high=mid-1;
				}
				else
					low=mid+1;

			}
			for(j=i-1;j>=low;j--)
				s.elem[j+1]=s.elem[j];
			s.elem[low]=temp;
		}
	}
}
int main(){
	int a[5]={5,6,9,8,2};
	staLinkList s;
	init(s,a,5);
	BinaryInsertSort(s);
	output(s);
	return 0;

}

