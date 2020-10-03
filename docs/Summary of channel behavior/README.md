# Summary of channel behavior

Summary 📝 of state of a channel 🆚 operations in Go.

Channels are the building blocks of concurrent go programs. A channel can have 4 states - nil, closed, full, or empty. We can perform send, receive, and close operations on them. Each combination of a state and operations yields a specific behavior. The following table summarizes this.

Read this as - A Send operation on the nil channel will block.

![IMAGE](channel_behavior.jpeg)
