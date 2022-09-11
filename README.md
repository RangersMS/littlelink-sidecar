# LittleLink-Sidecar

**⚠️ Work in progress**\
This project is in an early stage of development!

---

[LittleLink-Server](https://github.com/techno-tim/littlelink-server) relies on an external service like GitHub to host the avater. LittleLink-Sidecar adresses this by syncing the avatar of a user from a service like GitHub periodically and serve it via http locally. If you change your profile picture on that external service the change will automatically be adapted locally.

Add a rule for your reverse proxy to forward a specific path to LittleLink-Sidecar.

Example:\
Requests to `https://rengers.io/profile-media/` are forwarded to littelink-sidecar. Instead of loading a profile picture from GitHub into LittleLink-Server `https://rengers.io/profile-media/avatar` can be used. Littlelink-sidecar will periodically update the local avatar with your GitHub profile.
