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

        public static long aVeryBigSum(List<Long> ar) 
        {    
                Long longInteger = 0L;
                for(Long i: ar)
                {
                longInteger += i;        
                }
                return longInteger;
        }
        
- or:

        public static long aVeryBigSum(List<Long> ar) 
        {    
                Long longInteger = 0L;
                for(int i = 0; i < ar.size(); i++)
                {
                longInteger += ar.get(i);        
                }
                return longInteger;
        }

- [Compare the Triplets](https://www.hackerrank.com/challenges/compare-the-triplets/problem?h_r=profile)

        public static List<Integer> compareTriplets(List<Integer> a, List<Integer> b) 
         {        
        
                Integer[] result = {0,0};
                for(int i=0; i < a.size(); i++)
                {
                        if(a.get(i) > b.get(i))
                        {
                        result[0] += 1;
                        } 
                        else if(a.get(i) < b.get(i))
                        {
                        result[1] += 1;
                }
        }
        return Arrays.asList(result);
        }  
    
- [Plus Minus](https://www.hackerrank.com/challenges/plus-minus/problem?h_r=profile)

        public static void plusMinus(List<Integer> arr) 
        {

                double zero = 0;
                double minus = 0;
                double plus = 0;

                for(int i=0; i < arr.size(); i++)
                {
                    if(arr.get(i) > 0)
                    {
                    plus += 1;
                    } 
                    else if(arr.get(i) < 0)
                    {
                    minus += 1;
                    }
                    else {
                    zero += 1; 
                    }
                }            
                System.out.println(plus/arr.size() + "\n" + minus/arr.size() + "\n" + zero/arr.size());
        }
    
    
- [Diagonal Difference](https://www.hackerrank.com/challenges/diagonal-difference/problem?h_r=profile)

        public static int diagonalDifference(List<List<Integer>> arr) 
        {
                int sum1 = 0;
                int sum2 = 0;
                int size = arr.size();
                for(int i = 0; i< size; i++)
                {
                    sum1 += arr.get(i).get(i);
                    sum2 += arr.get(i).get(size - ( i + 1 ));              
                }
                return Math.abs(sum1-sum2);
        }
    
- [Staircase](https://www.hackerrank.com/challenges/staircase/problem?h_r=profile)

        public static void staircase(int n) 
            {       
                for(int i = 1; i <= n; i++)
                {
                 int interspace = n - i;
                 for(int j = 0; j < interspace; j++)
                 {
                     System.out.print(" ");
                 }
                 int hashtag = n-interspace;
                 for(int k = 0; k < hashtag; k++)
                 {
                     System.out.print("#");
                 } 
                 System.out.println();
                }   
            }
    
 - []()   or
 
        public static void staircase(int n) 
             {      
               StringBuilder sb = new StringBuilder();
               StringBuilder sb2 = new StringBuilder();

               for(int i = 0; i < n; i++) {
                   sb.append(" ");
               }
               for(int j = n-1; j >= 0; j--) {
                  sb = sb.replace(j, j+1, "#");
                  sb2.append(sb.toString());
                  sb2.append("\n");
               }
               System.out.println(sb2.toString());
            }
    
 - []()      

