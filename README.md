# HashMap-in-Java-

import java.util.*;

class Main{
    public static void main (String[] args) {
    
     HashMap<String ,Integer> map = new HashMap<>();
     map.put("A",2);
     map.put("B",3);
     map.put("C",4);
     
     System.out.println(map);
     
     map.put("C",9); // update value in the map
     System.out.println(map);
     
     // Search Element in Map
     if(map.containsKey("S")){
         System.out.println("key is exsit");
     }
     else{
         System.out.println("key is not present");
     }
     
     // key exsits in java
     System.out.println(map.get("A")); // value print
     System.out.println(map.get("M")); // Null print
     
     // Iteration in HashMap
    for( Map.Entry<String, Integer> s : map.entrySet()){;
     System.out.println(s.getKey()+" ");
     System.out.println(s.getValue()+" ");
    }
    
     // keySet  only value
     Set<String> keys = map.keySet();
     for(String i: keys){
         System.out.println(i + " " +map.get(i));
     }
     
     
     // Remove value in HashMap
     map.remove("A");
     System.out.println(map);
     
    }
}




