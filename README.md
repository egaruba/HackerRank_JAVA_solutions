## HackerRank_JAVA_solutions
Real world Java solutions based on HackerRank challenges



A Very Big Sum (Difficulty 2.0):

Scenario: Summing Up Financial Transactions
Use Case: In a banking application, where financial transactions involve large amounts, the A Very Big Sum code can be used to accurately calculate the total transaction amount.
Birthday Cake Candles (Difficulty 2.5):

Scenario: Celebrating Birthdays
Use Case: For a birthday party planning application, you might need to find out how many candles are on a birthday cake. The Birthday Cake Candles code helps count the number of candles with the highest height.
Grading Students (Difficulty 3.0):

Scenario: Student Grade Calculation
Use Case: In an educational system, the Grading Students code could be used to determine the final grades of students based on their performance and a grading scale. It involves applying simple rules to round up grades.
Plus Minus (Difficulty 3.5):

Scenario: Weather Analysis
Use Case: Imagine a weather application analyzing temperature data. The Plus Minus code could be used to calculate the percentage of positive, negative, and zero temperature readings over a period.
Staircase (Difficulty 4.0):

Scenario: Architectural Design
Use Case: In architectural design software, the Staircase code can be employed to create visual representations of staircases, where nested loops help in generating the step patterns.
Time Conversion (Difficulty 4.0):

Scenario: Scheduling Events
Use Case: In an event management system, the Time Conversion code can be used to convert different time formats. For instance, converting from 12-hour to 24-hour format for scheduling purposes.
Compare the Triplets (Difficulty 4.5):

Scenario: Team Performance Evaluation
Use Case: In a sports analytics application, the Compare the Triplets code might be utilized to compare the performance of two teams in various aspects like offense, defense, and strategy.
Mini-Max Sum (Difficulty 4.5):

Scenario: Financial Planning
Use Case: For financial planners, the Mini-Max Sum code could be applied to analyze investment portfolios. It helps in identifying the minimum and maximum possible sums by excluding one investment at a time.
Diagonal Difference (Difficulty 5.0):

Scenario: Image Processing
Use Case: In image processing applications, the Diagonal Difference code might be used to calculate the difference between pixel values along diagonals, assisting in identifying contrasts.
Number Line Jumps (Difficulty 6.0):

Scenario: GPS Navigation
Use Case: In a GPS navigation system, the Number Line Jumps code could represent the movement of two objects (like vehicles) along a number line. The algorithm checks if they will meet after a certain number of jumps.
Cats and a Mouse (Difficulty 6.5):

Scenario: Wildlife Tracking
Use Case: For wildlife researchers, the Cats and a Mouse code can be analogous to tracking movements of two predators (cats) and a prey (mouse) in a defined area.
Searching an Element in Array Binary Search (Difficulty 7.0):

Scenario: Database Query Optimization
Use Case: In a database system, the Searching an Element in Array Binary Search code might be applied to optimize the search for a specific record in a large dataset.
Breaking the Records (Difficulty 7.5):

Scenario: Sports Records Analysis
Use Case: For sports analysts, the Breaking the Records code could be used to analyze athletes' performances, identifying when they break or set new records.





