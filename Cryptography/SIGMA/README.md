# SIGMA Challenge

![0](https://user-images.githubusercontent.com/62826765/77846301-29a23a80-71ad-11ea-866c-953f38127112.png)

We were given a long number :
10320831141252164475480592397410881183128414021520157116851780189419421991209921942315241625302578269728072902300131153236334834643575368637343782389340044129

After analyzing it we found that the first 3 digits are the ASCII of "g", but the 3 next digits doesn't give us anything. 
We go back to the title, Sigma's symbol is the symbol of sum that we use in Maths. Hmmmm, so it's all about sum ! 

We do 208-103 = 105 which is the ASCII of "i" and 311-208 = 103 which is the ASCII of "g" ...

So we write a script:
"""
sigma = [103,208,311,412,521,644,754,805,923,974,1088,1183,1284,1402,1520,1571,1685,1780,1894,1942,1991,2099,
	 2194,2315,2416,2530,2578,2697,2807,2902,3001,3115,3236,3348,3464,3575,3686,3734,3782,3893,4004,4129]

flag = chr(sigma[0])
for i in range(len(sigma)-1):
	flag += chr(sigma[i+1]-sigma[i])

print flag
"""
And here we are :

![1](https://user-images.githubusercontent.com/62826765/77846626-450e4500-71af-11ea-9c88-9197163e0779.png)


gigem{n3v3r_evv3r_r01l_yer0wn_cryptoo00oo}
