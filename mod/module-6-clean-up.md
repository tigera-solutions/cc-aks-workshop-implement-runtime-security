# Module 6 - Clean up

1. Delete the example application stacks.

   ```bash
   kubectl delete -f pre/005-vote-app-manifest.yaml
   ```

2. Delete the AKS cluster.

   ```bash
   az aks delete \
     --resource-group $RESOURCE_GROUP \
     --name $CLUSTERNAME
   ```

3. Delete the resource group.

   ```bash
   az group delete \
     --name $RESOURCE_GROUP
   ```

4. Delete this repo

   ```bash
   cd .. && rm -Rf cc-aks-implement-runtime-security
   ```

5. Delete environment variables backup file.

   ```bash
   rm ~/workshopvars.env
   ```

---

[:leftwards_arrow_with_hook: Back to Main](/README.md)  <br>

[:arrow_left: Module 5 - Quarantine Infected Workloads and Visualize KSPM](/mod/module-5-quarantine-kspm.md)
