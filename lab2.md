# Lab 2
## Part 1: StringServer
- **Here is my code:** ![Image](Screenshot 2023-04-24 at 6.48.48 PM.png)
- **Here are my two screenshots of my code working:**
- **Screenshot 1:** `/add-message?s=Jesse`: ![Image](Screenshot 2023-04-24 at 6.57.34 PM.png)
- For step 1 the /add is called. Then the it creates array by splitting the string where the = sign is. The query which is the s which stands for string, and the <message> you input whch in this case is Hello. So parameter 0 equals s, and the Hello message is added to the previous string. Which creates the whole brand new string. Then we return the line and Jesse is printed on the page.
- **Screenshot 2:** `http://localhost:2323/add-message?s=Vega`: ![Image](Screenshot 2023-04-24 at 7.01.36 PM.png)
What is happening:
- The line variable is an Jesse as of now, since in our first step we set line equal to Jesse. 
- The first method called is the handlerequest. `public String handleRequest(URI url) {`: The URI in this example is the url, the url variable is then equal to http://localhost:2323/add-message?s=Vega.
- Now in this example, /add is found in the our url so that brings us to the else stament. 
- 'String[] parameters = url.getQuery().split("=");` : This line then sets parameter equal ["s","Vega"] as it splits the query into two strings. Strings because of the type before the parameter variable. 
- `String line2 = String.format(parameters[1]);`: line2 will equal the index 1 of parameter which is "Vega". So the variable line2 is now eqaul to "Vega" in this case. 
- `line += line2 + "\n";` line will then add/equal line 2. It is importan to notice the `/n` becaus ethat starts the new line.
- `return String.format(line);` This will finally return what we see inthe code above. Line will equal that until you repeat, which will then change it.


  
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
- **Why it works now: It works now because in the for loop we had to divide the array by two since we want the middle to stay the same. Then I needed to set it as a variable so I made the new variable temp. In the lat line  I made sure the element stayed in the middle and made the variable equal to temp.**

	
## Part 3: What I learned
- **During week 3, I found the URL very interesting. Before I had no idea what was in a url. I thought there was no patterns to them, and that it was all just random stuff made for each websites. But after learning, the domain, the paths, and the query it makes a lot more sense. Now when I look at the url, I can see what is happening and I notice it. It was also cool to see how to set up our own url. I had no idea we could do that with code, I just thought you always had to use a website like weebly or wix. I think it's my new favorite thing to make servers, and run stuff.**
