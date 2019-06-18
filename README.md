# markdown-templates
Saved Pull Request templates

## Using multiple PR templates
(take in mind that when using 1 unique PR template, it will be shown automatically when creating a new PR)

### 1. "the official" way

1. Include your saved PR templates into a repository-root/PULL_REQUEST_TEMPLATE folder (this must be in the repopsitory root and the templates in master before using it).
Name the templates in a easy-to-remember way.
2. Open the "New Pull Request" form, from any branch containing changes
3. Add the &template=name-of-the-template.md query string key-value
4. The selected template will be shown

### 2. Use the "Saved Replies" feature

1. Copy the template you want to use
2. Save it as a "Saved Reply" in the "New Pull Request" form
3. Use it

(note that it won't be shareable, so your team may have different templates at any time)


### 3. Use a unique PR template pointing to the other templates

1. Create an 'index template' as a PR template in repository-root/.github/PULL_REQUEST_TEMPLATE.md
    
    ```
    Use the PR template that better fits to this case:
    
    - [Hotfix template](./PULL_REQUEST_TEMPLATE/hotfix-default.md)
    - [Feature template](./PULL_REQUEST_TEMPLATE/feature-default.md)
    ```
    
2. When opening a new PR, the 'index template' will be shown and the developer should use which fits better to his needs