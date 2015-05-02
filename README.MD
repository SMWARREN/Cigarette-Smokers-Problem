Sean Warren

[![Alt text for your video](http://img.youtube.com/vi/k1tsGGz-Qw0/0.jpg)](https://www.youtube.com/watch?v=k1tsGGz-Qw0)

Video You Must Watch - Key & Peeles Hy On PotEnUse

# The Problem - The Cigarette Smokers Problem
----------------------------------------------------------------------------------------------
Write solution to solve the currently very un-PC"cigarette smokers problem" in java using Java threads, and monitors (using the "synchronized" keyword) (If it bothers your PC sensTosibilities, think of it at the Pot-smokers problem and then it is all proper again.

Consider a simulation with three smoker threads and one agent thread. Each smoker continuously makes a cigarette and smokes it. But to make a cigarette, a smoker needs three ingredients: tobacco, paper, and matches. One of the smoker threads has only paper, another has only tobacco, and the third has only matches. The agent thread has an infinite supply of all three materials. The three smoker threads are initially blocked. The agent places two randomly chosen (different) ingredients on the table and unblocks the one smoker who has the remaining ingredient. The agent then blocks. The unblocked smoker removes the two ingredients from the table, makes a cigarette, and smokes it for a random amount of time, unblocking the agent on completion of smoking the cigarette. The agent then puts out another random two of the three ingredients, and the cycle repeats.
> In this program I used Monitors, Array Lists and Agents "Java's monitor supports two kinds of thread synchronization: mutual exclusion and cooperation. Mutual exclusion, which is supported in the Java virtual machine via object locks, enables multiple threads to independently work on shared data without interfering with each other. 

> Cooperation, which is supported in the Java virtual machine via the wait and notify methods of class Object, enables threads to work together towards a common goal." - http://www.artima.com/insidejvm/ed2/threadsynch.html. This made it easy to implement a multithreaded program by extending classes throughout my project. The agents class helped me implement multithreading as well as the monitors, but made it easier to communicate between threads. An agent is an architectural foundation used to control other objects.

---------------------------------------------------
- An agent must have its own unique identity
- An agent host must allow multiple agents to co-exist and execute simultaneously
- Agents must be able to determine what other agents are executing in the agent host
- Agents must be able to determine what messages other agents accept and send
- An agent host must allow agents to communicate with each other and the agent host
- An agent host must be able to negotiate the exchange of agents
- An agent host must be able to freeze an executing agent and transfer it to another host
- An agent host must be able to thaw an agent transferred from another and allow it to resume execution
- The agent host must prevent agents from directly interfering with each other


# Errors
The only problem that I can find, is that the program runs forever because I never implemented a while loop with a decrementing variable.
