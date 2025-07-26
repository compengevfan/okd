Web User Guide: 
https://developer.1password.com/docs/k8s/k8s-operator/?deployment-type=manual

You will need "1password-credentials.json" which can be obtained from 1password.com

To Create the “op-credentials” secret, do this, not what’s in the web guide
cat 1password-credentials.json | base64 | tr '/+' '_-' | tr -d '=' | tr -d '\n' > op-session

After cloning the 1password operator repo, replace the "manager.yaml" file with the one you updated.

After running “make deploy”, wait for the “onepassword-connect” deployment to show up. Scale it down 0 and update the YAML to set: runAsNonRoot: false