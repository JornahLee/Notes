

# 树：

二叉树

2-3树：属于B树

B树：一个m阶树，每个节点至少有两个子节点，至多有m-1个节点（所有节点保存索引和数据）

B+树：与B树不同点在于，只有叶子节点才保存数据，非叶子节点只保存索引

B*树

红黑树

# 二叉树

## 基本概念
叶子：
根
度：
深度：
分类：



## 分类：

满二叉树

二叉搜索树（二叉排序树，排序二叉树）

平衡二叉树（左右子树的深度差<=1）








## 创建二叉树：

\1.       先（后）序数组，中序数组 生成二叉树

\2.       有序数组构建平衡二叉树（二叉搜索树）

## 遍历二叉树：

思想：深度优先搜索dfs

 

 

思想：广度优先搜索bfs

 

## 二叉树的最大深度

pubilc static int maxDepth(TreeNode root){

​                   if(root==null) return 0;

​                   int dep1=0,dep2=0;

​                   if(root.left!=null) dep1=maxDepth(root.left);

​                   if(root.right!=null) dep2=maxDepth(root.right);

​                   return dep1>dep2?dep1+1:dep2+1;

​         }

## 二叉树的最小深度

