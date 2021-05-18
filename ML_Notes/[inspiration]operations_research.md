## Operations Research





Examples: https://web.stanford.edu/class/ee364a/lectures/examples.pdf



An amazing variety of practical problems involving decision making (or system design, analysis, and operation) can be cast in the form of a mathematical optimization problem, or some variation such as a multicriterion optimization problem. Indeed, mathematical optimization has become an important tool in many areas. It is widely used in engineering, in electronic design automation, automatic control systems, and optimal design problems arising in civil, chemical, mechanical, and aerospace engineering. Optimization is used for problems arising in network design and operation, finance, supply chain management, scheduling, and many other areas. The list of applications is still steadily expanding.

https://web.stanford.edu/~boyd/cvxbook/bv_cvxbook.pdf



**Applications**: 

For most of these applications, mathematical optimization is used as an aid to a human decision maker, system designer, or system operator, who supervises the process, checks the results, and modifies the problem (or the solution approach) when necessary. This human decision maker also carries out any actions suggested by the optimization problem, e.g., buying or selling assets to achieve the optimal portfolio.

**In portfolio optimization, f**or example, we seek the best way to invest some capital in a set of n assets. The variable xi represents the investment in the ith asset, so the vector x ∈ R n describes the overall portfolio allocation across the set of assets. The constraints might represent a limit on the budget (i.e., a limit on the total amount to be invested), the requirement that investments are nonnegative (assuming short positions are not allowed), and a minimum acceptable value of expected return for the whole portfolio. The objective or cost function might be a measure of the overall risk or variance of the portfolio return. In this case, the optimization problem (1.1) corresponds to choosing a portfolio allocation that minimizes risk, among all possible allocations that meet the firm requirements.



Another example is **device sizing in electronic design,** which is the task of choosing the width and length of each device in an electronic circuit. Here the variables represent the widths and lengths of the devices. The constraints represent a variety of engineering requirements, such as limits on the device sizes imposed by the manufacturing process, timing requirements that ensure that the circuit can operate reliably at a specified speed, and a limit on the total area of the circuit. A common objective in a device sizing problem is the total power consumed by the circuit. The optimization problem (1.1) is to find the device sizes that satisfy the design requirements (on manufacturability, timing, and area) and are most power efficient



