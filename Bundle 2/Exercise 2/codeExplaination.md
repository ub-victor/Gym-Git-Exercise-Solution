<style>
  .tag {
    display: inline-block;
    background-color: #007bff;
    color: white;
    padding: 5px 10px;
    border-radius: 5px;
    font-size: 14px;
    margin: 2px;
  }
</style>

# Project Title

## Exercise 2: Service Redesign

### Overview
In this exercise, we will be redesigning the `service.html` page and managing branches effectively.

### Steps

1. **Checkout Main Branch**
   - Command: `git checkout main`
   - Description: Switch to the main branch to ensure you have the latest changes.

2. **Create a New Branch**
   - Command: `git checkout -b <span class="tag">ft/service-redesign</span>`
   - Description: Create a new branch for the service redesign.

3. **Add Changes to `service.html`**
   - Description: Make necessary changes to the `service.html` page.

4. **Commit and Push Changes**
   - Commands:
     - `git add service.html`
     - `git commit -m "Redesign service page"`
     - `git push origin <span class="tag">ft/service-redesign</span>`
   - Description: Commit your changes and push them to the remote repository.

5. **Create a Pull Request**
   - Description: Open a PR for your changes against the main branch.

6. **Handle Merge Conflicts**
   - Description: If there are conflicts, resolve them by merging the main branch into your feature branch.

### Tags
- **Branching**: <span class="tag">ft/service-redesign</span>
- **Main Branch**: <span class="tag">main</span>
- **Pull Request**: <span class="tag">PR</span>
- **Merge Conflicts**: <span class="tag">conflict</span>