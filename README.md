# Remote Debug action for apolo-flow to be used with Apolo flow template

This is a [`apolo-flow`](https://github.com/neuro-inc/neuro-flow) action enabling remote debugging. It's intended to be used with Apolo [platform template](https://github.com/neuro-inc/flow-template), but can be adapted for other use cases as well.

This action exposes SSH port (22) and maps it to port 2211 used for PyCharm remote Python debugging feature.

It also expectes references to 4 remotes: for data, config, code and results folders. These remotes will be mounted to `/project/data`, `/project/config`, `/project/modules` and `/project/results` respectively.