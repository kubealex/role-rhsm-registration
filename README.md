# Ansible Role: role_rhsm_registration

An Ansible role to manage Red Hat Subscriptions using the `community.general.redhat_subscription` module.

## Role Variables

Below are the variables that can be customized when using this role:

- `role_rhsm_registration_activationkey`: Red Hat Subscription Manager activation key.
- `role_rhsm_registration_auto_attach`: Auto-attach flag.
- `role_rhsm_registration_consumer_id`: Red Hat Subscription Manager consumer ID.
- `role_rhsm_registration_consumer_name`: Red Hat Subscription Manager consumer name.
- `role_rhsm_registration_consumer_type`: Red Hat Subscription Manager consumer type.
- `role_rhsm_registration_environment`: Red Hat Subscription Manager environment.
- `role_rhsm_registration_force_register`: Force registration flag.
- `role_rhsm_registration_org_id`: Red Hat Subscription Manager organization ID.
- `role_rhsm_registration_password`: Red Hat Subscription Manager password.
- `role_rhsm_registration_pool_ids`: List of Red Hat Subscription Manager pool IDs.
- `role_rhsm_registration_release`: Red Hat Subscription Manager release.
- `role_rhsm_registration_rhsm_baseurl`: Red Hat Subscription Manager base URL.
- `role_rhsm_registration_rhsm_repo_ca_cert`: Red Hat Subscription Manager repository CA certificate.
- `role_rhsm_registration_server_hostname`: Red Hat Subscription Manager server hostname.
- `role_rhsm_registration_server_insecure`: Red Hat Subscription Manager server insecure flag.
- `role_rhsm_registration_server_port`: Red Hat Subscription Manager server port.
- `role_rhsm_registration_server_prefix`: Red Hat Subscription Manager server prefix.
- `role_rhsm_registration_server_proxy_hostname`: Red Hat Subscription Manager server proxy hostname.
- `role_rhsm_registration_server_proxy_password`: Red Hat Subscription Manager server proxy password.
- `role_rhsm_registration_server_proxy_port`: Red Hat Subscription Manager server proxy port.
- `role_rhsm_registration_server_proxy_scheme`: Red Hat Subscription Manager server proxy scheme.
- `role_rhsm_registration_server_proxy_user`: Red Hat Subscription Manager server proxy user.
- `role_rhsm_registration_state`: Desired state of the registration (default: present).
- `role_rhsm_registration_syspurpose`: Red Hat Subscription Manager system purpose.
- `role_rhsm_registration_token`: Red Hat Subscription Manager token.
- `role_rhsm_registration_username`: Red Hat Subscription Manager username.

## Examples


```yaml
- name: Manage Red Hat Subscriptions with Activation Key and Organization ID
  hosts: servers
  roles:
    - role: role_rhsm_registration
      role_rhsm_registration_activationkey: "your_activation_key"
      role_rhsm_registration_org_id: "your_organization_id"
```

```yaml
- name: Manage Red Hat Subscriptions with Username and Password
  hosts: servers
  roles:
    - role: role_rhsm_registration
      role_rhsm_registration_username: "your_username"
      role_rhsm_registration_password: "your_password"
```

```yaml
- name: Manage Red Hat Subscriptions with Username, Password, and List of Pool IDs
  hosts: servers
  roles:
    - role: role_rhsm_registration
      role_rhsm_registration_username: "your_username"
      role_rhsm_registration_password: "your_password"
      role_rhsm_registration_pool_ids:
        - "pool_id_1"
        - "pool_id_2"
```
