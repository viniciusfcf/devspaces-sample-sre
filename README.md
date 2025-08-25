# devspaces-sample-sre
## Red Hat OpenShift Dev Spaces SRE Sample

### Documentation

- [Configuring Getting Started Samples in OpenShift Dev Spaces](https://docs.redhat.com/en/documentation/red_hat_openshift_dev_spaces/3.22/html-single/administration_guide/index#configuring-getting-started-samples)

### Installing `sre-samples.json` in OpenShift Dev Spaces

1. **Download the `sre-samples.json` file**
	- Ensure you have the `sre-samples.json` file from this repository.

2. **Access your OpenShift Dev Spaces instance**
	- Log in to your OpenShift cluster and open the Dev Spaces dashboard.

3. **Create a ConfigMap with the samples configuration:**
	`oc create configmap sre-started-samples --from-file=sre-samples.json -n openshift-devspaces`

4. **Add the required labels to the ConfigMap**
	`oc create configmap sre-started-samples --from-file=sre-samples.json -n openshift-devspaces`

5. **Verify installation**
	- The SRE CloudOps Workspace sample should now appear in the Dev Spaces samples list.
	- Launch a workspace using the sample to verify it works as expected.

For more details, refer to the [official documentation](https://docs.redhat.com/en/documentation/red_hat_openshift_dev_spaces/3.22/html-single/administration_guide/index#configuring-getting-started-samples).