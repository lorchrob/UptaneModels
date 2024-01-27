# Tamarin models

This directory contains the Uptane Tamarin models. Below, we outline instructions for interacting with the Tamarin models, as well as an overview of the purpose of each `.spthy` file.

* To run the models, install the Tamarin prover ([Tamarin Prover (tamarin-prover.github.io)](https://tamarin-prover.github.io/)) and run the command `tamarin-prover interactive .`. Then, navigate to [http://127.0.0.1:3001/]() in your browser to interact with the Tamarin models.
* Some proofs take longer to prove automatically. So, we include the files SanityChecks.spthy, TargetsWeakAuth.spthy, OtherWeakAuth.spthy, and StrongAuth.spthy which contain proofs for the corresponding lemmas.
* Each Tamarin model has a commented-out key compromise rule. To simulate a situation with key compromise, the rule can be uncommented.
