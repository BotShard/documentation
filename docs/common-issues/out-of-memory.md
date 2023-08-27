---
sidebar_position: 3
---

# Out Of Memory / Killed

It's worth noting that our free tier imposes limits on RAM and CPU usage, which may not be sufficient for larger bots that require more resources to fetch from NPM. If you're hosting a large bot, you may want to consider purchasing our paid tier.

If you're unable to upgrade to a paid tier, you could try a workaround. First, run your bot on your local machine. Then, zip the entire directory's contents, including `node_modules`. Finally, upload the zipped file to the server and unzip it via the file manager.

:::caution

If you are using native Node modules (modules that must be compiled into bytecode, such as `canvas`), this workaround will probably not work unless you have an ARM64 computer.

:::
