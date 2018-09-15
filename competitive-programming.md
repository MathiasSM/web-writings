---
title: Competitive Programming
date: 2015-01
description: Solving programming problems within a strict timeframe and specifications of memory or running time limits
path: /blog/competitive-programming
TOC: true
---

After a great math professor convinced me and two other students, we started (re)learning to code sooner and with one goal in mind: To compete in the "Coding Marathons" (how they're commonly called in my university). 

## The ACM-ICPC

The Association for Computing Machinery - International Collegiate Programming Contest (ACM-ICPC) is an annual competition for college students around the world, to compete against 40,000 other students in local and regional rounds for the opportunity to participate in the World Finals.

The rules are simple enough:

+ Group
  + Made by 3 students of the same university.

+ Materials
  + Each group is given a single computer.
  + Each group can bring (with some limits) books or other non-electronic material.
  + Paper and pencils are provided.

+ Competition
  + Each competition (or round) lasts 5 hours.
  + Each consists of solving 8 to 13 programming problems.
  + At any given moment, except for the final (dead) hour, a team is able to watch the scoreboard of solved problems by other teams.


## Other competitions 

The ICPC is but one of many worldwide competitions to prove your coding and logical thinking skills. Big companies like Google or Facebook like the idea enough to host their own competitions (CodeJam and HackerCup, respectively). The format is a little different from competition to competition, but topics are generally the same (lots and lots of topics).

If you're a minor, high-school student, you can compete en the International Olympiad in Informatics (IOI), which is, along with the ICPC, one of the oldest programming competitions, besides being one of the big five international science olympiads.

There are also many other institutions that organize coding competitions (even as its main activity), online or on-site. Some of them are the "Competitive Programming Network" (or RPC, "Red de Programación Competitiva" in Spanish), Codeforces (from Russia), CodeChef (from India), Topcoder (from the USA), HackerRank (from the USA); almost every competition is in English as a Standard to avoid ambiguity due to translation.

## What you can learn training

There are tons of things you can learn; and you must learn them if you want to reach for glory (red status in Codeforces, for example). Among those topics are a great deal of magical data structures, graph theory, geometry, string analysis, dynamic programming, number theory, and so much more.

Dealing with such quantity of information it's normal to get intimidated. And indeed, this might not be everyone's cup of tea, but it's impossible to know without trying. I can just say it can get pretty fun.

### How to start training

I started training soon in my studies, at the same time that my then team Augusto and Rubmary, with help from Prof. Ricardo. He guided us through the beginning of our journey, with puzzles and basic programming tasks that required just a bit more thinking than the last one. I love puzzles and find it a great way to train logical thinking.

We picked up C++ as it's the most used language in ICPC competitions, and found in it a powerful tool, too big to handle whole at first, but flexible enough to provide a simple learning environment. One thing I learned on the way, though, is that the language doesn't matter than much: The main goal of these competitions is to think of a solution. The basics are enough to start, and in the way more and more details of the language will show themselves.

The easiest way to train is to use an online judge of solutions. The judges usually have big catalogs of problems, which you can choose from, pick one, code a solution, and the judge will test it against several (usually hidden to the user) test cases to prove your solution correct, or give you some feedback as to why it's not (too much time running, too much memory used, crashed along the way, didn't even compile, ...). 

A common judge is SPOJ, and here are some easy problems for beginners: TEST, ADDREV, HELLOKIT, OFFSIDE, CANDY, NSTEPS, DRAWM, CYLINDER. Some not-so-for-beginners problems: FARIDA, SAMER08F, STPAR, CHOCOLA, HISTOGRA, PIGBANK, AGGRCOW. Do not look for answers before you try it yourself.

### Basic topics to learn along

Theory and implementations to be learning right after you start are:

+ Asymptotic Notation
+ Data Structures
  + Arrays
  + Linked lists
  + Stacks and Queues
  + Graphs
    + Adjacency matrix
    + Adjacency list
    + Arc list
+ Algorithms
  + Sorting (Bubblesort, Mergesort, Quicksort)
  + Binary Search
  + On graphs
    + Traversal (DFS, BFS)
    + Backtracking

There are many other topics. You're free to search around for them or contact me if you need help with anything.

### Best practices

+ Practice writing code on paper, even pseudo code. 
+ Practice reading other people code (important: read your teammates' code a lot, understand their thought process). 
+ Practice in online contests like Codeforces, and measure yourself with others. 
+ Don't look for other people's solutions, unless you're certain you can't solve it yourself; but, even then, implement the solution yourself so that you get experience on problems similar to that. 
+ Always solve off-contest any problem you couldn't solve on time. 
+ Read posts online explaining topics, or the books itself. 
+ Don't get stuck on a single problem, move on to another (that goes for in-contest and off-contest alike).
+ Read the editorials for the contests after the fact (sometimes written by competitors in ugly but potentially interesting blogs).
+ Don't lose the habit.
+ Keep a template for online contests, practice writing it quickly for on-sites, keep it short.

~~~cpp
#include <bits/stdc++.h>

#define FOR(i, from, to) for (int i = (from) ; i < to ; i++)
#define ms(obj, val) memset(obj, val, sizeof(obj))
#define ri(i) scanf("%d",&i)
#define mp make_pair
#define pb push_back

#define INF 0x3f3f3f3f
#define EPS 1e-10
#define PI acos(-1)

using namespace std;

typedef long long ll;
typedef pair<int, int> ii;
typedef vector<int> vi;

int gcd(int a, int b){ return b ? gcd(b, a % b) : a; }
int mcm(int a, int b){ return a * b / gcd(a, b); }
int pot(int a, int b){ return b ? (pot(a, b >> 1))*(pot(a, b >> 1))*(b & 1 ? a : 1) : 1; }

int main(){

}
~~~

