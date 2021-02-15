Current state:
- Components deploy without error
- RDS deployment takes a little while, but wait: no doesn't cause fault
- RDS cleanup is ok, but it doesn't appear to trigger an actual delete
- RDS clean up needs to remove ENI before Subnet removal, appears about 5 to 10 min wait
- EC2 can access PSQL
TODO:
- Validate cleanup tasks
  - RDS does not clean up
  - Subnet cannot remove due to RDS ENI
- Change to deploy multiple tower instances
- Integrate with Tower installation
