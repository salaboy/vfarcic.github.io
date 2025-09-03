<!-- .slide: data-background="../img/background/hands-on.jpg" -->
## Hands-on Time

# Setup


> Install [NodeJS](https://nodejs.org/en/download) if you don't have it already.

```sh
npm install -g @anthropic-ai/claude-code

git clone https://github.com/vfarcic/dot-ai-demo

cd dot-ai-demo

git pull

git fetch

git switch policies
```


> Make sure that Docker is up-and-running. We'll use it to create a KinD cluster.

> Watch [Nix for Everyone: Unleash Devbox for Simplified Development](https://youtu.be/WiFLtcBvGMU) if you are not familiar with Devbox. Alternatively, you can skip Devbox and install all the tools listed in `devbox.json` yourself.


```sh
devbox shell

./dot.nu setup --dot-ai-tag 0.81.0 --qdrant-run false --qdrant-tag 0.7.0

source .env

claude
```
