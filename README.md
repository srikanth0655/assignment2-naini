# assignment2-naini
# Srikanth Naini
### Niagara Falls
When it comes to the natural wonders of the world, Niagara Falls continues to intrigue. Created as water flowed into the Niagara River from the North American Great Lakes **12,000 years** ago, these three spectacular waterfalls form the hub of a sightseeing and recreational area with enough outdoor and indoor activities to make **a great weekend getaway** or extended vacation


--- 
##  Directions from Maryville to Kansas City 
1. Book a cab from Maryville to Kansas Airport.
2. Finish the check-in process through online.
   1. Take boarding pass from the self service kiosk.
   2. Waiting for the flight
   3. Board your flight.
3. Complete your check out process at Hyderabad.


* Clothes
    * sweater
    * shoes
* Cosmetics
    * Sunscreen Lotion
    * Facewash
* Money
* Snacks
    * Chocolates
    * Biscuits

    [AboutMe](https://github.com/srikanth0655/assignment2-naini/blob/main/AboutMe.md)

    ---

    # Table Creation

    A table with three columns recommends the some of the best foods that i experienced in India.

    | Food/Drink    |   Location    | Price |
    |   ---         |   ---         |  ---  |
    |Chicken Nuggets|   McDonalds   |  $4   |
    | Chicken Pizza |   PizzaHut    |  $3   |
    | Tuna          |  starbucks    |  $2   |

    ---

# Quotes and Autors

> "Be the change you want to see in the world" - By
 *Mahatma Gandhi*     <br>                     
>  "Screw it ,Let's do it" - By 
*Richard Branson*



-----
## Code Fencing (Graph traversal)
In computer science, graph traversal (also known as graph search) refers to the process of visiting (checking and/or updating) each vertex in a graph. Such traversals are classified by the order in which the vertices are visited. Tree traversal is a special case of graph traversal.<https://en.wikipedia.org/wiki/Graph_traversal>

```
vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}
```
<https://cp-algorithms.com/graph/breadth-first-search.html>

