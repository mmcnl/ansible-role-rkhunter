## Example Playbook

    - hosts: all
      tasks:
        - import_role:
            name: rkhunter
          vars:
            rkhunter_notification_email: admin@example.com
            rkhunter_additional_config:
              - ALLOWHIDDENDIR=/etc/.git
              - ALLOWHIDDENFILE=/etc/.gitignore
              - ALLOWHIDDENFILE=/etc/.etckeeper

## License

MIT

