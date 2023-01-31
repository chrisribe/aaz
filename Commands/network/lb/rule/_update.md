# [Command] _network lb rule update_

Update a load balancing rule.

## Versions

### [2022-05-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5uZXR3b3JrL2xvYWRiYWxhbmNlcnMve30=/2022-05-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/microsoft.network/loadbalancers/{} 2022-05-01 properties.loadBalancingRules[] -->

#### examples

- Update a load balancing rule to change the protocol to UDP.
    ```bash
        network lb rule update -g MyResourceGroup --lb-name MyLb -n MyLbRule --protocol Udp
    ```

- Update a load balancing rule to support HA ports.
    ```bash
        network lb rule update -g MyResourceGroup --lb-name MyLb -n MyLbRule \ --protocol All --frontend-port 0 --backend-port 0
    ```