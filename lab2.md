# Lab 2
## Part 1: StringServer
- Here is my code: ![Image](Screenshot 2023-04-24 at 6.48.48 PM.png)
- Here are my two screenshots of my code working:
- Step 1 `/add-message?s=Jesse`: ![Image](Screenshot 2023-04-24 at 6.57.34 PM.png)
- For step 1 the /add is called. Then the it creates array by splitting the string where the = sign is. The query which is the s which stands for string, and the <message> you input whch in this case is Hello. So parameter 0 equals s, and the Hello message is added to the previous string. Which creates the whole brand new string. Then we return the line and Jesse is printed on the page.
- Step 2 `/add-message?s=Vega`: ![Image](Screenshot 2023-04-24 at 7.01.36 PM.png)
- In step 2 the similar things happen to it as in step 1. But insted of just creating a string, this time it is added to the string. Which is why we now see Jesse Vega. And we have to notice the "\n". That is important because that is what starts the new line. Also not that whatever is inputted into the <message> area, it will be then turned to a string. If we input an 878 it will turn it into a string. 

  
## Part 2: Bugs
- Doesn't induce failure: `public void testReverseINPlace() {
    int[] input1 = { 15 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 15 }, input1);
	}`
- Induces Failure : `public void testReverseInPlace2() {
    int[] input1 = { 1,2,3,4,5 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{5,4,3,2,1}, input1);
	}`
  
- Output: ![Image](
-Before: ![Image](
-After: ![Image](
