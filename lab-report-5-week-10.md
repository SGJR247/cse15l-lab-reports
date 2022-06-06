# Lab Report 5 - Week 10
## By Samuel Genous Jr.

*Lab 9 Test Comparisons*

**1. Process of Comparing Tests**

I used `vimdiff my-markdown-parser/results.txt cse15lsp22-markdown-parser/results.txt` in the command line terminal, in order to find the tests with different results, and read through the lines between both implementations' results.txt files in order to find their differences.

___

**2. Test File with Different Results**

[Link to Test File From Provided Repository (22.md)](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/22.md)

___

**3. Output of Tests Between Implementations**
  * Which is Correct?
      
      My implementation of MarkdownParse resulted in the correct output for 22.md, whereas the implementation from the provided repository was wrong.
  * Actual/Expected Outputs
 
      ![Results of Vimdiff MarkdownParse](https://user-images.githubusercontent.com/103216157/172106474-8f1f8ad8-c44c-49f0-ae9f-d02ea2e5b5bf.png)

      Actual Output in Vimdiff

      ![Expected CommonMark Output](https://user-images.githubusercontent.com/103216157/172107725-37439e8c-5543-415a-b122-400e7cc59066.png)

      Expected Output in CommonMark demo site

  *  Description of Bug

      I believe the code in the provided repository has a bug that keeps it from recognizing certain special characters (/, \, etc.) inside of the parentheses for the link. This could possibly be due to how the getCloseParen method reacts to said characters when being called, and thereby ignoring the entire link as a whole. Therefore, this prevented the output of this implementation of MarkdownParse from putting in the link for `foo` into the array.
      
      ![MarkdownParse Code: Location of Bug in Provided Repository](https://user-images.githubusercontent.com/103216157/172109675-eb409d2b-e9eb-43fd-8f75-a7968107051b.png)
