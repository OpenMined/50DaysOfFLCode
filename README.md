<h1><img src="./assets/OpenMined-Icon.png" height="100">Day 01 - Your First Federated Learning Project</h1>

# Welcome to Day 1 of 50 Days of FL Code!

Welcome to your first day of the 50 Days of FL Code challenge! Today, we'll be setting up SyftBox and exploring its basic features to lay the groundwork for our federated learning journey.

## Today's Agenda

1. Introduction to SyftBox
2. Installation and Setup
3. Exploring Public and Private Spaces
4. Creating Your First Federated Learning Ring

## 1. Introduction to SyftBox

SyftBox is a powerful tool that combines file-sharing, network-aware file permissions, and background tasks to make Privacy-Enhancing Technologies (PETs) more accessible and practical. It allows for conditional data access, enabling federated learning and other privacy-preserving computations.

## 2. Installation and Setup

### Install SyftBox

Open your terminal and run the following command:

```bash
curl -LsSf https://syftbox.openmined.org/datasites/subha@openmined.org/install.sh | sh
```

If that doesn't work, try:

```bash
curl -LsSf https://syftbox.openmined.org/install.sh | sh
```

### Launch SyftBox

After installation, start the SyftBox client:

```bash
syftbox client
```

You should see a new SyftBox folder appear on your desktop with several subfolders.

## 3. Exploring Public and Private Spaces

### Public Space: Home.html

1. Navigate to your SyftBox folder
2. Create a new file called `home.html`
3. Add some content to your `home.html` file
4. Visit https://syftbox.openmined.org/datasites to see your public space

### Private Space: Echo App

1. In your SyftBox folder, create a new folder called `echo`
2. Inside the `echo` folder, create a file named `app.py`
3. Add the following code to `app.py`:

```python
import sys

def main():
    print("Hello from your private space!")
    if len(sys.argv) > 1:
        print(f"You said: {sys.argv[1]}")

if __name__ == "__main__":
    main()
```

4. Run your private app and observe the output in your terminal

### Semi-Public Space: chat.txt

1. Create a new folder called `chat` in your SyftBox folder
2. Inside the `chat` folder, create a file named `chat.txt`
3. Create a `_.syftperm` file in the same folder to define access permissions
4. Edit `chat.txt` and observe how permissions affect visibility

## 4. Creating Your First Federated Learning Ring

### Basic RING Setup

1. Create a new folder called `ring` in your SyftBox folder
2. Inside the `ring` folder, create a file named `data.json` with some sample data
3. Create a `ring.py` file with basic RING functionality
4. Run the RING and observe how data is shared and computed across nodes

### Building RING from Scratch

1. Create a new `custom_ring` folder
2. Implement basic RING functionality from scratch
3. Test your custom RING implementation

## Next Steps

- Experiment with different types of data in your RING
- Explore more advanced SyftBox features
- Prepare for upcoming apps: Ring-he, Ring-dp, and Ring-llm

Remember to share your progress on social media with #50DaysOfFLCode. Join us in the Slack channel to discuss your experience and get help if needed.

Tomorrow, we'll dive deeper into SyftBox's features and build a more complex federated learning system. Keep up the great work!

[<img src="./../assets/OpenMined-Logo-Light.png" alt="OpenMined" height="32" />](https://openmined.org)

Happy coding, and see you tomorrow for Day 2!
