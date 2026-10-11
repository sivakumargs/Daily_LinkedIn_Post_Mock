# Daily_LinkedIn_Post_Mock
Daily LinkedIn Post Mock

My DevSecOps notes, Linux commands, Docker setup, and hands-on labs

# Step 2 — Create a Markdown file
1. Open your newly created repository.
2. Click Add file → Create new file.
3. In the filename box, enter Docker-Setup.md. The .md extension means Markdown.
4. In the large editor below, type or paste the Markdown content shown in the next section.

# Step 3 — Write the content with large headings and smaller text
Copy the following example into the GitHub editor. This uses the same formatting technique as the screenshot.

    ## Step 1: Setup Linux VM (Amazon Linux AMI)
    
    1. Login to your AWS Cloud account.
    2. Create a Linux VM and connect to it using MobaXterm or SSH.
    
    ## Step 2: Install Docker in Amazon Linux VM
    
    Run the following commands:
    
    ```bash
    sudo yum update -y
    sudo yum install docker -y
    sudo systemctl start docker
    ```
    
    Enable Docker to start automatically:
    
    ```bash
    sudo systemctl enable docker
    ```
    
    Verify the Docker installation:
    
    ```bash
    docker --version
    sudo systemctl status docker
    ```
    
    ## Step 3: Verify Docker Installation
    
    Run a test container:
    
    ```bash
    sudo docker run hello-world
    ```
    
    If Docker is installed and running correctly, the command should display a confirmation message.
    
    ## Step 4: Important Notes
    
    - Keep your Linux system updated.
    - Avoid sharing SSH private keys.
    - Use least-privilege permissions.
    - Never commit passwords, private keys, or AWS credentials to GitHub.
    
    ## Step 5: Practice Task
    
    - [ ] Create an Amazon Linux VM.
    - [ ] Install Docker.
    - [ ] Start and enable the Docker service.
    - [ ] Verify Docker using the hello-world container.


# 4. Markdown heading cheat sheet
Keep this table handy when writing any DevSecOps documentation.

# Concepts Index

| Doc | Summary |
|---|---|

| What you type | What GitHub displays |
| --- | --- |
| # Step 1: Setup | Largest heading |
| ## Step 2: Install | Medium heading |
| ### Step 2.1: Configure | Smaller heading |
| Normal text here. |	Regular text |
| ** Important note ** |	Bold text |
| `docker --version` |	docker --version |
| Three backticks around commands |	Separate code block |
| - [ ] Practice task |	Unchecked checkbox |

**Note**: GitHub supports up to six heading levels, from # through ######. Use the levels in order to keep your document organized.

# Step 5 — Save the file in your repository
Once you are satisfied with the Preview:
  1. Click Commit changes….
  2. Enter a commit message, for example: Add Docker setup documentation.
  3. Select the option to commit directly to the main branch, if shown.
  4. Click Commit changes to save the file.
     
Your file is now stored in your repository. When you open Docker-Setup.md later, GitHub will display the formatted version by default.



