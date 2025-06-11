# cse-231-assignment-4-solved
**TO GET THIS SOLUTION VISIT:** [CSE-231 Assignment 4 Solved](https://mantutor.com/product/cse-231-operating-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114216&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE-231 Assignment 4 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
Systems Section B

Topic: Concurrency and

1. All questions have to be done using the C programming language only.

2. The general guidelines mentioned in each question will ensure more readable code and an easier time during the demo for both you and your evaluator, so please follow them.

3. Helper functions can be added as necessary. Ensure that you are only using the synchronization primitive as mentioned in the question.

Question 1:

The dining philosophers problem (OSTEP Chapter 31, page 13) is a classic problem to demonstrate the concepts of deadlocks. The original setup contains five philosophers sitting on a round table, with a fork between each philosopher. Each philosopher can perform only one of two actions – eating and thinking. For eating, each philosopher requires 2 forks that are kept at their left and right sides. Allowing unrestricted access to each philosopher can lead to a deadlock.

Consider a modified version of the classic problem stated below:

Besides the 5 forks, there are now 2 bowls that are kept at the centre of the table.

For eating, each of them now requires two forks and a bowl.

Model the above problem using threads as philosophers. Specifically, each philosopher carries out 2 tasks, eating and thinking. Time required for both tasks can be simulated using the sleep() function (or any other function that causes a delay), and each philosopher must indicate what action it is carrying out by printing to the console.

You must also ensure that there are no deadlocks in the code. You are only allowed to use

Mutexes (locks) and Conditional Variables for this question

Guideline: Please structure your code to contain the following functions:

void* philosopher(void* args) // for running philosopher thread

void eating() // for entering eating state

void thinking() // for entering thinking state

Deliverables:

● C code

● Readme file explaining the following:

○ Why deadlocks can occur in the problem setup

○ How your proposed solution avoids deadlock.

○ Fairness of the

solution i.e. for your implementation, which and how many of the 5 philosopher threads are able to eat, and a rough estimate of how often a philosopher is able to eat (if at all).

Question 2: Imagine a situation where multiple passengers eagerly await their turn to take a ride in a car. This car has a limited capacity and can only set

off when fully occupied, with a maximum of C passengers on board (where C is less than the total number of passengers). Passengers have the simple tasks of getting on and off the car, while the car itself must manage the loading, running, and unloading procedures. Passengers are allowed to board only when the car has completed the loading process, and the car can commence its journey once it has reached its maximum passenger capacity. Passengers can disembark from the car only after it has completed its unloading process. Simulate the above by modeling the car and the passengers as threads. Take the total number of passengers and capacity as input from the user.

Simulate the above problem by modeling the passengers and car as threads. Specifically, the car thread has to do the following tasks:

1. Load specified number of passengers for the ride

2. Wait for all passengers to get on the ride

3. Run the duration of the ride

4. Unload all the passengers until ride is empty

Each passenger thread has to do the following:

1. Board the ride when it is available

2. Get off the ride when the ride is over

Time taken for each step can be simulated using the sleep function with appropriate duration, and every action carried out must be printed to console (in case of passengers, mention which passenger is carrying out the action using appropriate means). Synchronization can be carried out between car and passenger threads as necessary. Ensure that your code is deadlock-free. Use semaphores for synchronization.

Guidelines: Please ensure that the following functions are present in the code: void* car(void* args) // car thread void* passenger(void* args) // passenger thread

void load() //

loading car with passengers

void unload() //

unloading passengers

void board() //

passenger boards car

void offboard() // passenger gets off car

Deliverables:

● C code

● Writeup explaining code logic and how you avoid concurrency bugs in code

Question 3:

Modeling each car as a thread, write a program such that all cars from the left and the right side are able to cross without violating the above constraints (the number of cars on the left and right is to be taken as input from the user).

The following assumptions are also satisfied:

1. Once a car gets on the

bridge, it will definitely cross it.

2. Each car takes a fixed amount of time to cross the bridge. Crossing the bridge can be simulated as the thread calling the sleep() function.

For every thread that crosses the bridge, you must indicate which thread it is and which side it is originating from by printing appropriate information to the console. Use semaphores for synchronization.

Guidelines/Hint: It would be much easier to write different thread functions for left and right side cars. Therefore, please try and include the following functions:

void* left(void* args) // cars on the left

void* right(void* args) // cars on the right void passing(int

dir) // car from some direction is traveling on the bridge

Deliverables:

● C code

● Writeup explaining code

Published using Google Docs logic and how you avoid Report abuse Learn more concurrency bugs in code
