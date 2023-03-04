# Ansible Project

This is a project that uses Ansible to manage multiple servers. The project includes several roles that can be used to perform various tasks on the servers, including user management, package installation, and application deployment.

## Getting Started

To use this project, you will need to have Ansible installed on your local machine. You will also need to have SSH access to the servers you want to manage.

To get started, follow these steps:

1. Clone this repository to your local machine.
2. Modify the `hosts` file to include the IP addresses or hostnames of your servers.
3. Modify the `group_vars` files to include the variables specific to your environment.
4. Run the playbook(s) you want to use.

## Roles

The project includes the following roles:

- `create_users`: Creates users on all servers.
- `install_httpd`: Installs and starts the HTTPD service on the specified servers.
- `deploy_app`: Deploys a web application from a GitHub repository to the specified servers.
- `install_docker`: Installs Docker on the specified servers if they are in the dev group.
- `install_packages`: Installs NumPy and Pandas on all servers.
- `install_jenkins`: Installs Jenkins on the specified servers if they are in the prod group.

## Playbooks

The project includes several playbooks that use the roles to perform various tasks:

- `deploy.yml`: Deploys the web application to the specified servers.
- `install.yml`: Installs the required packages on all servers.
- `manage_users.yml`: Creates users on all servers.

## Contributing

Contributions to this project are welcome! If you have a suggestion or would like to contribute code, please create a pull request.
