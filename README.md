# 🛒 Retail Customer Intelligence

## 🛠️ Setup

```bash
# 1. Create & activate the conda environment
conda create -n yolo_env python=3.12 -y
conda activate yolo_env

# 2. Install dependencies
pip install ultralytics opencv-python numpy ipykernel

# 3. Register Jupyter kernel
python -m ipykernel install --user --name=yolo_env --display-name "yolo_env"
```

> Model weights (`yolo26n.pt`) download automatically on first run.

## 🚀 Run

1. `jupyter notebook` → open **main.ipynb** → set kernel to **yolo_env** → run the cell.
2. A live preview window opens. Press **`q`** to stop early.
3. Output saves to `runs/detect/retail_analytics_output.mp4`.

To change the input video, edit `video_path` in the `main()` function. The system auto-detects the zone layout (checkout lanes vs. shopping corridor) based on the filename.