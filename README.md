# Remote Debug action for neuro-flow to be used with Neu.ro template

This is a [`neuro-flow`](https://github.com/neuro-inc/neuro-flow) action enabling remote debugging. It's intended to be used with Neu.ro [platform template](https://github.com/neuro-inc/cookiecutter-neuro-project), but can be adapted for other use cases as well.

This action exposes SSH port (22) and maps it to port 2211 used for PyCharm remote Python debugging feature.

It also expectes references to 4 remotes: for data, config, code and results folders. These remotes will be mounted to `/project/data`, `/project/config`, `/project/modules` and `/project/results` respectively.