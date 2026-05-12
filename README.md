# hostel-management-system
    #include<iostream>
using namespace std;
class hostel{
	private:
		string student_name;
		string fathername;
		int age;
		int room_no;
		
		 
		 public:
			void setname(){
					cout<<"*****************************************"<<endl;
				 cout<<"welcome to this hostel:"<<endl;
			cout<<"ARROMA_BOYS_ HOSTEL"<<endl;
			
				cout<<"*****************************************"<<endl;
			cout<<"enter the  student name:"<<endl;
				cin>>student_name;
			}
		  
				void setfname(){
				
				  	cout<<"*****************************************"<<endl;
			 	cout<<"enter the  father name:"<<endl;
				cin>>fathername;
			}
				 void setyear(){
				 
			cout<<"enter the age of student:"<<endl;
				cin>>age;
					cout<<"*****************************************"<<endl;
			}
			
			void setarea(){
				
					cout<<"*****************************************"<<endl;
						 
			
				cout<<"allote the room ::"<<endl;
				cin>>room_no;
			}
			
			
			
				
				void display(){
					cout<<"name"<<student_name<<endl;
					cout<<"age"<<age<<endl;
					cout<<"room no"<<room_no<<endl;
					
						cout<<"*****************************************"<<endl;
				}
				
		};
		
	  	 
			 class rooms:public hostel{
			 	protected:
			 		int roomofsize;
			 		int noofbathrooms;
			 		
			 		public:
			 			
			 			rooms(int rs,int nb){
			 				roomofsize=rs;
			 				noofbathrooms=nb;
			 				
			 					cout<<"*****************************************"<<endl;
						 }
						 
						 void show(){
						 	cout<<"room size"<<roomofsize<<endl;
						 	cout<<"no of bathrooms"<<noofbathrooms<<endl;
						 	
						 		cout<<"*****************************************"<<endl;
						 }
			 };
			 
			 
			 class furniture:public hostel{
			 	protected:
			 		int bed;
			 		int ac;
			 		int roomcolor;
			 		
			 		public:
			 			void setbd(){
			 					cout<<"*****************************************"<<endl;
			 				cout<<"1 bed IS  avalible:"<<endl;
						 }
						 
						 void setAC(){
						 	cout<<"ac is avvalible::"<<endl;
						 	
						 		cout<<"*****************************************"<<endl;
						 }
						 void setcolour(){
						 	cout<<"enter the room color which u want::"<<endl;
						 	cin>>roomcolor;
						 		cout<<"*****************************************"<<endl;
						 		
						 		cout<<"..........................................."<<endl;
						 }
						  
			 };
			 
			 
	 
			 class mess:public hostel {
			 	protected:
			 	int rent;
			 	int bill;
			 	 
			 	public:
			 		
			 		//setter
			 		
			 		void setrent(int r){
			 			rent=r;
			 			cout<<"*****************************************"<<endl;
					 }
					 
					 void setbill(int b){
					 	bill=b;
					 	cout<<"*****************************************"<<endl;
					 }
					 
					 int getrent(){
					 	return rent;
					 	cout<<"*****************************************"<<endl;
					 }
					 
					 //getter
					 int getbill(){
					 	return bill;
					 	cout<<"*****************************************"<<endl;
					 }
			 	 
			 		  
			 	void display(){
			 		
			 		cout<<"room fee"<<rent<<endl;
			 		cout<<"bill"<<bill<<endl;
						 }
			 	
			 };
			 class food:public hostel{
			 	protected:
			 		int rice;
			 		int meat;
			 		
			 		public:
			 			void display(){
			 				cout<<"rice"<<rice<<endl;
			 				cout<<"meat"<<meat<<endl;
						 }
						 
			 };
			 
			 class security:public hostel{
			 	protected:
			 		string camera;
			 		int contact;
			 		
			 		public:
			 			
			 			security(string ca,int co){
			 				cout<<"*****************************************"<<endl;
			 				
			 				cout<<".......SECURITY............"<<endl;
			 				camera=ca;
			 				contact=co;
						 }
						 
						 void show(){
						 	cout<<"camera:"<<camera<<endl;
						 	cout<<"contact:"<<contact<<endl;
						 	cout<<"*****************************************"<<endl;
						 }
						  
			 };
			 
		  
int main(){
	hostel h1;
	h1.setname();
	h1.setfname();
	h1.setarea();
	h1.setyear();
	cout<<">>>>>>>>>>>>>>>>>"<<endl;
	
	
	
	rooms r1(150.5,1);
	r1.show();
		cout<<">>>>>>>>>>>>>>>>>"<<endl;
	
	
	
	
	furniture f1;
	f1.setbd();
	f1.setAC();
	f1.setcolour();
		cout<<">>>>>>>>>>>>>>>>>"<<endl;
	
	 
 mess m1;
 
 m1.setrent(20000);
 
 m1.setbill(2000);
 m1.display();
 	cout<<">>>>>>>>>>>>>>>>>"<<endl;
 	
 	int food[1];
 	for(int i=0;i<1;i++){
 			cout<<"*****************************************"<<endl;
 				cout<<"*****************************************"<<endl;
 					cout<<"*****************************************"<<endl;
 					
 					cout<<".......MENU............"<<endl;
 		cout<<"monday_wednesday avalible rice::"<<(i+1)<<endl;
 		cout<<"thursday_saturday avalible meat::"<<(i+1)<<endl;
	 }
	 
	 
	 security*s1=new security("cctv camera",92123);
	 s1->show();
	 cout<<"*****************************************"<<endl;
	 
 	
 	 
	return 0;
	
}
