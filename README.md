# Reinforcement-Learning
These are my notes on Reinforcement Learning. It would majorly contain 
1. Notes from David Silver lecture series(DeepMind channel)
2. Examples from github or other online sources
(Will also, try to take these online examples to my local environment and tinker with them, to try variations)


_____________________________________________________________________________________________________________________________
1.Notes from David Silver lecture series:

1. Lecture 1:
https://www.youtube.com/watch?v=2pWv7GOvuf0

http://www.cs.ucl.ac.uk/staff/D.Silver/web/Teaching.html

Books:
An introduction to Reinforcement Learning, Sutton and Barto (1998) available free online
http://webdocs.cs.ualbera.ca/~sutton/book/the-book.html

Algorithms for Reinforcement Learning, Szepesvari (smaller book)
http://www.ualberta.ca/~szepesva/papers/RLAlgsInMDPs.pdf



                                 About Reinforcement Learning
Sits at the intersection of many sciences.
Optimal way to make decisions.

There is no supervisor, only a reward signal. (Its a trial and error paradigm)
Feedback is delayed, not instantaneous.
Time really matters in RL. (sequential and non i.i.d data)
Agent's actions affect the subsequent data it receives.

Examples of RL:
Fly stunt manoeuvres in a helicopter
Play backgammon (defeat the world chamption)
manage investment portfolio
Control a power station
Make a humanoid robot walk
Play Atari games better than humans

                              The Reinforcement Learning Problem         
Reward Rt is a scalar feedback signal
Indicates how well agent is doing at step t
The agent's job is to maximise cumulative reward
RL is based on reward hypothesis
Reward Hypothesis
All goals can be described by the maximisation of expected cumulative reward
--Questions?
My question : What if the goal and reward is not one simple score. What if it has conflicting parts?
for example short term gratification vs long term success.
-- could probably be answered by choosing a holistic reward signal/funtion.

Examples of Rewards:
Money in case of finance related problems etc.
score in case of Atari games

                          Sequential Decision Making
Goal : Select actions to maximize total future reward
Actions may have long term consquences
Reward may be delayed
Cant be greedy, may be better to sacrifice now to gain more later

                    Agent and Environment
                    
Environment ---> (Observation,Reward) ---> Agent ---> Action --> Environment (Looped to first env.)
(Ot, Rt) ---> Agent ----> At

                  History and State
Ht = A1,O1,R1,.............,At,Ot,Rt
i.e. all observable variables upto time t
the future/what happens next depends on history
  the agent selects actions
  the env. selects obs and rewards
State is the information used to determine what happens next

Formally state is a function of history (any function)
            St = f(Ht)
Environment sate is environment's private representation
data the env. uses o pick the next obs/reward
the env. is usually not visible to the agent.
















