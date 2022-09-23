## HackerRank_JAVA_solutions
Java task solutions at HackerRank

- [Simple Array Sum](https://www.hackerrank.com/challenges/simple-array-sum/problem) 
        
        public static int simpleArraySum(List<Integer> ar) 
        {    
          int sum = 0;
          for(int i : ar)
            {
               sum += i;
            }
          return sum;
        }

- or:
   
        public static int simpleArraySum(List<Integer> ar)
        {
                int sum = 0;
                for(int i = 0; i < ar.size(); i++)
                {
                        sum += ar.get(i);
                }
                return sum;
        }
        
- []() 
