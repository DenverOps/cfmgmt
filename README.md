# cfmgmt
#### Troubleshooting
- hijack: Backend error: Exit status: 500, message: {"Type":"","Message":"runc exec: exit status 1: exec failed: container_linux.go:259: starting container process caused \"exec: \\\"config-repo/ci/tasks/cf-mgmt.sh\\\": permission denied\"\n","Handle":""}
- change add execute permisisons chmod +x ci/tasks/cf-mgmt.sh

#### how to update pipeline
- fly -t lite set-pipeline -p cf-mgmt -c pipeline.yml --load-vars-from=vars.yml

#### How to add org
- cf-mgmt-osx add-org-to-config --org test

#### How to add space
- cf-mgmt-osx add-space-to-config --org test --space dev