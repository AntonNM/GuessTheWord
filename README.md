
Coturn server conf

https://www.videosdk.live/developer-hub/stun-turn-server/webrtc-turn-server

```
   listening-port=3478
   fingerprint
   use-auth-secret
   static-auth-secret=mysecret
   realm=my-turn-server.mycompany.com
   total-quota=100
   bps-capacity=0
   stale-nonce=600
   no-multicast-peers
   no-cli
   log-file=/var/log/turnserver.log
   simple-log

```


# Kubernetes

### web Server

Deployment
LoadBalancer service
CPU HorizontalPodAutoscalar (HPA)

### Signaling Server

Statefulset
Headless service
CPU HPA



### Coturn 

TBD
option 1.)
StatefulSet
HeadlessService
CPU HPA
