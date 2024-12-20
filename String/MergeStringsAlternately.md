
https://leetcode.com/problems/merge-strings-alternately/description/?envType=study-plan-v2&envId=leetcode-75

```java
class Solution {
    public String mergeAlternately(String word1, String word2) {
        int word1Size = word1.length();
        int word2Size = word2.length();

        StringBuilder sb = new StringBuilder();

        int i = 0;
        int j = 0;

        while(i < word1Size || j < word2Size ) {
            if(i < word1Size) {
                sb.append(word1.charAt(i++));
            }

            if(j < word2Size) {
                sb.append(word2.charAt(j++));
            }
        }

        return sb.toString();
    }
}

```
