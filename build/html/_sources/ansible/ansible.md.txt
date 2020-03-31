# Ansible Notes

- Pause the Playbook task execution

  ```yaml
  - pause:
  minutes: 1
  ```

- Run VM Provisioning Workflow

  ```yaml
  tower-cli workflow_job launch --workflow-job-template=92 -e @~/vm_build.yaml
  ```

* Do Until Loop

  ```yaml
  register: copy_to_iso
  until: copy_to_iso is succeeded
  retries: 5
  delay: 10
  ```

* Pull variable from previous plays/roles

  ```yaml
  "{{ hostvars['host_from_previous_play'].variable_you_want }}"
  ```
