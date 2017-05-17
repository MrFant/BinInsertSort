#include <stdlib.h>
#define MAX 5
using namespace std;
typedef int Type;
typedef struct {
	int cur;
	Type data;
}node,*Node;
struct staLinkList{
	Node elem;
	int maxSize;
	int n;		
};
void init(staLinkList &s,Type a[],int n){
	s.maxSize=MAX;
	s.n=n;
	s.elem=new node[MAX+1];
	if(s.elem==NULL){
		cerr<<"Fail to allocate space"<<endl;
		exit(1);
	}
	s.elem[0].data=MAX;
	s.elem[0].cur=1;
	for(int i=1;i<=n;i++){
		s.elem[i].data=a[i-1];
		s.elem[i].cur=i+1;
	}
	s.elem[n].cur=0;		//the last one,especially


}

void output(staLinkList &s){
	int i;
	for(i=1;i<=s.n;i++){
		cout<<s.elem[i].data<<endl;
	}
}
