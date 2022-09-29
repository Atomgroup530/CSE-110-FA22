# Xun Liu 柳逊
![profile](profiles/Profile.jpg)

> Start early, start often.

---
## **MENU**
---
  - [**BIO**](#bio)
  - [**SKILLS**](#skills)
  - [**Leetcode Example**](#leetcode-example)
  - [**CHECKLIST**](#checklist)
  - [EASTEREGG](profiles/Face-Reveal.jpg)
[private](PRIVATE.txt)
## **BIO**
---
Hi, I'm Xun Liu 柳逊, 3rd year Computer Engineering student from Tianjin, China. I choose this major because solving prolems with softwares is fun and useful. I'm currently looking for an intern position in software engineering.

When I'm not studying computer or looking for a job, I play and make music with guitar, keybaord, and bass. I'm also enthusiastic about skateboarding, especially freestyle skateboarding.

Let me know if we share the same hobby, interest, or career goals :)
## **SKILLS**
---
1. **Language & Tools**
   - Good command of ***Python, Java, C, C++ language***
   - Proficient use of ***Vim and VS Code*** operations
2. **Academic Commands**
   - Proficiency ***in circuit analysis*** and ***circuit assembling***
   - Good command of ***Calculus*** and ***complex number calculation***
   - Proficiency in using ***Zoom functions***, ***screen projection***, and other electronic teaching facilities
3. **Communication Abilities**
   - Proficiency in explaining class material in ***words and drawings***
   - Proficiency in ***communication*** and ***teamwork skills***

### Leetcode Example
---
[671. Second Minimum Node In a Binary Tree](https://leetcode.com/problems/second-minimum-node-in-a-binary-tree/)
```
/**
 * Definition for a binary tree node.
 * struct TreeNode {
 *     int val;
 *     TreeNode *left;
 *     TreeNode *right;
 *     TreeNode() : val(0), left(nullptr), right(nullptr) {}
 *     TreeNode(int x) : val(x), left(nullptr), right(nullptr) {}
 *     TreeNode(int x, TreeNode *left, TreeNode *right) : val(x), left(left), right(right) {}
 * };
 */
class Solution {
public:
    set<int> ss;
	
    void inorder(TreeNode* root){
        if(root== NULL) return;
        inorder(root->left);
        ss.insert(root->val);
        inorder(root->right);
    }
	
    int findSecondMinimumValue(TreeNode* root) {
        inorder(root);
        if(ss.size() < 2 )return -1;
        vector<int> v(ss.begin(),ss.end());
        return v[1];
    }
};
```

## **CHECKLIST**
---
- [x] Pictures
- [x] Headings
- [x] Styling text
- [x] Quoting text
- [x] Quoting code
- [x] External Links
- [x] Section links
- [x] Relative links (Link to another .md file or an image in your repo. If linking to an image, encode it as a regular link rather than an image.)
- [x] Ordered and Unordered Lists
- [x] Task lists