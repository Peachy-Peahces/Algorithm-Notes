# Priority Queue
**Abstract:**

---
# 前言：
---
# 优先队列

其本质上还是通过二叉堆来实现，首先介绍二叉堆的概念：
二叉堆是一种特殊的“完全二叉树”，它在内存中通常用数组来存储。它必须同时满足以下两个条件：
  结构特性： 它必须是一棵完全二叉树 (Complete Binary Tree)。
  堆序特性： 树中所有的父节点，都必须满足一个特定的“堆序” (Heap Order)。这个顺序分为两种：
    大根堆 (Max Heap)： 任何一个父节点的值，都大于或等于它的任意一个子节点的值。
    小根堆 (Min Heap)： 任何一个父节点的值，都小于或等于它的任意一个子节点的值。
    <img width="1004" height="427" alt="image" src="https://github.com/user-attachments/assets/b84132df-72b6-4afc-82c9-aa7a804eefd3" />

### 大根堆的上浮调整
如下图所示：
<img width="1158" height="610" alt="image" src="https://github.com/user-attachments/assets/409853de-b302-44d6-b0e6-51796b2a23c1" />
先加到队尾，随后进行上浮，与父节点进行比较
边界条件：i比较到根节点即可，再进行元素交换

### 大根堆的下沉调整
pop堆顶元素后，需要把
边界条件：比较到最后一个非叶子节点，后续都是叶子节点，没有子节点，不需要再考虑和孩子比较
<img width="1169" height="523" alt="image" src="https://github.com/user-attachments/assets/e1aea888-9b54-4ac2-8564-ed226cc60d55" />


