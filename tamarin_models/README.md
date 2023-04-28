# Tamarin models
* Presented modularly. Helps Tamarin's reasoning engine as it proves/disproves lemmas.
  We separate different parts of the protocol to help Tamarin's search. We split the model
  into VVM verification, image verification, and metadata verification.
* For image and metadata verification, we further split into whether or not
  there is a key compromise. The key compromise versions have an extra rule
  modeling the compromise. In theory, these could be wrapped together,
  but the separation makes the lemmas easier to parse.
* For some lemmas we run into issues with termination, so there is some commentary
  above troublesome lemmas about how to get Tamarin to terminate.
* At the Tamarin level, we only consider a primary with one secondary ECU (rather than
  two secondaries, like at the CRV level). This is because the properties
  that require reasoning about multiple secondaries (image compatibility issues)
  are not cryptographic.