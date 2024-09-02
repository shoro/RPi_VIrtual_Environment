# Create a virtual environment on Raspberry Pi 4
To create a virtual environment on a Raspberry Pi 4, you'll typically be using Python's built-in **_'venv'_** module. Here's how you can do it step-by-step:

### 1. Update Your System:
First, ensure that your Raspberry Pi's package lists are up to date.
```
sudo apt-get update
sudo apt-get upgrade -y
```

### 2. Install Python (if not already installed):
Raspberry Pi OS usually comes with Python pre-installed. You can check if Python is installed by running:
```
python3 --version
```
If Python isn't installed, you can install it using:
```
sudo apt-get install python3
```

### 3. Install **_'venv'_** (if not already installed):
The **_'venv'_** module should come with Python by default, but if it’s not installed, you can install it with:
```
sudo apt-get install python3-venv
```

### 4. Create a Virtual Environment:
Navigate to the directory where you want to create your virtual environment or create a new directory:
```
mkdir myproject
cd myproject
```
Now, create a virtual environment using the following command:
```
python3 -m venv myenv
```
Here, **_'myenv'_** is the name of the virtual environment folder. You can name it whatever you like.

### 5. Activate the Virtual Environment:
To activate the virtual environment, use the following command:
```
source myenv/bin/activate
```
Once activated, your command prompt will change to show that you are now operating within the virtual environment.

### 6. Install Packages:
With the virtual environment activated, you can install packages using **_'pip'_**:
```
pip install <package-name>
```

### 7. Deactivate the Virtual Environment:
When you are done, you can deactivate the virtual environment by running:
```
deactivate
```
Your virtual environment on the Raspberry Pi 4 is now set up!
