# zero0knowledge-proof

This is a demo to show How can you prove your age to facebook that you are above 14 without revelaing your exact age.

Consider the scenario Yoshika who is ‘n’ years old needs to prove to facebook she is atleast ‘m’ years old.
Yoshika age is ‘n’ and need to prove to facebook that her age is  atleast ‘m’, Yoshika sends sends the “Verified age” and “Proof” to Facebook. Facebook start applying hash chaining with “Proof” ‘m’ times and check the result match with the “Verified age”. If two values are same, the Facebook can let Yoshika use facebook services. If two values are different, then Facebook can assume child’s statement was false.   

VerifiedAge=Hash (n times) (seed_value)
Proof = Hash (n-mtimes) (seed_value)
VerifiedEdge == Hash (m times) (seed_value)

n = age of child
m = age to prove
x = seed generated by trusted party
Proof P is generated by Trusted party
Verified age V is generated by Yoshika
m times Hash is generated by Facebook to check if age is atleast m or not.

