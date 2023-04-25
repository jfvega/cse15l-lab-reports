# Lab 2
## Part 1: StringServer
- **Here is my code:** ![Image](Screenshot 2023-04-24 at 6.48.48 PM.png)
- **Here are my two screenshots of my code working:**
- **Step 1** `/add-message?s=Jesse`: ![Image](Screenshot 2023-04-24 at 6.57.34 PM.png)
- For step 1 the /add is called. Then the it creates array by splitting the string where the = sign is. The query which is the s which stands for string, and the <message> you input whch in this case is Hello. So parameter 0 equals s, and the Hello message is added to the previous string. Which creates the whole brand new string. Then we return the line and Jesse is printed on the page.
- **Step 2:** `/add-message?s=Vega`: ![Image](Screenshot 2023-04-24 at 7.01.36 PM.png)
- In step 2 the similar things happen to it as in step 1. But insted of just creating a string, this time it is added to the string. Which is why we now see Jesse Vega. And we have to notice the "\n". That is important because that is what starts the new line. Also not that whatever is inputted into the <message> area, it will be then turned to a string. If we input an 878 it will turn it into a string. 

  
## Part 2: Bugs
- **Doesn't induce failure:** `public void testReverseINPlace() {
    int[] input1 = { 15 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 15 }, input1);
	}`
- **Induces Failure :** `public void testReverseInPlace2() {
    int[] input1 = { 1,2,3,4,5 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{5,4,3,2,1}, input1);
	}`
  
- **Output:** ![Image](Screenshot 2023-04-24 at 7.41.58 PM.png)
- **Before:**  `static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }`
- **After:**  `static void reverseInPlace(int[] arr) {
    for(int i = 0; i < (arr.length/2); i += 1) {
    int temp = arr[i];//need to set it to varible
      arr[i] = arr[arr.length - i - 1];// make sure the middle elemnt stays//same as other note
      arr[arr.length-i-1]= temp;
    }
  }`
- **Why it works now: It works now because in the for loop we had to divide the array by two since we want the middle to tsay the same. Then I needed to set it as a variable so i made the new variable temp. In the lat line  I made sure the element stayed in the middle and made the variable equal to temp.**

	
## Part 3: What I learned
- **During week 3, I found the URL very interesting. Before I had no idea what was in a url. I thought there was no patterns to them, and that it was all just random stuff made for each websites. But after learning, the domain, the paths, and the query it makes a lot more sense. Now when I look at the url, I can see what is happening and I notice it. It was also cool to see how to set up our own url. I had no idea we could do that with code, I just thought you always had to use a website like weebly or wix. I think it's my new favorite thing to make servers, and run stuff.**
