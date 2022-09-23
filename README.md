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
        
- [A Very Big Sum](https://www.hackerrank.com/challenges/a-very-big-sum/problem?h_r=profile) 

        public static long aVeryBigSum(List<Long> ar) {
    
                Long longInteger = 0L;
                for(Long i: ar)
                {
                longInteger += i;        
                }
                return longInteger;
        }