**In data fitting, th**e task is to find a model, from a family of potential models, that best fits some observed data and prior information. Here the variables are the parameters in the model, and the constraints can represent prior information or required limits on the parameters (such as nonnegativity). The objective function might be a measure of misfit or prediction error between the observed data and the values predicted by the model, or a statistical measure of the unlikeliness or implausibility of the parameter values. The optimization problem (1.1) is to find the model parameter values that are consistent with the prior information, and give the smallest misfit or prediction error with the observed data (or, in a statistical



### More Examples: 

* Network flow - Max flow
* Max likelihood  - Least square regresion 
* Compression sensing 
* SVM - regulairzed likelihood 

---



- [critical path analysis](https://en.wikipedia.org/wiki/Critical_path_analysis) or [project planning](https://en.wikipedia.org/wiki/Project_planning): identifying those processes in a complex project which affect the overall duration of the project

- [Floorplanning](https://en.wikipedia.org/wiki/Floorplanning): designing the layout of equipment in a factory or components on a [computer chip](https://en.wikipedia.org/wiki/Computer_chip) to reduce [manufacturing](https://en.wikipedia.org/wiki/Manufacturing) time (therefore reducing cost)

- [Network optimization](https://en.wikipedia.org/wiki/Telecommunications_network): for instance, setup of telecommunications or power system networks to maintain quality of service during outages

- [Resource allocation](https://en.wikipedia.org/wiki/Resource_allocation) problems

- [Facility location](https://en.wikipedia.org/wiki/Facility_location_(optimization_problem))

- Assignment Problems:

  - [Assignment problem](https://en.wikipedia.org/wiki/Assignment_problem)
  - Generalized assignment problem
  - [Quadratic assignment problem](https://en.wikipedia.org/wiki/Quadratic_assignment_problem)
  - [Weapon target assignment problem](https://en.wikipedia.org/wiki/Weapon_target_assignment_problem)

- [Bayesian search theory](https://en.wikipedia.org/wiki/Bayesian_search_theory): looking for a target

- [Optimal search](https://en.wikipedia.org/wiki/Search_theory)

- [Routing](https://en.wikipedia.org/wiki/Routing), such as determining the routes of buses so that as few buses are needed as possible

- [Supply chain management](https://en.wikipedia.org/wiki/Supply_chain_management): managing the flow of raw materials and products based on uncertain demand for the finished products

- Project production activities: managing the flow of work activities in a capital project in response to system variability through operations research tools for variability reduction and buffer allocation using a combination of allocation of capacity, inventory and time[[29\]](https://en.wikipedia.org/wiki/Operations_research#cite_note-29)[[30\]](https://en.wikipedia.org/wiki/Operations_research#cite_note-30)

- Efficient messaging and customer response tactics

- [Automation](https://en.wikipedia.org/wiki/Automation): automating or integrating robotic systems in human-driven operations processes

- [Globalization](https://en.wikipedia.org/wiki/Globalization): globalizing operations processes in order to take advantage of cheaper materials, labor, land or other productivity inputs

- Transportation: managing [freight](https://en.wikipedia.org/wiki/Freight) transportation and delivery systems (Examples: [LTL shipping](https://en.wikipedia.org/wiki/Less_than_truckload_shipping), [intermodal freight transport](https://en.wikipedia.org/wiki/Intermodal_freight_transport), [travelling salesman problem](https://en.wikipedia.org/wiki/Travelling_salesman_problem))

- Scheduling

  :

  - [Personnel staffing](https://en.wikipedia.org/wiki/Nurse_scheduling_problem)
  - Manufacturing steps
  - [Project tasks](https://en.wikipedia.org/wiki/Project_management)
  - Network data traffic: these are known as [queueing models](https://en.wikipedia.org/wiki/Queueing_model) or queueing systems.
  - Sports events and their television coverage

- Blending of raw materials in oil refineries

- Determining optimal prices, in many retail and B2B settings, within the disciplines of [pricing science](https://en.wikipedia.org/wiki/Pricing_science)

- [Cutting stock problem](https://en.wikipedia.org/wiki/Cutting_stock_problem): Cutting small items out of bigger ones.

Operational research is also used extensively in government where [evidence-based policy](https://en.wikipedia.org/wiki/Evidence-based_policy) is used.







**The challenge, and art, in using convex optimization is in recognizing and formulating the problem. Once this formulation is done, solving the problem is, like least-squares or linear programming, (almost) technology.**

---

Solutions: 



A solution method for a class of optimization problems is an algorithm that computes a solution of the problem (to some given accuracy), given a particular problem from the class, i.e., an instance of the problem. Since the late 1940s, a large effort has gone into developing algorithms for solving various classes of optimization problems, analyzing their properties, and developing good software implementations. The effectiveness of these algorithms, i.e., our ability to solve the optimization problem (1.1), varies considerably, and depends on factors such as the particular forms of the objective and constraint functions, how many variables and constraints there are, and special structure, such as sparsity. (A problem is sparse if each constraint function depends on only a small number of the variables).



A least-squares problem is an optimization problem with no constraints (i.e., m = 0) and an objective which is a sum of squares of terms of the form a T i x − bi :



Another important class of optimization problems is linear programming



---



### Interesting Videos: 



Operations Research: https://youtu.be/0oMVVx81kCs



Econometrics and Operations Research: https://youtu.be/x91n_aIqA8Y

 ###  What is 'econometrics'? 

https://youtu.be/3C0UAXktkdQ

---



Books: 



Introductory Economtrics - A modern Approach



---



Optimisation

- W L Winston, Operations Research: Applications and Algorithms, Brooks/Cole (4th ed., 1998)
- D Bertsimas and J N Tsitsiklis, Introduction to Linear Optimization, Athena Scientific (3rd ed., 1997)
- George B. Dantzig and Mukund N. Thapa, Linear Programming 2: Theory and extensions, Springer (2003)

Simulation

- S Ross, Simulation, Academic Press (5th ed., 2012)
- A M Law and W D Kelton, Simulation Modelling and Analysis, McGraw Hill (3rd ed., 2000)
- M Pidd, Computer Simulation in Management Science, Wiley (5th ed., 2006)