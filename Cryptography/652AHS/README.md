# 652AHS Challenge
![1](https://user-images.githubusercontent.com/62826765/77844821-9ca5b400-71a1-11ea-8932-a0f7cfb2994c.png)

First, we connect to the server :

![2](https://user-images.githubusercontent.com/62826765/77844857-f908d380-71a1-11ea-8681-1e2655d7832a.png)

He says that we have to select an option. Let's select the first option "Enter password" :

![3](https://user-images.githubusercontent.com/62826765/77844942-92d08080-71a2-11ea-8a0a-e798d71139c8.png)

So we have to enter a password to connect, but we don't have any password !
Then, let's try to reset it :

![4](https://user-images.githubusercontent.com/62826765/77845037-7c76f480-71a3-11ea-89d2-91e07c768897.png)

So to prove our identity and and reset the password, we have to answer the following 20 yes/no security questions. But are we going to bruteforce 2^20 possibilities ?! Naaah ofc not :D

We try to send "Yes" or "No" to some questions, we notice that sometimes it doesn't take the same time to pass to the next question, it means that he is comparing the answer to something, which leads us to the Timing Attack ! (https://en.wikipedia.org/wiki/Timing_attack)

If the answer is TRUE, he will take more time cause he will enter to a loop and compare all characters. If it's FALSE, he will break.

Based on that, we can determine all the answers and set new password :

![5](https://user-images.githubusercontent.com/62826765/77845613-2bb5ca80-71a8-11ea-9dbd-31238bf48ba7.png)

And BOOOOOOM !!

gigem{t1ck_t0ck_toCk_t111ck_tiCK_tockk}
