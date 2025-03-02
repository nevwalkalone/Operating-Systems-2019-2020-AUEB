# Second Assignment

Read this [section](https://github.com/nevwalkalone/POSIX-Projects/blob/main/README.md) (if you haven't already), before proceeding.

In this second assignment there have been added deliverers
who deliver the orders to the clients. The way the cooks perform is also changed.

The pizzeria has 𝑁𝑐𝑜𝑜𝑘 cooks, 𝑁𝑜𝑣𝑒𝑛 ovens and 𝑁deliverer deliverers. The first order is
made at the time 0, and every next order is made after a random period of time and it ranges in
the interval [𝑇𝑜𝑟𝑑𝑒𝑟𝑙𝑜𝑤, 𝑇𝑜𝑟𝑑𝑒𝑟ℎ𝑖𝑔ℎ]. Every order includes a random integer number of pizzas in
the interval [𝑁𝑜𝑟𝑑𝑒𝑟𝑙𝑜𝑤, 𝑁𝑜𝑟𝑑𝑒𝑟ℎ𝑖𝑔ℎ]. The order has to wait until a cook is available. When a cook
is available, a 𝑇𝑝𝑟𝑒𝑝 amount of time is required for each pizza to be prepared for the oven. Then,
the cook waits until an oven is available. When an oven is available, all pizzas of the particular
order go into the same oven and bake for 𝑇𝑏𝑎𝑘𝑒 amount of time. Note that the cook is available
for a new order right after placing the pizzas in the oven (he does not wait for the pizzas to be
baked). When the pizzas are baked, the oven turns automatically off and waits for a deliverer.
When a deliverer is available, he/she takes all pizzas of the particular order out of the oven (which is
then available for another order). He/she then packs the order and delivers it to the client. The
delivery lasts for a random (integer) period of time in the interval [𝑇𝑙𝑜𝑤, 𝑇ℎ𝑖𝑔ℎ]. After the delivery, the
deliverer needs the same amount of time to return to the pizzeria and to take on the next
order. Every cook deals with only one order each time, from the moment the order is handed to
him/her until it is placed inside the oven. Every deliverer delivers only one order each time he/she
goes out of the pizzeria.

## Useful Reads

For a full overview it is highly suggested that you read:

- [Project Assignment](assignment-report/project2-assignment.pdf), that contains all the details about the assignment's tasks.
- [Project Report](assignment-report/project2-report.pdf), that contains all the details about the actual implementation of this system and the analysis of the code.

## Program Execution

1. **Clone** repository

   ```console
   git clone https://github.com/nevwalkalone/POSIX-Projects.git
   ```

2. **Change** directory to src

   ```console
   cd POSIX-Projects/2nd-Assignment/src
   ```

3. **Run** `test-res2.sh` script which will compile and execute `pizza2.c` with 2 integer parameters, 100 (total orders) and 1000 (for the initial seed)

   ```console
   ./test-res2.sh
   ```
