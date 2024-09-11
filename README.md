
# Git Basics

## 1. Set Up Your Project
- Create a new folder called `product-card`.
- Inside the folder, create a file named `index.html`.
- Add basic HTML structure to `index.html`.

## 2. Initialize Git
- Open the terminal in your project folder.
- Run the command `history -c` (optional step to clear terminal history).
- Run the command `git init` to initialize a new Git repository.

## 3. Check the Status of Your Repository
- Use `git status` to see the current status of your files.

## 4. Stage Your Changes
- Stage the `index.html` file using:
  ```bash
  git add index.html
  ```
- Verify the changes are staged using `git status`.

## 5. Commit Your Changes
- Commit your changes with a message using:
  ```bash
  git commit -m "Initial commit of index.html"
  ```

## 6. Add CSS
- Create a file named `styles.css`.
- Link the `styles.css` file to your HTML.
- Stage and commit the changes with an appropriate message using:
  ```bash
  git add .
  git commit -m "Added CSS file and linked it to HTML"
  ```
- Use `git status` to verify there is nothing left to commit.

## 7. Modify Your HTML File
- Add the basic structure of the product card in `index.html` with elements like the image, product name, price, rating, and button.
- Use the following command to stage and commit the changes directly:
  ```bash
  git commit -am "Added HTML structure for the product card"
  ```

## 8. Amend the Last Commit
- If you realize that you made a typo in your last commit message, amend it using:
  ```bash
  git commit --amend -m "Add HTML structure for the product card"
  ```

## 9. Add CSS for Styling
- Add basic styles in `styles.css` to center the card, set the font, and size elements appropriately.
- Make the page visually resemble the card in the image.
- Stage and commit these changes.

## 10. View Your Commit History
- Use `git log` to see the detailed history of your commits.
- Use `git log --oneline` to see a simplified version of the commit history.

## 11. Checkout to an Older Commit
- Use `git log --oneline` to find the commit hash of your first commit.
- Use `git checkout <commit-hash>` to view your project as it was at the initial commit (replace `<commit-hash>` with the actual hash).

## 12. Go Back to the Latest Commit
- Run `git checkout master` (or `main` if your branch is named differently) to return to the latest version of your project.

## 13. Create a .gitignore File
- In your project’s root directory, create a new file named `.gitignore`.
- Open the `.gitignore` file in your text editor and add the patterns or filenames of the files you want to ignore. Each line should contain one pattern. For example:
  ```plaintext
  # Ignore log files and node_modules folder
  *.log
  node_modules/
  ```
- Stage and commit the `.gitignore` file with an appropriate message:
  ```bash
  git add .gitignore
  git commit -m "Added .gitignore to exclude unnecessary files"
  ```
- To ensure the `.gitignore` works as expected, try adding a file that matches the patterns in `.gitignore` and verify that it doesn't show up in `git status`.

## 14. Save Command History
- Run the command to save your command history to a file:
  ```bash
  history > history.txt
  ```



