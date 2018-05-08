# Pendulum Waves

This is a simulation of a "wave pendulum." A wave pendulum refers to a number of pendulums with monotonically varying lengths, such that each pendulum executes one less full cycle than the pendulum next to it in some fixed amount of time. The result is a hypnotic pattern that arises and disintegrates into seeming chaos only to reappear at the end of its cycle.

<br> </br>
<body> 
    <p> Upon first attempt, I calculated the pendula lengths with discrete increments of some finite value. Upon observation though, this does not reveal the pendulum wave patterns desired. For that, each pendulum must have an integer multiple number of oscillations in a full pendulum wave period. If the longest pendulum makes 10 oscillations in the total period of the system, then the other n pendula must make 10 + 1, 10 + 2, 10 +3, ... 10 + n, oscillations in the same time period to reveal the desired pattern.
    </p>
    </br>
    <p> To calculate the pendula lengths for N pendula, I assumed a small angle approximation so that
    
    $$T = 2\pi \sqrt{\frac{l}{g}}$$ . Now if the total period is $T_{tot}$, then 
    <br> </br>
    <br>  </br>
    $$T = \frac{T_{tot}}{N+n}$$ where N is the number of oscillations of the largest pendulum and n is the number of the nth pendulum. Setting these equal and solving for the length gives the lambda function included in the code below. 
    
    $$l(n) = g(\frac{T_{tot}}{2\pi(N + n)})^2$$
    </p>
    
    <p> In order to create a parabolic length pattern, I used the formula  
        $$l(n) = g(\frac{T_{tot}}{2\pi(N + n^{2})})^2$$
        
        </p>
        <p>
        And created an array of pendulum lengths iterating from -n/2 to n/2. The head on view, however, only shows half of the pendulum because the other half are exactly the same and perfectly overlap.

    </p>
    
    
    <p> As a side note, the total period is set to 60 seconds, so around 60 seconds the entire pattern should restart </p>
    

</body>
