public class Remove {
    // Removing 'a' from string
    static String remove(String s, int idx) {
        if(idx == s.length()) 
        return " ";
        String smallAns = remove(s, idx +1); // recursion
        char currChar = s.charAt(0);
        
        if(currChar != 'g') { // checking for current char
            return currChar + smallAns;
         } else {
            return smallAns;
         }
        }
        public static void main(String[] args) {
            Scanner sc = new Scanner(System.in);
            String s = sc.nextLine();
            System.out.println(remove(s,0));
        }
    }
    

