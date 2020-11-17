Example envoy config for connecting to Kafka using X.509 SVIDs provided by SPIRE.

envoy.yaml.j2: Template for generating a config
vars.yaml: Template variables as used in the slides
example.yaml: config generated from the template, using the examples from the slides.

Usage: `j2 envoy.yaml.j2 vars.yaml > example.yaml`

Tested with Envoy 1.15.2. Health checks will initially fail until a connection with the SDS is established.
