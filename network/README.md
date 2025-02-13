If you ever want to use this test know that you have to spin up the iperf server first. Get the ip and then edit the client yaml.


`k apply -f iperf3-server.yaml`

`kubectl get pod iperf3-server -o jsonpath='{.status.podIP}'`

`k apply -f iperf3-client.yaml`