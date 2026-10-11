**Important:** Git does not track empty folders on their own. Create a file inside each folder to make it appear in your repository.

# Step 1: Setup Linux VM (Amazon Linux AMI)

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

