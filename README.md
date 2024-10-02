# Preparation Tips:

- Brush up on all common algorithms and data structures.

    - Sorting: Learn Merge Sort as it is also a common solution for problems like Count of smaller numbers after self.
    - Binary Tree: Implement a class with insert, delete, find, and various traversals (inorder, postorder, preorder, left view, right view, top view, bottom view, BFS).
    - Binary Search Tree: Insert, delete, find, convert between tree and list.
    - Union Find: Implement union, and find.
    - Segment Tree: Implement get range answer, and update.
    - Trie: Implement insert and read.
    - Heap: Implement heapify, add, and remove.
    - Matrix: Solve shortest path problems like 01-matrix, rotten oranges, flood fill, rat in a maze etc.
    - Graph: Solve shortest path problems using Dijkstra.

- Once you are clear with the basics, I recommend this cheatsheet [URL1]. It's not mine, but I'm thankful I randomly found it in a LinkedIn post. It covers a wide variety of questions and specific topic tabs. Practice a few questions on important topics like Tree, BST, Graph, Shortest Path, Trie, BFS, Disjoint Set, Matrix, etc.

- **Important**: Remove topic tags from questions and shuffle them to practice identifying the appropriate data structure during an interview.

- **Important**: I always used DFS to detect cycles in directed graphs and failed many interviews because of it. A turning point came when I accidentally learned about Kahn's algorithm while looking at the solution for Course Schedule II [URL2].
Since then, I've solved every graph, tree, and matrix problem using BFS, and it has been the most efficient approach. While some problems may require DFS, those are rarely asked in interviews. Focus on mastering BFS; it will elevate your problem-solving skills to the next level. Trust me, you will rarely need to use DFS in interviews!

- **Important**: Only practice medium and hard questions. Forget about easy ones. Even if medium questions feel challenging, you will only improve by attempting them. Easy questions are never asked in interviews.

- Google interview questions are unique and can't be found elsewhere. There is a fixed pool of confidential questions created each year from which the interview panel selects, including follow-up questions.

- If you've completed all your preparations and need more questions to practice, I strongly suggest visiting [URL3]. In the problems section, filter for hard and medium problems with the company tag "Google." The problems there are unique, challenging, and can also be found on LeetCode.

- YouTube channels like @techdose4u, @NeetCode, and @TheAdityaVerma were particularly helpful to me during practice.

## Systems Design:

- First, understand the intuition behind the CAP theorem. You should grasp the meanings of consistency and availability. For example, I always imagine a bank with one ATM. If you prioritize consistency, the ATM will only be available when the bank's server is online, ensuring that the balance is always correct. Conversely, if you prioritize availability, the ATM will process withdrawals even if the server is down, allowing money to be withdrawn without verifying the balance. This is why banking systems are designed to prioritize consistency.

- Start with learning about unique ID generators. Although this has become a cliché and isn't asked as often, it's still valuable to understand every variation, including the Twitter Snowflake technique, to see how system design concepts evolve.

- Next, learn how to implement a distributed key-value database for both consistent and available use cases.

- Study how to implement distributed locking.

- **Important**: While common problems like Ola, YouTube, and TinyURL are frequently discussed online, interviews present new challenges. For example, designing a Top-K leaderboard. Recommended resources:
    - System Design Interview – An Insider's Guide by Alex Xu Volume 1: Good for understanding basic concepts and classic problems.
    - System Design Interview – An Insider's Guide by Alex Xu Volume 2: Covers a new set of less common problems.
    - YouTube Channel @jordanhasnolife5163 : Offers videos on unique and less common system design problems. The explanations may be fast, but they are useful for understanding diverse scenarios.
    - It's useful to understand key MSA patterns like API Gateway, BFF, Circuit Breaker, Database per Service, Event-Driven Architecture, and Saga. Focus on the Saga pattern (using a queue) to handle rollbacks and avoiding race conditions in multi-service transactions like order placement, ensuring consistency and atomicity—either all changes go through or none.
    - YouTube Channel @interviewpen: It covers many questions that SDEs often wonder about but rarely have time to research, such as OAuth and SQL query optimization. While these topics might not provide immediate help for an upcoming interview, they will certainly benefit you in the long run.

- **Important**: Don't overlook Low-Level Design (LLD). Although High-Level Design (HLD) questions are popular, LLD is just as important for interviews. You can find relevant questions on LeetCode, such as external merge sort, elevator algorithms, parking lots, or Twitter feeds.

- **Important**: Einstein said, "If you can't explain it simply, you don't understand it well enough." In HLD, we often add unnecessary components for minor objectives. For example, a queue, CDN or Elasticsearch might not be needed, but we tend to include them to impress the interviewer. However, seasoned system architects see this as over-complicating the system, which increases operational costs.

- **Important**: Avoid overcommitting. Don't add features or requirements that weren't explicitly asked for by the interviewer, as it can make your design overly complex and difficult to implement.

Good luck with your preparations!


URL1-https://docs.google.com/spreadsheets/d/1o3Amyyt4qSmy_Yx4Dv7-UCn_DYLPiufUMUzvsWCSBg0/edit?usp=sharing
URL2-https://leetcode.ca/2016-06-27-210-Course-Schedule-II/
URL3-https://www.lintcode.com/
