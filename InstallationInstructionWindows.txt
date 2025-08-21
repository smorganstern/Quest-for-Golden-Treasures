Setup Instructions (Windows)
1. Open Anaconda Command Prompt
Launch the Anaconda Prompt from the Start menu.

2. Check for Existing Environments
conda info --envs

### 3. Create a New Environment

conda create -n ai python=3.10 -y

### 4. Activate the Environment

conda activate ai

### 5. Install Required Packages

pip install ultralytics
pip install opencv-python
pip install pandas matplotlib

### 5. Verify YOLOv8 Installation

yolo version

### 6. Train or Run the Model 
* copy the pt file to the main directory before running.  Create a source video called gold.mp4 or change the source to an image or live camera.
yolo task=detect mode=predict model=goldlabels.pt source="gold.mp4"

### Optional GPU acceleration

Install the latest NVIDIA GPU drivers.
Install the CUDA Toolkit (matching the GPU and PyTorch requirements).
