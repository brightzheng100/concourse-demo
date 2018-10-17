# concourse-demo

Simple Concourse demo pipelines

# FAQ

1. `hijack` quits quietly without any reponse?

It's because some Docker images don't provide proper entry.
Try adding `/bin/sh` at the end of `hijack` cli, like:
`$ fly -t demo hijack -j pipeline-ring/job-ring /bin/sh`


