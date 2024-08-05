# Using gh-scoped-creds to securely push changes to Github repository

---

## **GitHub Scoped Credentials**

### Purpose:
[gh-scoped-creds](https://github.com/jupyterhub/gh-scoped-creds) allows instructors and students using Datahub to securely push changes to specific GitHub repositories without exposing broader access or long-term credentials.

### Goals:
1. **Secure Repository Access**: Users can push only to specific repositories.
2. **Temporary Credentials**: No long-term storage of sensitive data.
3. **Admin Control**: GitHub organization admins manage which repositories can be accessed.

### How It Works:
1. **GitHub App**: A GitHub app is created for Datahub.
2. **Temporary Tokens**: Use the command line tool `gh-scoped-creds` to get a temporary push token.
3. **Integration**: Use `%ghscopedcreds` in Jupyter notebooks for easy access.

### Requesting Access/Installation:

1. **Install the App**:
   - Install the [GitHub App](https://github.com/organizations/berkeley-dsep-infra/settings/apps/) tagged to your hub by clicking the green button "install". For Eg: If you are using Data 100 hub then install "data100 Berkeley Datahub Access" Github app
   - Select specific repositories for which you want to grant read and write access.

2. **Contact Datahub Infra Admins**:
   - Request admins to add `gh-scoped-creds` to the hub's image by specifying the hub you are using via this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=felder%2Cbalajialg%2Cshaneknapp&labels=package-request&projects=&template=package_request.yml&title=Request+python+package+X+for+class+Y). Here is a [sample request](https://github.com/berkeley-dsep-infra/datahub/issues/4879) for adding `gh-scoped-creds` in Data100 hub. 

### Using the Tool:

1. **Run the Tool**:
    ```bash
    gh-scoped-creds
    ```
   - Follow the instructions to authenticate and obtain a temporary token.

2. **In Jupyter Notebook**:
    ```python
    import gh_scoped_creds
    %ghscopedcreds
    ```
   - Authenticate as prompted.

### Security Notes:
- Authentication lasts for 8 hours.
- Regularly update permissions to ensure security.

### Troubleshooting:
- Check the GitHub App settings for correct permissions.

For more details, visit the [GitHub repository](https://github.com/jupyterhub/gh-scoped-creds).