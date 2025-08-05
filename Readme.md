# Microservices Launcher

## Description

Launcher and orchestration layer for the Simple Store microservices architecture.

### Steps to Create Git Submodules

1. Create a new repository on GitHub
2. Clone the repository to your local machine
3. Add the submodules

   ```bash
   git submodule add <repository_url> <directory_name>
   ```

4. Add the changes to the repository (`git add`, `git commit`, `git push`)  
   Example:

   ```bash
   git add .
   git commit -m "Add submodule"
   git push
   ```

5. Initialize and update submodules. When someone clones the repository for the first time, they should run the following command to initialize and update the submodules:

   ```bash
   git submodule update --init --recursive
   ```

6. To update the submodule references:

   ```bash
   git submodule update --remote
   ```

## Important

If you're working in the repository that contains the submodules, **always update and push changes to the submodule first**, and **only then** push to the main repository.

Doing it in the reverse order may break the submodule references in the main repository and lead to conflicts.
