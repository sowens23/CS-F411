# CS-F411 Analysis of Algorithms
## Course Description

```
#include <iostream>
int main() {
  std::cout << "Hello traveler, here's a towel for protection. Take care of yourself out there." << std::endl;
  return 0;
}
```

## Class Repositories
  - [sowens23-GitHub](https://github.com/sowens23)
  - [GitHubPortal](https://github.com/sowens23/Newbie-Gains/blob/main/README.md)
  - [CS-F411 Class Canvas](https://canvas.alaska.edu/courses/31505/modules)

## References
  - Course Reading: [Intro to Algorithms](https://www.cs.mcgill.ca/~akroit/math/compsci/Cormen%20Introduction%20to%20Algorithms.pdf)

## Big Notes
  - 

## Class Assignments
| ## | Description | Repo | Deliverable 1 | Deliverable 1 |
| --- | --- | --- | --- | --- |

## Class Note Directory
|            Week-## | Description | Quick Link | Other Notes | HW-## | Lab-## |
| ------------------ | --- | --- | --- | --- | --- |
| [Week-01](#Week-01) | --- | --- | --- | --- | --- |
| [Week-02](#Week-02) | --- | --- | --- | --- | --- |
| [Week-03](#Week-03) | --- | --- | --- | --- | --- |
| [Week-04](#Week-04) | --- | --- | --- | --- | --- |
| [Week-05](#Week-05) | --- | --- | --- | --- | --- |
| [Week-06](#Week-06) | --- | --- | --- | --- | --- |
| [Week-07](#Week-07) | --- | --- | --- | --- | --- |
| [Week-08](#Week-08) | --- | --- | --- | --- | --- |
| [Week-09](#Week-09) | --- | --- | --- | --- | --- |
| [Week-10](#Week-10) | --- | --- | --- | --- | --- |
| [Week-11](#Week-11) | --- | --- | --- | --- | --- |
| [Week-12](#Week-12) | --- | --- | --- | --- | --- |
| [Week-13](#Week-13) | --- | --- | --- | --- | --- |
| [Week-14](#Week-14) | --- | --- | --- | --- | --- |
| [Week-15](#Week-15) | --- | --- | --- | --- | --- |

# Class Notes

## Week-01
[08-24-26 - 08-30-26](#TOP)
  - A faster computer can make a program faster. A faster algorithm can make the impossible possible!
  - Measuing the speed of an algorithm is a difficult task.
  - Wall-clock time measures even with the same algorithm, can be impacted by hardware, OS, language, compiler, hardware load, etc.
  - We're spending a lot of time reviewing big O notation and which components of a time complexity analysis are most important.
  - Scalability Timeline
    - 1 > logn > n > nlogn > n^2 > n^3 > 2^n > n!
  - Big O: Defines an upper bound of the speed complexity of an algorithm where g(n) is always larger than f(n)
  - Big Omega: Defines the asymptotic lower bound where g(n) is always smaller than f(n)
  - Big Theta: Defines both asymptotically tight bound (Upper and Lower)
    - So for example;
      - f(n) = 4n^2 + 7n + 12 = BigTheta(n^2) for some cn^2
      - Where:
        - Big O = (4+7+12)n^2 = 25n^2
        - Big Omega = 4n^2
        - Such that:
          4n^2 <= f(n) <= 25n^2 for (n >= 1)
          
  | *Notation* | Termin | Meaning | Mental Picture |
  | --- | --- | --- | --- |
  | f = O(n) | Big-O | No faster than g | Bounded above |
  | f = o(n) | Little-O | Strictly slower than g | Ratio -> 0 |
  | f = Ω(n) | Big Omega | No slower than g | Bounded Below |
  | f = ω(n) | Little Omega | Strictly faster than g | Ratio -> inf |
  | f = θ(n) | Theta | Same asymptotic rate | Ratio behaves like a constant |

## Week-02
[08/31/26 - 09/06/26](#TOP)  
  - If you take the limit ratio of two notations ex. 
    - n^2 vs n = (n^2)/n = Infinity   (little-w) (strictly faster)
    - n vs n^2 = n/(n^2) = Zero       (big o)
    - Set relationships
      1. o(g)
  - Choose your proof weapon

    | | **Direct** | **Contrapositive** | **Contradiction** | **Induction** |
    | --- | --- | --- | --- | --- |
    | **Assumption** | Start with P | Start with -Q | Assume the bad world | First domino |
    | **Method of Proof** | Walk to Q | Reach -P | Make it impossible | Then every next one |
    | Symbol | P => Q | -Q => -P |  

  ### Direct Proof
  - Claim: If *n* is even, then n^2 is even.
    - If n is even, then *n-2k*
    - Then n^2 = (2k)^2 = 4k^2 = 2(2k)^2
    - Since we know n is an integer, n^2 is even.
  - Claim: If a and b are odd, then a+b will be even
    - If a = 2n+1 and b = 2m+1
    - And a+b = 2n+1 + 2m+1 = 2(n+m+1)
    - Therefore a+b is even.

  ### Contrapositive Proof
  - Contrapositive *not P* therefore *not Q*
  - Claim: If *n* is even, then *n^2* is even
    - If n *is odd*, then *n^2 is odd*
    - Let n=2k+1, then (2k+1)^2 =4(k^2)+1
    - Therefore claim is true because if n^2 is odd, then n is odd.

  ### Contradiction Proof
  - Prove that *not Q* is impossible through reason, therefore Q must be true.
  - Logic: Assume that a lie is true, and pick it apart to prove that it's impossible to be true.
  - Claim: There is a largest integer.
    - If n is largest integer, then what is n+1
    - n < n+1
    - Therefore, there is no largest integer.

  ### Induction Proof
  - Induction is used to prove a series of iterations as a general concept that proves a starting case, and a general case to apply to every additional iteration.
  - This is important in Computer Science, because we often deal in iterative formulas and loops.
  - Claim: For every n in P(n) where n>=1.
    - Prove P(1) is true
    - Prove P(k) is true
    - Prove P(k+1) is also true

## Week-03
[09/07/26 - 09/13/26](#TOP)  

## Week-04
[09/14/26 - 09/20/26](#TOP)  

## Week-05
[09/21/26 - 09/27/26](#TOP)  

## Week-06
[09/28/26 - 10/04/26](#TOP)  

## Week-07
[10/05/26 - 10/11/26](#TOP)  

## Week-08
[10/12/26 - 10/18/26](#TOP)  

## Week-09
[10/19/26 - 10/25/26](#TOP)  

## Week-10
[10/26/26 - 11/01/26](#TOP)  

## Week-11
[11/02/26 - 11/08/26](#TOP)  

## Week-12
[11/09/26 - 11/15/26](#TOP)  

## Week-13
[11/16/26 - 11/22/26](#TOP)  

## Week-14
[11/23/26 - 11/24/26](#TOP)  

## Week-15
[11/30/26 - 12/06/26](#TOP)  
