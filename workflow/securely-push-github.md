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

1. **Create a GitHub App**:
   - Go to GitHub -> Settings -> Developer Settings -> GitHub Apps -> New GitHub App.
   - Fill in the required details and enable Device Flow.
   - Set repository permissions to "Read & Write".
   - Allow installation on "Any account".
   - Save the `Client ID` and `Public Link` as the admins require this information.

2. **Install the App**:
   - Follow instructions to install the GitHub App on your account or organization.
   - Select specific repositories to grant access.

3. **Contact Datahub Infra Admins**:
   - Request admins to add `gh-scoped-creds` to the Datahub instance you are using by using this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=felder%2Cbalajialg%2Cshaneknapp&labels=package-request&projects=&template=package_request.yml&title=Request+python+package+X+for+class+Y). Here is a [sample request](https://github.com/berkeley-dsep-infra/datahub/issues/4879) for adding `gh-scoped-creds` in Data100 hub. Please don't forget to add `Client ID` and `Public Link`


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