1. [Calculating Total Sales](#CalculateTotalSales)
2. [A Very Big Sum](#AVeryBigSum)
3. [Compare the Triplets](#CompareTheTriplets)
4. [Plus Minus](#PlusMinus)
5. [Diagonal Difference](#DiagonalDifference)
6. [Staircase](#Staircase)
7. [Mini-Max Sum](#Mini-Max-Sum)
8. [Birthday Cake Candles](#BirthdayCakeCandles)
9. [Time Conversion](#TimeConversion)
10. [Grading Students](#GradingStudents)
11. [Cats and a Mouse](#CatsMouse)
12. [Number Line Jumps](#NumberLineJumps)
13. [Breaking the Records](#BreakingTheRecords)
14. [](#)

<a name=""></a>
1. <a name="CalculateTotalSales"></a>[Calculating Total Sales](#) - Suppose you are developing a point-of-sale system and you need to calculate the total sales for a day based on sales figures stored in an array, how would you approach implementing the necessary code for this task? Provide a Java code snippet demonstrating how you would calculate the total sales by summing up the sales figures in the array.
        
   public class PointOfSaleSystem {

   public static int calculateTotalSales(int[] salesFigures) {
        int totalSales = 0;

        for (int sales : salesFigures) {
            totalSales += sales;
        }

        return totalSales;
    }

    public static void main(String[] args) {
        int[] dailySales = {150, 230, 180, 210, 190};

        int totalSalesForDay = calculateTotalSales(dailySales);

        System.out.println("Total Sales for the Day: $" + totalSalesForDay);
    }
}

- Explanation:
The calculateTotalSales function is designed to take an array of sales figures as input and iterate through the array, summing up the sales figures. The main method provides an example array dailySales, and the result is displayed, demonstrating the approach to calculate total sales for a day in the context of a point-of-sale system.
        
2. <a name="AVeryBigSum"></a>[A Very Big Sum](https://www.hackerrank.com/challenges/a-very-big-sum/problem?h_r=profile) 

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

3. <a name="CompareTheTriplets"></a>[Compare the Triplets](https://www.hackerrank.com/challenges/compare-the-triplets/problem?h_r=profile) - comparison points by comparing a[0] with b[0], a[1] with b[1], and a[2] with b[2].

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
    
4. <a name="PlusMinus"></a>[Plus Minus](https://www.hackerrank.com/challenges/plus-minus/problem?h_r=profile)

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
    
    
5. <a name="DiagonalDifference"></a>[Diagonal Difference](https://www.hackerrank.com/challenges/diagonal-difference/problem?h_r=profile)

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
    
6. <a name="Staircase"></a>[Staircase](https://www.hackerrank.com/challenges/staircase/problem?h_r=profile)

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
    
7. <a name="Mini-Max-Sum"></a>[Mini-Max Sum](https://www.hackerrank.com/challenges/mini-max-sum/problem?h_r=profile)      
 
         public static void miniMaxSum(List<Integer> arr) {            
            long minValue = 0;
            long maxValue = 0;
            Collections.sort(arr); 
            int size = arr.size();  
            for(int i = 0; i < size-1; i++)
            {
                minValue += arr.get(i);
            }
            for(int j = 1; j < size; j++)
            {
                maxValue += arr.get(j);
            }
            System.out.println(minValue + " " + maxValue);
            }
    
8. <a name="BirthdayCakeCandles"></a>[Birthday Cake Candles](https://www.hackerrank.com/challenges/birthday-cake-candles/problem?h_r=profile)  

        public static int birthdayCakeCandles(List<Integer> candles) {
                int count = 0;
                int max = Collections.max(candles);

                for (int x : candles){
                    if  (x == max){
                        count += 1;
                    }
                }
                return count;   
            }

- []() or

        public static int birthdayCakeCandles(List<Integer> candles) {
                int count = 0;
                int max = 0;
                for(int x : candles)
                {
                    if(max < x)
                    {
                        max += 1;
                    }
                }
                for(int i = 0; i < candles.size(); i++)
                {            
                    if(candles.get(i) == max)
                    {
                        count += 1;
                    }
                }
                return count;  
            }
    
9. <a name="TimeConversion"></a>[Time Conversion](https://www.hackerrank.com/challenges/time-conversion/problem?h_r=profile)

        public static String timeConversion(String s) {

            String str = s.substring(8, 9); 
            s = s.substring(0, 8); 
            int hr = Integer.parseInt(s.substring(0, 2));

            if(str.equalsIgnoreCase("p") && (hr != 12))
            { 
                hr += 12; s = hr + s.substring(2); 
            }
            else if(str.equalsIgnoreCase("a") && (hr == 12))
            { 
                s = "00" + s.substring(2); 
            } 
            return s; 

        }
    
10. <a name="GradingStudents"></a>[Grading Students](https://www.hackerrank.com/challenges/grading/problem?h_r=profile)

        public static List<Integer> gradingStudents(List<Integer> grades) {
                for (int i = 0; i < grades.size(); i++ ) {
                    int item = grades.get(i);
                    if (item >= 38 && item%5 != 0) {
                        int targetNumber = ((item/5) +1) * 5;
                        int difference = targetNumber - item;
                        if ( difference < 3 )
                            grades.set(i, targetNumber); 
                    }
                }        
                return grades;
            }    
                                   


11. <a name="CatsMouse"></a>[Cats and a Mouse](https://www.hackerrank.com/challenges/cats-and-a-mouse/problem?h_r=profile)

        static String catAndMouse(int x, int y, int z) 
                {
                        int d1 = Math.abs(x-z);
                        int d2 = Math.abs(y-z);
                        if(d1>d2)
                        {
                            return "Cat B";
                        } 
                        else if(d1<d2)
                        {
                            return "Cat A";
                        }
                        return "Mouse C";
                }
    
    
12. <a name="NumberLineJumps"></a>[Number Line Jumps](https://www.hackerrank.com/challenges/kangaroo/problem?h_r=profile)

        public static String kangaroo(int x1, int v1, int x2, int v2) 
            {
                String output = "NO";
                for (int i = 0; i <= 10000; i++) {

                    x1 += v1; 
                    x2 += v2;

                    if (x1 == x2) {
                        output = "YES"; break;
                    }
                    else
                    {
                        output = "NO";
                    }
                }
                return output;    
            }
    
13. <a name="BreakingTheRecords"></a>[Breaking the Records](https://www.hackerrank.com/challenges/breaking-best-and-worst-records/problem?h_r=profile)    

                class Result {    

                    public static List<Integer> breakingRecords(List<Integer> scores) {            
                        int highestScoreCounter = 0;
                        int currenthighestScore = scores.get(0);
                        for (int i = 1; i < scores.size(); i++ ) {
                            if (scores.get(i) > currenthighestScore) {
                                highestScoreCounter++;  
                                currenthighestScore = scores.get(i);
                            } 
                        }                
                        int lowestScoreCounter = 0;
                        int currentLowestScore = scores.get(0);
                        for (int i = 1; i < scores.size(); i++ ) {
                            if (scores.get(i) < currentLowestScore) {
                                lowestScoreCounter++;  
                                currentLowestScore = scores.get(i);
                            } 
                        }
                        List<Integer> output = new ArrayList<Integer>();
                        output.add(highestScoreCounter);
                        output.add(lowestScoreCounter);
                        return output;
                    }
                }


- []()  
