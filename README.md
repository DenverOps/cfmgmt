# cfmgmt
#### Troubleshooting
- hijack: Backend error: Exit status: 500, message: {"Type":"","Message":"runc exec: exit status 1: exec failed: container_linux.go:259: starting container process caused \"exec: \\\"config-repo/ci/tasks/cf-mgmt.sh\\\": permission denied\"\n","Handle":""}
- change add execute permisisons chmod +x ci/tasks/cf-mgmt.sh