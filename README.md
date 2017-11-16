# RoboContest

RoboContest

Description

Computer Engineering Department of Sharif University of Technology is holding a nationwide robotic contest. Each attending team brings a fixed number of identical small robots specifically designed for the contest. The contest table is large enough and a map has been drawn on it. The map contains many regions each painted in a color different from the colors of its neighboring regions. The robots can detect the colors on the map.


The contest is held once for each team and the winning teams will advance to the second round. For each team, the contest referees consisting of representatives of each participating university will select k regions of the map and the team will put one robot in each of the selected regions. Each robot can turn in any direction and move from one region to any of the neighboring regions. The contest clock starts from zero and ticks with a loud sound at the beginning of each 10 seconds. The principal rule of the contest is that at each clock tick, each robot should move from its current region to one of its neighboring regions so that it is there at the next clock tick. The regions are small enough that this is always possible. Two or more robots can be in one region at the same time.


The goal of the contest is that the robots of the playing team should move according to the given rule, so that in one of the future ticks all robots meet in one region. The playing team wins if it succeeds in doing so or the robot driver program detects the impossibility of achieving this goal, in which case the robots are ordered not to move on the first tick. A Playing team does not know anything about the map before the contest and receives the actual map data and initial positions just a few minutes before they start, long enough to enter the data to the robots memories. So, the program driving the robot should work for any possible map and initial positions.

You are the top programmer of your university team in this contest. You should write one program to drive all the robots of your team. It should receive the map data and the initial positions of all robots and outputs the (possibly empty) set of moves that each robot should follow, such that all robots meet in one region in one of the future clock ticks. In this ACM programming contest you are to solve a rather simpler problem. You just have to find out whether such synchronous moves of robots are possible.

Input

The first line of the input file contains a single integer t (1 <= t <= 10), the number of test cases, followed by the input data for each test case. The first line of each test data contains two integers n (1 <= n <= 100) and k (1 <= k <= 100) which are the number of regions and the number of robots, respectively. Following the first line, there are n lines each describing one region in the following way: an arbitrary non-negative integer, which is the unique identification number of the region, the number of neighbors of that region (m), followed by a sequence of m numbers corresponding to identification numbers of the neighboring regions. The last line of the test case contains k integers which are the id numbers of the initial regions of robots.

Output

There should be one line per test case containing a single word YES or NO depending on whether or not a successful sequence of synchronous moves of robots is possible.

Sample Input

1
4 2
1 3 2 3 4
2 3 1 3 4
3 3 1 2 4
4 3 1 2 3
1 2

Sample Output

YES
