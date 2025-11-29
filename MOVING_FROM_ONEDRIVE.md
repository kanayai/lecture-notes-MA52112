# Moving Project Out of OneDrive

**CRITICAL:** Storing Git repositories inside OneDrive can cause data corruption and sync conflicts. Follow these steps to move your project to a safe local location and set it up on your other computers.

## Step 1: On THIS Computer (Where the code is now)

Since your code is already pushed to GitHub, it is safe to move.

1.  **Move the Folder:**
    *   Open Finder.
    *   Drag and drop the `lecture-notes` folder **OUT** of OneDrive.
    *   Move it to a local folder like `Documents` or `Projects` (e.g., `/Users/yourname/Documents/lecture-notes`).

2.  **Verify the Move:**
    *   Open your terminal.
    *   Navigate to the new location:
        ```bash
        cd ~/Documents/lecture-notes
        ```
    *   Run your sync script to ensure everything is connected:
        ```bash
        ./scripts/sync_work.sh
        ```

3.  **Cleanup OneDrive:**
    *   Check your OneDrive folder. If a copy of `lecture-notes` still exists there, **delete it**.

## Step 2: On Your OTHER Computer

When you switch to your second computer (e.g., Home PC or Office Mac):

1.  **Let OneDrive Sync:**
    *   Wait for OneDrive to update. It should automatically remove the `lecture-notes` folder since you deleted/moved it on the first computer.
    *   If it's still there, **delete it manually**.

2.  **Clone the Repository:**
    *   Open your terminal.
    *   Navigate to where you want the project to live (e.g., `Documents`):
        ```bash
        cd ~/Documents
        ```
    *   Download a fresh copy from GitHub:
        ```bash
        git clone https://github.com/kanayai/lecture-notes-MA52112.git
        ```

3.  **Setup the Script:**
    *   Enter the new folder:
        ```bash
        cd lecture-notes-MA52112
        ```
    *   Make the sync script executable:
        ```bash
        chmod +x scripts/sync_work.sh
        ```

## Daily Workflow

Now that you have two independent, safe copies, use the script to keep them in sync:

*   **Start of day:** Run `./scripts/sync_work.sh` (Pulls new work)
*   **End of day:** Run `./scripts/sync_work.sh` (Pushes your work)
