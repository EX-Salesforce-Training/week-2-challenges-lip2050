public class POB {

    // FACTORIAL
   
    public static Integer nFactorial(Integer n)
{
    long ans = 1;
    if (n < 0) {
        System.debug('No negative numbers');
    }
    else
    {
    for (Integer i = 1; i <= n; i++) {
        ans = ans * i;
    }
    }
    System.debug(ans);
    return n;

    }
    
    
	//FIBONACCI SEQUENCE

	public static Integer nfibonacci (Integer n){
    integer a=1;
    integer b=0;
    integer c=0;
    if (n==0){
        return n;
    }else{
	for (integer i=0; i<n; i++){
       
    c=a+b;
    a=b;
    b=c;
}
    system.debug(c);  
        return c;
    }
}
    
    
    
	// SORT
	    
    public static List<Integer> SortArray(List<Integer>intList){
        Integer Lee;
        boolean change =false;
        do{
            change = false;
        for (Integer i=0; i< intList.size(); i++){
            if(intList[i] > IntList[i+1]){
                change= true;
                Lee = intList[i+1];
                intList.set(intList[i+1],intList[i]);
                intList.set(intList[i],Lee);
            }
            }
        }while(change);
        return intList;
            
    }
 
    
    //LEFT ROTATION
     
   public static Integer[] rotateLeftNTimes( Integer[] aray, Integer n){
       List<integer> newAray = new List<integer>(aray);
    integer p;
       integer en = newAray.size();
       integer x = n;
       if (n>=en){
           x = math.mod(n,en);
       }
    for (Integer i=0; i<=x; i++){
        
        p=newAray.get(0);

        newAray.remove(0);

        newAray.add(p);
       }
 system.debug(newAray);
return newAray; 
   }





// Balance Brackets 

    public static Boolean bracketsAreBalanced( String s ){
    	
         String[] brc =s.split('');
        
        for (Integer i=0; i < brc.size(); i++){
        if(brc[i] == '(' || brc[i] == '{' || brc[i] =='['){
            return true;
        }
        if(brc[i] == ')' || brc[i] == '}' || brc[i] == ']'){
            return true;
        } 
        else{
        return false;
    }
       
    }
      return false;  
    }
    
    
}
