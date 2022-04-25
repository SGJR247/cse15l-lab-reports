# Lab Report 2 - Week 4
## By Samuel Genous Jr.

*Lab 3 Code Changes to Fix Bugs*

**1. Newline Fix (Samuel Genous Jr.)**
  
![Genous Newline Fix](https://user-images.githubusercontent.com/103216157/165007517-82323667-caa3-49f7-a428-36ef263c0527.png)

  * [Link to Test File with Failure-Inducing Input](https://github.com/SGJR247/markdown-parser/blob/main/test-file2.md?plain=1)
  * Symptom of Failure-Inducing Input
  
![Newline OutOfMemoryError](https://user-images.githubusercontent.com/103216157/165008574-9816ae1d-b821-4739-a768-7ade18941d11.png)

  * The failure-inducing input in the test file has blank newlines in between the given links, and at the end of the file. Intially, there were no actions the MarkdownParse.java file would be able to take, with the original version of the code it had. Thus, it was unable to recognize the newlines and ended up leading to an OutofMemoryError in the command line terminal.

**2. Using Image Link in Markdown (Edwin Ambrosia)**

![Ambrosia Image Fix](https://user-images.githubusercontent.com/103216157/165009374-74b9c3ba-cc3f-4644-986f-9df4a7039eed.png)

  * [Link to Test File with Failure-Inducing Input](https://github.com/eambrosio27/markdown-parser/commit/03aca9bffbf24720050087e71f6bf7b4e0b524c6)
  * Symptom of Failure-Inducing Input

![Image OutOfMemoryError](https://user-images.githubusercontent.com/103216157/165009703-47616c0f-49fc-4e56-83d1-5a3cf8ad4a82.png)

  * This test file includes a line that contains an image link. However, MarkdownParse.java wasn't originally equipped to handle lines that contained images. So, the program did not know what to do about the "!" in front of the "[" for the image line.

**3. Empty Link List (Shaodong Shan)**

![Shan Empty List Fix](https://user-images.githubusercontent.com/103216157/165012036-fd0305a4-6846-4c9a-9022-b066ca82c34a.png)

  * [Link to Test File with Failure-Inducing Input](https://github.com/TooMuchFish/markdown-parser/blob/main/test3.md)
  * Symptom of Failure-Inducing Input

![Empty Link List](https://user-images.githubusercontent.com/103216157/165012100-954a0b29-83d6-4db0-860d-8b01e2229a58.png)

  * This test file has a link that has a large space gap between the "]" and "(" characters, resulting in failure-inducing input. Because of this, MarkdownParse.java does not recognize this line as a link and does not take the link address. This results in an empty list being printed out in the command line terminal. 
