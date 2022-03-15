---
title: Running a BOX locally
id: box-setup
---

# Running a BOX locally

The easiest way to get the BOX server running locally is to clone our repo and use docker.

```
  > git clone https://github.com/functionland/fula
  > docker-compose -f docker-compose-dev.yml up
```

Next, take note of the [PeerID](https://docs.libp2p.io/concepts/peer-id/) that the BOX server created on startup.

To find that have a look at your docker-compose logs for the following -

```
box_1             | Swarm listening on /dns4/wrtc-star1.par.dwebops.pub/tcp/443/wss/p2p-webrtc-star/p2p/12D3KooWPeEhynWyG7dHytppDP6ZG6jhEv7LcDLWsExGq1YD784E
box_1             | Swarm listening on /dns4/wrtc-star2.sjc.dwebops.pub/tcp/443/wss/p2p-webrtc-star/p2p/12D3KooWPeEhynWyG7dHytppDP6ZG6jhEv7LcDLWsExGq1YD784E
```

Now head over to [using the samples](./using-samples) to verify the BOX server is running properly and that you are able to connect to it.