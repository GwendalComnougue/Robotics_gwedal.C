# Robotics_gwedal.C

here you can find the kinematic direct and inverse of the spider robot.

![hexapod](https://user-images.githubusercontent.com/82094943/139660905-5f26ee78-0664-498c-998c-b32bfa6df795.jpg)


Direct kinematic :

P1:

Z1= 0		

X1= L1*cos(θ1)	

Y1= L1*sin(θ1)			                                                                                       										


P2:

Z2= L2* sin(θ2)		

X2= cos(θ1)*(L1+L2 cos(θ2))		


Y2= sin(θ1)*(L1+L2 cos(θ2))			



P3:		

Z3= sin(θ2)*(L2+sin(θ3*L3))			

X3= cos (θ1)*(L1+L2 cos(θ2)+L3 cos(θ2+θ3))	

Y3= sin (θ1)*(L1+L2 cos(θ2)+L3 cos(θ2+θ3))			



Inverse kinematic

θ1 = Arctan(X/Y)

θ2 = Arctan[sin(θ3-L3)/(L2+cos(θ3)L3)]

θ3 = Arcos [(x²+y²+(z-L1)²-L2²-L3²)/(2*L2*L3)]

you can find more information in the Kinematic.PDF


