# Week 1 Live Session

## 8/24/2022

- Live sessions will be focused on exploration of related topics.
- Not many grades. Two papers, two projects.
- Midterm and final. Very challenging. Open-ended, expla
- Example (Freebie): `Describe purpose of bell's inequality, what experiments are related to bell's inequality?`
- Not taking attendance.
- Not a lot of sympathy for late submissions.
- elliptic curve more secure than RSA.

### Discussion

- in late 1800s, early 1900s, some people thought all things about physics had already been figured out
  - nature of light was problematic. **wave? particle?** different people were doing different experiments which triggered different behaviors of light, driven by different parameters.
  - Black body radiation. What determines how many electrons are knocked off a particle? Quantization of energy.
- All subatomic particles are a **probability wave** (it plots out like a wave when graphed, not actually moving like a wave). In the macro world, things either are or are not. In the subatomic world, a particular subatomic particle has a probability of being in different states.
  - Wave-particle duality. Subatomic particle is in a **superposition** of all possible states until something happens. (until you _collapse the wave function_). This is fundamentally bizarre. **The universe is fundamentally weird, empirically.**
    - This means you can do things with a qubit (**quantum bit = qubit; the counterpart in quantum computing to the bit in classical computing**) that you cannot do with a classical bit.
- Decoherence: problem in quantum computing. When qubit wave function collapses before you are ready for it to collapse.
- Entanglement. Two subatomic particles sharing a wave function, so if you collapse one it collapses the other. Instantaneously. Despite Albert Einstein proving that nothing happens instantaneously.
  - Non-locality -> when two particles are entangled.
  - Sometimes we want to entangle two qubits. Other times we don't want this but it still happens which causes issues.
  - No one understands this. Has been researched over many decades. First experiments tried to prove that entanglement wasn't real.
  - [**Bell's inequality** / **Bell's theorem**](https://en.wikipedia.org/wiki/Bell%27s_theorem) was designed to give an alternative explanation for entanglement. He deduced that if measurements are performed independently on the two separated particles of an entangled pair, then the assumption that the outcomes depend upon hidden variables within each half implies a mathematical constraint on how the outcomes on the two measurements are correlated. This constraint would later be named the Bell inequality. Bell then showed that quantum physics predicts correlations that violate this inequality. Consequently, the only way that hidden variables could explain the predictions of quantum physics is if they are "nonlocal", which is to say that somehow the two particles were able to interact instantaneously no matter how widely the two particles are separated
  - [Shor's algorithm, breaking RSA](https://en.wikipedia.org/wiki/Shor%27s_algorithm), developed 1994 by American mathematician Peter Shor. It's really hard to factor a large integer into its prime factors. If you can factor a large number into its prime factors easily, you could quite easily get the public and private key. Assume that a quantum computer may allow you to crack a public & private key in, say, 3 weeks. Certs are usually installed for a year. This voids HTTPS.
    - Where are we with this algorithm? Still theoretical? Hardware caught up?
    - **If a quantum computer with a sufficient number of qubits could operate without succumbing to quantum noise and other quantum-decoherence phenomena**, then Shor's algorithm **could** be used to break public-key cryptography schemes, such as
      - The RSA scheme
      - The Finite Field Diffie-Hellman key exchange
      - The Elliptic Curve Diffie-Hellman key exchange[6]
    - Take a smaller integer, factor it with Shor's algo on a quantum computer. Take that same small integer and factor with classical computer. Use difference in computation time to extrapolate how long it would take to factor real large integer and prove that quantum can solve problem in X time.
- Pre-wright brothers, war department consistently tried and failed to build flying machines. Someone said "men will fly someday, but only after tons of expenditure/investment/etc." Wright bros build successful machine a week later. By "doing things differently".

  - **So many people working** on addressing decoherence, problems in quantum computing in so many different ways that it's **almost guaranteed** that problems will be solved.

#### End of Class Speculative Prompt

Roger Penrose, professor Ameritus of Oxford in mathematical physics, now 91. Received Nobel prize a few years ago. He and Stuart Hameroff [claimed in 1990s](https://theconversation.com/can-consciousness-be-explained-by-quantum-physics-my-research-takes-us-a-step-closer-to-finding-out-164582) that human consciousness arises due to quantum fluctuations in microtubules in neurons. Microtubules are scaffolding in neurons, they help guide protein formation, DNA formation. Issues that affect microtubules cause diseases. Connection between microtubules issues and alzheimers which degrades consciousness.

- People argued against it because they thought there is no way to store and process information in quantum states. Those are void.
- Others said you will never get quantum behavior at room temperature. However, quantum physics are at play in biology within plants, proved empirically.
- What if they are right? What if our consciousness is based on quantum fluctuations in neuron microtubules? If we are intentionally creating quantum fluctuations in machines, does that mean we are "creating" synthetic consciousness?
