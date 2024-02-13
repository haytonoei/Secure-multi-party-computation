# Secure-multi-party-computation (MPC)
Solution 3: allows parties to perform computations on data while keeping that data private

 mathematical, replaced by TEE, never decrypt, homomorphic encryption 

"combines sketches without ever decrypting them and only computes a single noisy reach and frequency estimate

main features:
1. It computes its output solely on encrypted inputs, which remain encrypted even while
being computed upon, and only agreed upon outputs are ever revealed. Moreover, such
outputs can be made differentially private as part of the encrypted work load.
2. Its error for both reach and frequency computation is constant regardless of the number
of inputs, which means it can scale to any number of data providers without losing any
accuracy.
3. Its security model is distributed, which means that:
a. There is no single trusted third party that must be relied upon for either
trustworthiness of output or security of data.
b. Only explicitly requested outputs are computed and there will be several
independent logs of these.
c. The only information learned from running the system is the agreed upon outputs
of the system
d. Compromising a single component of the system will not allow an attacker to
learn anything about data provider inputs. Indeed all components of the system
would need to be compromised in order for any of the encrypted inputs to be
revealed, which is a huge advantage in a world where high profile data breaches
seem all too common."

source: google research,"A System Design for Privacy-Preserving Reach and Frequency Estimation"
