NAME            READY   STATUS             RESTARTS      AGE
bad-sleep-pod   0/1     CrashLoopBackOff   6 (91s ago)   11m
Name:             bad-sleep-pod
Namespace:        default
Priority:         0
Service Account:  default
Node:             docker-desktop/192.168.65.3
Start Time:       Thu, 08 May 2025 19:35:55 +0300
Labels:           <none>
Annotations:      <none>
Status:           Running
IP:               10.1.0.36
IPs:
  IP:  10.1.0.36
Containers:
  bad-sleep:
    Container ID:   docker://7976c64d1e5bc00ca3680c8e3b46d1a2ad593f33b7c9965f5ce77fe302beba9b
    Image:          courselabs/bad-sleep
    Image ID:       docker-pullable://courselabs/bad-sleep@sha256:248b6bf6909533baa38a9c6913941895b69688bc6008ffa138e503199ff5c90d
    Port:           <none>
    Host Port:      <none>
    State:          Waiting
      Reason:       CrashLoopBackOff
    Last State:     Terminated
      Reason:       Completed
      Exit Code:    0
      Started:      Thu, 08 May 2025 19:44:59 +0300
      Finished:     Thu, 08 May 2025 19:45:29 +0300
    Ready:          False
    Restart Count:  6
    Limits:
      cpu:     500m
      memory:  128Mi
    Requests:
      cpu:        250m
      memory:     64Mi
    Environment:  <none>
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-z5nz6 (ro)
Conditions:
  Type                        Status
  PodReadyToStartContainers   True 
  Initialized                 True 
  Ready                       False 
  ContainersReady             False 
  PodScheduled                True 
Volumes:
  kube-api-access-z5nz6:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    ConfigMapOptional:       <nil>
    DownwardAPI:             true
QoS Class:                   Burstable
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type     Reason     Age                     From               Message
  ----     ------     ----                    ----               -------
  Normal   Scheduled  11m                     default-scheduler  Successfully assigned default/bad-sleep-pod to docker-desktop
  Normal   Pulled     11m                     kubelet            Successfully pulled image "courselabs/bad-sleep" in 12.525s (12.525s including waiting). Image size: 4312009 bytes.
  Normal   Pulled     10m                     kubelet            Successfully pulled image "courselabs/bad-sleep" in 2.64s (2.64s including waiting). Image size: 4312009 bytes.
  Normal   Pulled     9m39s                   kubelet            Successfully pulled image "courselabs/bad-sleep" in 2.946s (2.946s including waiting). Image size: 4312009 bytes.
  Normal   Pulled     8m40s                   kubelet            Successfully pulled image "courselabs/bad-sleep" in 2.715s (2.715s including waiting). Image size: 4312009 bytes.
  Normal   Pulled     7m26s                   kubelet            Successfully pulled image "courselabs/bad-sleep" in 2.755s (2.755s including waiting). Image size: 4312009 bytes.
  Normal   Pulled     5m28s                   kubelet            Successfully pulled image "courselabs/bad-sleep" in 2.897s (2.898s including waiting). Image size: 4312009 bytes.
  Normal   Created    5m27s (x6 over 10m)     kubelet            Created container: bad-sleep
  Normal   Started    5m27s (x6 over 10m)     kubelet            Started container bad-sleep
  Warning  BackOff    2m29s (x26 over 9m53s)  kubelet            Back-off restarting failed container bad-sleep in pod bad-sleep-pod_default(41c35a72-a540-4bb7-96f4-6e5977495e41)
  Normal   Pulling    2m17s (x7 over 11m)     kubelet            Pulling image "courselabs/bad-sleep"
  Normal   Pulled     2m14s                   kubelet            Successfully pulled image "courselabs/bad-sleep" in 2.98s (2.98s including waiting). Image size: 4312009 bytes.
