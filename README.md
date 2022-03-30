##include<stdio.h>

int acc(int rehea[3][2], int ID, int PIN) {
    
    int gabaya=0;
    
    for(int i=0;i<3;i++) {
        
        if(ID==rehea[i][0] && PIN==rehea[i][1]){
            
            gabaya=1;
        }
    }
    return gabaya;
}
int main(){
   
     int rehea[3][2]={{1234,1111},{2345,2222},{3456,3333}};
  
      int ID, PIN;
 
       printf("ENTER ID NUMBER:");
  
      scanf("%d",&ID);
 
       printf("ENTER PIN:");
  
      scanf("%d",&PIN);
    
  
      if(acc(rehea,ID,PIN))
    {
       
         printf("YOU HAVE SUCCESSULLY LOGGED IN\nID#:%d",ID);
    }    
    
    
      else {
       
         printf("INVALID ID/PIN");
    }
    return 0;
