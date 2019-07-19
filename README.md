# atlassistant

**atlassistant** is the place where are discuted and elaborated the principes of a tailor-made, hackable and privacy respectful "intelligent" virtual assistant.

This repository holds what's in our head for the future of this project.

## Motivation

The concept of **atlassistant** was born following the revelations of collect and misuse of private informations from most of the GAFA(M) and the release of cheap and powerful personal computers like the Raspberry. We believe that it is now possible to offer an alternative to the market major virtual assistants: a solution that is hackable (in a DIY approach), 100% open source and working on personal equipment without information gathering.

## Approach

Instead of putting everything in a single repository, the goal is to create a library which handle the understanding and acting parts of the system and let everyone embed this library in their own program. So by definition, there is no user interface in the core library.

Going from idea to implementation should be as easy as possible, including writing training samples, translations and handlers.

To make it more end user friendly, satellite projects are being built to expose an agent (ie. your assistant with its state) on communication channels (such as MQTT or WebSockets).

The final step is then to develop some clients (Terminal, chatbots, audio pod, mobile app, web app) which connect to an agent using those channels.

## Current status

The core library has been built in **Python** and is called [pytlas](https://github.com/atlassistant/pytlas). It already works pretty well, has many tests, can be integrated in people's programs without a hassle and has been tested on a Raspberry Pi 3.

We are currently building other components such as a broker to expose this library on multiple communication channels and the final step will be to create client apps and skills to make it really useful to people.

## Contributing

All ideas/help are welcome, you can already [develop some skills](https://pytlas.readthedocs.io/en/latest/writing_skills/index.html), talk about this project and submit PRs.
