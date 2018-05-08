# Pendulum Waves
<body>
<p>This is a simulation of a "wave pendulum." A wave pendulum refers to a number of pendulums with monotonically varying lengths, such that each pendulum executes one less full cycle than the pendulum next to it in some fixed amount of time. The result is a hypnotic pattern that arises and disintegrates into seeming chaos only to reappear at the end of its cycle. </p>

<p> To run, simply run pendulum.py </p>

<p> Upon first attempt, I calculated the pendula lengths with discrete increments of some finite value. Upon observation though, this does not reveal the pendulum wave patterns desired. For that, each pendulum must have an integer multiple number of oscillations in a full pendulum wave period. If the longest pendulum makes 10 oscillations in the total period of the system, then the other n pendula must make 10 + 1, 10 + 2, 10 +3, ... 10 + n, oscillations in the same time period to reveal the desired pattern. </p>
    
<p> As a side note, the total period is set to 60 seconds, so around 60 seconds the entire pattern should restart </p>
    

</body>
