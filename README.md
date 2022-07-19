# tekton-samples
Sample Tekton tasks and pipelines used for testing and experimenting

The bundles are already available in the quay repo, so the example pipelineruns 
can be executed by creating the pipelineRun resource with a create command:

```
oc create -f pipelineruns/build_pipelinerun_pass.yaml
```

You can edit the tasks and pipelines and push them using the tkn bundle push command:

```
tkn bundle push quay.io/YOUR_REPO_HERE/test-bundle:build-pipeline-pass -f pipelines/build_pipeline_pass.yaml
```
