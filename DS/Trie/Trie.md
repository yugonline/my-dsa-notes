## 
### Topic: Trie
--- 
### **Questions/Keywords (Left Column)**  
*Use this section for questions, keywords, or main ideas.*


--- 


#### **Notes (Right Column)***Detailed notes, explanations, or information go here.* 
- A trie is not always the best solution for example
	- In case if you have a string S and you want to find from a list of W words how many of them are prefixes to the string S 
	- Then creating a Trie is actually an overhead because it will take O(M) to create/precompute the Trie
	- Then it will take O(W*L) time to traverse the Trie for W words of average length L each. 
- Conversely if you have M strings to search IN and W words to find if they are prefixes or not of those M strings then Trie becomes useful
	- Now you have W words so searching will still be O(W*L) instead of generic prefix search which will be `O(W*L*M*P)` where W words have average length L and M strings have average length P
	- But there will be slightly more precompute with O(M*P) time taken to generate the Trie
	- So we go from multiplication to addition which is a huge speedup
- Here is a complete solution of Trie in Python
	- 

----

### Summary  *Write a brief summary of the key points covered in this section.*