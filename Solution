import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) throws IOException  {
        /* Enter your code here. Read input from STDIN. Print output to STDOUT. Your class should be named Solution. */
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        String input;
        List<String> myStack = new ArrayList<String>();
        List<String> Stack = new ArrayList<String>();
        input=br.readLine();
        while ((input = br.readLine()) != null) {
            
            String[] full=input.split(" ");
            String command=full[0];
            if(command.equals("4"))
            {
                String thing=Stack.get(Stack.size()-1);
                if(thing.charAt(0)=='0')
                {
                    for(int i=0;i<thing.length()-1;i++)
                    {
                        myStack.remove(myStack.size()-1);
                    }
                    Stack.remove(Stack.size()-1);
                    //System.out.println(myStack);
                }
                
                if(thing.charAt(0)=='1')
                {
                    
                    for(int k=thing.length()-1;k>0;k--)
                    {
                        myStack.add(Character.toString(thing.charAt(k)));
                    }
                        
                        Stack.remove(Stack.size()-1);
                        //System.out.println(myStack);
                }
            }
            if(full.length>1)
            {
            String operation=full[1];
            if(command.equals("1"))
            {
                
                for(int i=0;i<operation.length();i++)
                {
                    myStack.add(Character.toString(operation.charAt(i)));
                    
                }
                String code;
                code="0"+operation;
                Stack.add(code);
                
            }
            
            if(command.equals("2"))
            {
                
                String code="1";
                for(int i=0;i<Integer.parseInt(operation);i++)
                {
                    if(myStack.size()!=0){
                    code=code+myStack.get(myStack.size()-1);
                    myStack.remove(myStack.size()-1);
                    
                    
                    }
                }
                Stack.add(code);
                //System.out.println(Stack);
                //System.out.println(myStack);
                
            }
            if(command.equals("3"))
            {
                System.out.println(myStack.get(Integer.parseInt(operation)-1));
                //System.out.println(myStack);
            }

            }
        }
        br.close();
    }
}
